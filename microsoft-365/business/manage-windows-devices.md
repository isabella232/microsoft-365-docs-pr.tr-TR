---
title: Etki alanına katılmış Windows 10 cihazlarını kurumsal cihazlar tarafından yönetil Microsoft 365 etkinleştirme
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Yalnızca birkaç adımda Microsoft 365 Active-Directory'ye katılmış yerel Windows 10 cihazlarını nasıl koruyabilirsiniz hakkında bilgi edinebilirsiniz.
ms.openlocfilehash: f16962dd3c33c3c228da507bc5c4a902d76a8a08
ms.sourcegitcommit: b0d3abbccf4dd37e32d69664d3ebc9ab8dea760d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/21/2021
ms.locfileid: "52593903"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="05c07-103">Etki alanına katılmış Windows 10 cihazları başka bir kullanıcı tarafından yönetil Microsoft 365 İş Ekstra</span><span class="sxs-lookup"><span data-stu-id="05c07-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="05c07-104">Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Microsoft 365 İş Ekstra cihazlarınızı korumak için Windows 10'i kurabilirsiniz ve bu sırada yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="05c07-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="05c07-105">Bu korumayı ayarlamak için Azure **AD'ye katılan Karma cihazları kullanabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="05c07-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="05c07-106">Bu cihazlar hem şirket içi Active Directory'nize hem de kullanıcılarınıza Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="05c07-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="05c07-107">Bu videoda, bunu en yaygın senaryo için ayarlama adımları açıklanan ve aşağıdaki adımlarda da ayrıntılı olarak açıklanan bir anlatı yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="05c07-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="05c07-108">Başlamadan önce şu adımları tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="05c07-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="05c07-109">Azure AD hizmetleriyle kullanıcıları Azure AD'ye Bağlan.</span><span class="sxs-lookup"><span data-stu-id="05c07-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="05c07-110">Azure AD Kurumsal Bağlan (OU) eşitlemeyi tamamlama.</span><span class="sxs-lookup"><span data-stu-id="05c07-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="05c07-111">Eşitleyilen tüm etki alanı kullanıcılarının lisanslarının olduğundan emin Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="05c07-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="05c07-112">Adımlar [için bkz. Etki alanı kullanıcılarını Microsoft](manage-domain-users.md) ile eşitleme.</span><span class="sxs-lookup"><span data-stu-id="05c07-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="05c07-113">1. Intune'da MDM Yetkilisini doğrulama</span><span class="sxs-lookup"><span data-stu-id="05c07-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="05c07-114">Endpoint Manager'a gidin ve Microsoft Intune kayıt öğesini seçin, ardından Genel Bakış  sayfasında **MDM yetkilisinin** **Intune** olduğundan emin olun. [](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview)</span><span class="sxs-lookup"><span data-stu-id="05c07-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="05c07-115">**MDM yetkilisi Yok** **ise,** **MDM yetkilisine tıklarsanız** bunu **Intune olarak ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="05c07-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="05c07-116">**MDM** yetkilisi **Microsoft Office 365** ise Cihazlar Kaydetme cihazları'na gidin ve   >   **intune MDM** yetkilisini eklemek için sağ dosyanın **MDM** yetkilisini ekle iletişim kutusunu kullanın **(MDM** Yetkili Ekle iletişim kutusu yalnızca **MDM** Yetkilisi Ekle seçeneği Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="05c07-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="05c07-117">2. Bilgisayarları birleştirme için Azure AD'nin etkinleştirildiğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="05c07-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="05c07-118">Yönetim merkezi'ne gidin ve Yönetim Azure Active Directory listesinden Bir Azure Active Directory'ı seçin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  **(Azure Active Directory'ı** seçin).</span><span class="sxs-lookup"><span data-stu-id="05c07-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="05c07-119">Yönetim Azure Active Directory **gidin,** Cihazlar'ı  Azure Active Directory ve **ardından Cihaz** **ayarları'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="05c07-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="05c07-120">Kullanıcıların **cihazlarda Azure AD'ye katılanın etkinleştirildiğinden** emin olun</span><span class="sxs-lookup"><span data-stu-id="05c07-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="05c07-121">Tüm kullanıcıları etkinleştirmek için, Tüm olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="05c07-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="05c07-122">Belirli kullanıcıları etkinleştirmek için, belirli bir **kullanıcı** grubunu etkinleştirmek üzere Seçili olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="05c07-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="05c07-123">Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="05c07-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="05c07-124">Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.</span><span class="sxs-lookup"><span data-stu-id="05c07-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="05c07-125">3. MDM için Azure AD'nin etkinleştirildiğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="05c07-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="05c07-126">Yönetim merkezine gidin ve Uç <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> Nokta Yönetimi **t'yi**  seçin (Uç nokta görünmüyorsa Endpoint Manager'i seçin) </span><span class="sxs-lookup"><span data-stu-id="05c07-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="05c07-127">Genel **Microsoft Endpoint Manager merkezinde Cihazlar ve** **Kayıt**  >  **Windows** Windows  >  **gidin.**  >  </span><span class="sxs-lookup"><span data-stu-id="05c07-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="05c07-128">MDM kullanıcı kapsamının etkinleştirildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="05c07-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="05c07-129">Tüm bilgisayarları kaydetmek için, Azure AD'ye katılmış tüm kullanıcı bilgisayarlarını ve kullanıcılar Windows'e iş hesabı eklensin, yeni bilgisayarlar otomatik olarak kaydedilir. </span><span class="sxs-lookup"><span data-stu-id="05c07-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="05c07-130">Belirli bir **kullanıcı** grubunun bilgisayarlarını kaydetmek için Bazıları olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="05c07-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="05c07-131">Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="05c07-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="05c07-132">Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.</span><span class="sxs-lookup"><span data-stu-id="05c07-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="05c07-133">4. Gerekli kaynakları oluşturma</span><span class="sxs-lookup"><span data-stu-id="05c07-133">4. Create the required resources</span></span> 

<span data-ttu-id="05c07-134">Karma [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) birleştirmesini yapılandırmak için gereken görevlerin gerçekleştirilip, [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'i kullanımı basitleştirildi.</span><span class="sxs-lookup"><span data-stu-id="05c07-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="05c07-135">Bu cmdlet'i çağırıldığında, gerekli hizmet bağlantı noktası ve grup ilkesi oluşturulacak ve yapılandırılır.</span><span class="sxs-lookup"><span data-stu-id="05c07-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="05c07-136">Bu modülü, bir PowerShell örneğinden aşağıdakini faturalamaya göre yükleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="05c07-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="05c07-137">Bu modülü, Azure AD Bağlan çalıştıran Windows Server'a yüklemeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="05c07-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="05c07-138">Gerekli hizmet bağlantı noktası ve grup ilkesi oluşturmak  [için, Başlat-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırmış olursunuz.</span><span class="sxs-lookup"><span data-stu-id="05c07-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="05c07-139">Bu görevi yerine Microsoft 365 İş Ekstra yönetici kimlik bilgileriniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="05c07-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="05c07-140">Kaynakları oluşturmak için hazır olduğunda, aşağıdakini çağırın:</span><span class="sxs-lookup"><span data-stu-id="05c07-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="05c07-141">İlk komut Microsoft bulut ile bağlantı kuracak ve sizden istendiğinde genel yönetici Microsoft 365 İş Ekstra bilgilerinizi belirtir.</span><span class="sxs-lookup"><span data-stu-id="05c07-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="05c07-142">5. Grup İlkesini Bağlama</span><span class="sxs-lookup"><span data-stu-id="05c07-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="05c07-143">Grup İlkesi Yönetim Konsolu'nda (GPMC), ilkeyi bağlamayı istediğiniz konuma sağ tıklayın ve bağlam menüsünde Var olan *GPO'ya bağlantı...* öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="05c07-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="05c07-144">Yukarıdaki adımda oluşturulan ilkeyi seçin ve Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="05c07-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="05c07-145">En son Yönetim Şablonlarını Al</span><span class="sxs-lookup"><span data-stu-id="05c07-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="05c07-146">Otomatik **MDM** kaydı varsayılan Azure AD kimlik bilgilerini kullanarak etkinleştir ayarını görmüyorsanız bunun nedeni, Windows 10 sürüm 1803 veya daha sonraki sürümlerde ADMX'in yüklü olması olabilir.</span><span class="sxs-lookup"><span data-stu-id="05c07-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="05c07-147">Sorunu düzeltmek için şu adımları izleyin (Not: en son MDM.admx geriye dönük uyumlu):</span><span class="sxs-lookup"><span data-stu-id="05c07-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="05c07-148">İndirin: [Ekim 2020 Güncelleştirmesi'ne (20H2) Windows 10 Yönetim Şablonları (.admx).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="05c07-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="05c07-149">Paketi Etki Alanı Denetleyicisi'ne yükleyin.</span><span class="sxs-lookup"><span data-stu-id="05c07-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="05c07-150">Yönetim Şablonları sürümüne bağlı olarak şu klasöre gidin: **C:\Program Files (x86)\Microsoft Grup İlkesi\Windows 10 Ekim 2020 Güncelleştirmesi (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="05c07-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="05c07-151">Yukarıdaki **yolda İlke Tanımları** klasörünü **PolicyDefinitions olarak yeniden adlandırabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="05c07-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="05c07-152">Varsayılan olarak **POLICYDefinitions** klasörünü SYSVOL paylaşımınıza kopyalayın; varsayılan olarak **C:\Windows\SYSVOL\domain\Policies konumundadır.**</span><span class="sxs-lookup"><span data-stu-id="05c07-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="05c07-153">Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, PolicyDefinitions içeriğini oraya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="05c07-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="05c07-154">Birden fazla Etki Alanı Denetleyicisi olması durumunda, ilkelerin kullanılabilir olması için SYSVOL'nin çoğaltmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="05c07-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="05c07-155">Bu yordam, Yönetim Şablonlarının gelecek tüm sürümü için de kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="05c07-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="05c07-156">Bu noktada, Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik **MDM kaydı etkinleştir'i görüyor olması** gerekir.</span><span class="sxs-lookup"><span data-stu-id="05c07-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="05c07-157">İlgili içerik</span><span class="sxs-lookup"><span data-stu-id="05c07-157">Related content</span></span>

<span data-ttu-id="05c07-158">[Etki alanı kullanıcılarını yeni Microsoft 365](manage-domain-users.md) (makale)</span><span class="sxs-lookup"><span data-stu-id="05c07-158">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>

<span data-ttu-id="05c07-159">[Yönetim merkezinde grup oluşturma](../admin/create-groups/create-groups.md) (makale)</span><span class="sxs-lookup"><span data-stu-id="05c07-159">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>

<span data-ttu-id="05c07-160">[Öğretici: Yönetilen etki Azure Active Directory için karma etki alanlarını yapılandırma](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (makale)</span><span class="sxs-lookup"><span data-stu-id="05c07-160">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>