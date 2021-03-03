---
title: Etki alanına katılmış Windows 10 cihazlarının Microsoft 365 İş tarafından yönetilsini etkinleştirme
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Microsoft 365'in yalnızca birkaç adımda Active Directory'ye katılmış yerel Windows 10 cihazlarını korumayı nasıl etkinleştirebilirsiniz?
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407088"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="d30cd-103">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş Ekstra tarafından yönetillerini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="d30cd-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d30cd-104">Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 İş Ekstra'nın ayarlamasını yaparken, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d30cd-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="d30cd-105">Bu korumayı ayarlamak için, Karma **Azure AD'ye katılmış cihazları kullanabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="d30cd-106">Bu cihazlar hem şirket içi Active Directory'nize hem de Azure Active Directory'nize katılmış olur.</span><span class="sxs-lookup"><span data-stu-id="d30cd-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="d30cd-107">Bu videoda, bunu en yaygın senaryo için ayarlama adımları açıklanan ve aşağıdaki adımlarda da ayrıntılı olarak açıklanan bir senaryo yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="d30cd-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="d30cd-108">Başlamadan önce şu adımları tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="d30cd-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="d30cd-109">Azure AD Connect ile kullanıcıları Azure AD'ye eşitle.</span><span class="sxs-lookup"><span data-stu-id="d30cd-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="d30cd-110">Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlama.</span><span class="sxs-lookup"><span data-stu-id="d30cd-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="d30cd-111">Eşitleyilen tüm etki alanı kullanıcılarının Microsoft 365 İş Ekstra lisansları olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="d30cd-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="d30cd-112">Adımlar [için bkz. Etki alanı kullanıcılarını Microsoft'a](manage-domain-users.md) eşitleme.</span><span class="sxs-lookup"><span data-stu-id="d30cd-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="d30cd-113">1. Intune'da MDM Yetkilisini doğrulama</span><span class="sxs-lookup"><span data-stu-id="d30cd-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="d30cd-114">Uç Nokta [Yöneticisi'ne](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) gidin ve Microsoft Intune sayfasında  Cihaz kaydı'na tıklayın, ardından Genel Bakış sayfasında **MDM** yetkilisinin **Intune** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="d30cd-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="d30cd-115">**MDM yetkilisi Yok** **ise,** **MDM yetkilisini** **intune** olarak ayarlamak için tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d30cd-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="d30cd-116">**MDM** yetkilisi **Microsoft Office 365** ise Cihazları Kaydetme cihazlarına gidin ve   >   **Intune MDM** yetkilisini eklemek için sağdan **MDM** yetkili ekle iletişim kutusunu kullanın **(MDM** Yetkilisini Ekle iletişim kutusu yalnızca **MDM** Yetkilisi Microsoft Office 365 olarak ayarlanmışsa kullanılabilir).</span><span class="sxs-lookup"><span data-stu-id="d30cd-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="d30cd-117">2. Bilgisayarları birleştirme için Azure AD'nin etkinleştirildiğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="d30cd-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="d30cd-118">Yönetim merkezi listesinden yönetim merkezine gidin ve Azure Active Directory'yi seçin (Azure Active Directory görünür durumda değilse hepsini <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **göster'i** seçin). </span><span class="sxs-lookup"><span data-stu-id="d30cd-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="d30cd-119">Azure **Active Directory yönetim merkezinde,** **Azure Active Directory'ye** gidin, Cihazlar'ı **ve ardından** Cihaz **ayarlarını seçin.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="d30cd-120">Kullanıcıların **cihazları Azure AD'ye katılanın etkinleştiril** olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="d30cd-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="d30cd-121">Tüm kullanıcıları etkinleştirmek için, All olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="d30cd-122">Belirli kullanıcıları etkinleştirmek için, belirli bir **kullanıcı grubunu** etkinleştirmek üzere Seçili olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="d30cd-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="d30cd-123">Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d30cd-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="d30cd-124">Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="d30cd-125">3. MDM için Azure AD'nin etkinleştirildiğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="d30cd-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="d30cd-126">Yönetim merkezine gidin ve Uç Nokta Yönetimi t'yi seçin (Uç Nokta Yöneticisi görünür durumda <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> değilse Hepsini göster'i seçin)  </span><span class="sxs-lookup"><span data-stu-id="d30cd-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="d30cd-127">Microsoft **Endpoint Manager yönetim merkezinde Cihazlar** Windows Kaydı Otomatik   >    >  **Kaydı'ne**  >  **gidin.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="d30cd-128">MDM kullanıcı kapsamının etkinleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="d30cd-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="d30cd-129">Tüm bilgisayarları kaydetmek için, Kullanıcılar Windows'a iş hesabı eklensinken Azure AD'ye katılmış tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydeden All olarak ayarlayın. </span><span class="sxs-lookup"><span data-stu-id="d30cd-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="d30cd-130">Belirli bir **kullanıcı** grubunun bilgisayarlarını kaydetmek için Bazıları olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="d30cd-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="d30cd-131">Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d30cd-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="d30cd-132">Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="d30cd-133">4. Gerekli kaynakları oluşturma</span><span class="sxs-lookup"><span data-stu-id="d30cd-133">4. Create the required resources</span></span> 

<span data-ttu-id="d30cd-134">Karma [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) birleştirmesini yapılandırmak için gereken görevlerin gerçekleştirilip [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'i kullanımı basitleştirildi.</span><span class="sxs-lookup"><span data-stu-id="d30cd-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="d30cd-135">Bu cmdlet'i çağırıldığında, gerekli hizmet bağlantı noktası ve grup ilkesi oluşturularak yapılandırılır.</span><span class="sxs-lookup"><span data-stu-id="d30cd-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="d30cd-136">Bir PowerShell örneğinden aşağıdakini kullanarak bu modülü yükleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="d30cd-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="d30cd-137">Bu modülü Azure AD Connect çalıştıran Windows Server'a yüklemeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="d30cd-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="d30cd-138">Gerekli hizmet bağlantı noktası ve grup ilkesi oluşturmak  [için, Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırmış olursunuz.</span><span class="sxs-lookup"><span data-stu-id="d30cd-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="d30cd-139">Bu görevi gerçekleştirmek için Microsoft 365 İş Ekstra genel yönetici kimlik bilgileriniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d30cd-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="d30cd-140">Kaynakları oluşturmaya hazır olduğunda, aşağıdakini çağırın:</span><span class="sxs-lookup"><span data-stu-id="d30cd-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="d30cd-141">İlk komut Microsoft bulutuyla bağlantı kuracak ve sizden istendiğinde Microsoft 365 İş Ekstra genel yönetici kimlik bilgilerinizi belirtir.</span><span class="sxs-lookup"><span data-stu-id="d30cd-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="d30cd-142">5. Grup İlkesini bağlama</span><span class="sxs-lookup"><span data-stu-id="d30cd-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="d30cd-143">Grup İlkesi Yönetim Konsolu'nda (GPMC), ilkeyi bağlamayı istediğiniz konuma sağ tıklayın ve bağlam menüsünden Var olan *bir GPO'ya bağla...* öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="d30cd-144">Yukarıdaki adımda oluşturulan ilkeyi seçin ve Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="d30cd-145">En son Yönetim Şablonlarını al</span><span class="sxs-lookup"><span data-stu-id="d30cd-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="d30cd-146">Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik **MDM** kaydı etkinleştir ilkesini görmüyorsanız bunun nedeni Windows 10, sürüm 1803 veya sonraki sürümlerde ADMX'in yüklü olması olabilir.</span><span class="sxs-lookup"><span data-stu-id="d30cd-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="d30cd-147">Sorunu düzeltmek için şu adımları izleyin (Not: En son MDM.admx geriye doğru uyumludur):</span><span class="sxs-lookup"><span data-stu-id="d30cd-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="d30cd-148">İndir: [Windows 10 Ekim 2020 Güncelleştirmesi (20H2)](https://www.microsoft.com/download/102157)için Yönetim Şablonları (.admx).</span><span class="sxs-lookup"><span data-stu-id="d30cd-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="d30cd-149">Paketi Etki Alanı Denetleyicisi'ne yükleyin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="d30cd-150">Yönetim Şablonları sürümüne bağlı olarak şu klasöre gidin: **C:\Program Files (x86)\Microsoft Grup İlkesi\Windows 10 Ekim 2020 Güncelleştirmesi (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="d30cd-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="d30cd-151">Yukarıdaki **yolda İlke Tanımları** klasörünü **policyDefinitions olarak yeniden adlandırabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="d30cd-152">**PolicyDefinitions klasörünü** varsayılan olarak **C:\Windows\SYSVOL\domain\Policies** konumunda bulunan SYSVOL paylaşımınıza kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="d30cd-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="d30cd-153">Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, policyDefinitions içeriğini buraya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="d30cd-154">Birden fazla Etki Alanı Denetleyici varsa, ilkelerin kullanılabilir olması için SYSVOL'nin çoğaltmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="d30cd-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="d30cd-155">Bu yordam, Yönetim Şablonları'nın gelecekteki tüm sürümü için de çalışır.</span><span class="sxs-lookup"><span data-stu-id="d30cd-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="d30cd-156">Bu noktada, varsayılan Azure AD kimlik bilgilerini kullanarak otomatik **MDM kaydı etkinleştirme ilkesine bakabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="d30cd-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
