---
title: Etki alanına birleştirilmiş Windows 10 aygıtlarını iş için Microsoft 365 tarafından yönetilmesini etkinleştirin
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
description: Microsoft 365'in yerel Active-Directory'ye katılan Windows 10 aygıtlarını yalnızca birkaç adımda nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560853"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="a567a-103">Etki alanına bağlı Windows 10 cihazlarının Microsoft 365 Business Premium tarafından yönetilmesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="a567a-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a567a-104">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a567a-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="a567a-105">Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a567a-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a567a-106">Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="a567a-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="a567a-107">Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacağına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="a567a-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="a567a-108">Başlamadan önce şu adımları tamamladığınızdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="a567a-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="a567a-109">Azure AD Connect ile kullanıcıları Azure AD ile senkronize edin.</span><span class="sxs-lookup"><span data-stu-id="a567a-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="a567a-110">Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="a567a-111">Eşitlediğiniz tüm etki alanı kullanıcılarının Microsoft 365 Business Premium lisansına sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a567a-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a567a-112">Bkz. Adımlar için [etki alanı kullanıcılarını Microsoft'a senkronize edin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="a567a-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="a567a-113">1. Intune MDM Yetki doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a567a-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="a567a-114">[Endpoint Manager'a](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) gidin ve Microsoft Intune sayfasında Cihaz **kaydını**seçin ve ardından **Genel Bakış** sayfasında **MDM yetkilisinin** **Intune**olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a567a-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="a567a-115">**MDM yetkisi** **Yok**ise, **Intune**ayarlamak için **MDM yetkisini** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a567a-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="a567a-116">**MDM yetkisi** **Microsoft Office 365**ise, **Aygıtlar**Kayıt  >  **aygıtlarına** gidin ve **Intune MDM** yetkilisi ekleme hakkını sağdaki **MDM yetki** ekle iletişim kutusunu kullanın **(MDM Yetkilisi Ekle** iletişim kutusu yalnızca **MDM Yetkilisi** Microsoft Office 365'e ayarlanırsa kullanılabilir).</span><span class="sxs-lookup"><span data-stu-id="a567a-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="a567a-117">2. Bilgisayarlara katılmak için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a567a-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="a567a-118">Yönetici merkezleri listesinde yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve Azure **Active Directory'yi** seçin (Azure **Admin centers** Etkin Dizini görünmüyorsa tümünü göster'i seçin).</span><span class="sxs-lookup"><span data-stu-id="a567a-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="a567a-119">Azure **Etkin Dizin yönetici merkezinde,** **Azure Etkin Dizin'e** gidin, **Aygıtlar'ı** seçin ve ardından **Aygıt ayarlarını seçin.**</span><span class="sxs-lookup"><span data-stu-id="a567a-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="a567a-120">**Kullanıcıların Azure AD'de aygıtlara katılıp katılamayada** olabileceğini doğrulayın etkin</span><span class="sxs-lookup"><span data-stu-id="a567a-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="a567a-121">Tüm kullanıcıları etkinleştirmek için **Tümü'ne**ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="a567a-122">Belirli kullanıcıları etkinleştirmek için, belirli bir kullanıcı grubunu etkinleştirmek için **Seçili** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="a567a-123">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a567a-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="a567a-124">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="a567a-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="a567a-125">3. MDM için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a567a-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="a567a-126">Yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve **Endpoint Managemen**t'yi seçin **(Endpoint Manager** görünmüyorsa **tümünü göster'i** seçin)</span><span class="sxs-lookup"><span data-stu-id="a567a-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="a567a-127">Microsoft **Endpoint Manager yönetici merkezinde,** **Windows**Windows Kayıt Otomatik Kayıt Cihazlar  >  **Windows**  >  **Windows Enrollment**  >  **Automatic Enrollment**gidin.</span><span class="sxs-lookup"><span data-stu-id="a567a-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="a567a-128">MDM kullanıcı kapsamının etkin olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="a567a-129">Tüm bilgisayarları kaydetmek için, kullanıcılar Windows'a bir iş hesabı eklediğinde Azure AD'ye katılan tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydetmek için **Tümü'ne** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="a567a-130">Belirli bir kullanıcı grubunun bilgisayarlarını kaydetmek için **Bazıları'na** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="a567a-131">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a567a-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="a567a-132">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="a567a-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="a567a-133">4. Gerekli kaynakları oluşturma</span><span class="sxs-lookup"><span data-stu-id="a567a-133">4. Create the required resources</span></span> 

<span data-ttu-id="a567a-134">[Karma Azure AD birleştirmeyapılandırmak](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) için gerekli görevlerin yerine getirilmesi, [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'inin kullanımı yla basitleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="a567a-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="a567a-135">Bu cmdlet'i çağırdığınızda, gerekli servis bağlantı noktası ve grup ilkesini oluşturur ve yapılandıracaktır.</span><span class="sxs-lookup"><span data-stu-id="a567a-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="a567a-136">PowerShell örneğinden aşağıdakileri çağırarak bu modülü yükleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="a567a-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="a567a-137">Bu modülü Azure AD Connect çalıştıran Windows Server'a yüklemeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="a567a-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="a567a-138">Gerekli servis bağlantı noktası ve grup ilkesini oluşturmak için [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırırsınız.</span><span class="sxs-lookup"><span data-stu-id="a567a-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="a567a-139">Bu görevi yerine getirirken Microsoft 365 Business Premium global yönetici kimlik bilgilerinize ihtiyacınız olacaktır.</span><span class="sxs-lookup"><span data-stu-id="a567a-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="a567a-140">Kaynakları oluşturmaya hazır olduğunuzda aşağıdakileri çağırın:</span><span class="sxs-lookup"><span data-stu-id="a567a-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="a567a-141">İlk komut Microsoft bulutuyla bir bağlantı kurar ve sizden istendiğinde Microsoft 365 Business Premium global yönetici kimlik bilgilerinizi belirtin.</span><span class="sxs-lookup"><span data-stu-id="a567a-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="a567a-142">5. Grup İlkesini Bağla</span><span class="sxs-lookup"><span data-stu-id="a567a-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="a567a-143">Grup İlkesi Yönetim Konsolu'nda (GPMC), politikayı bağlamak istediğiniz konuma sağ tıklayın ve bağlam menüsünden *varolan bir GPO'yu bağlayın...* seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="a567a-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="a567a-144">Yukarıdaki adımda oluşturulan ilkeyi seçin ve **ardından Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a567a-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="a567a-145">En son Yönetim Şablonlarını Alın</span><span class="sxs-lookup"><span data-stu-id="a567a-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="a567a-146">**Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bunun nedeni Windows 10, sürüm 1803, sürüm 1809 veya sürüm 1903 için ADMX yüklü değil.</span><span class="sxs-lookup"><span data-stu-id="a567a-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="a567a-147">Sorunu gidermek için aşağıdaki adımları izleyin (Not: en son MDM.admx geriye dönük uyumludur):</span><span class="sxs-lookup"><span data-stu-id="a567a-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="a567a-148">Indirin: [Windows 10 Mayıs 2019 Güncelleştirmesi (1903) için Yönetim Şablonları (.admx)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="a567a-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="a567a-149">Paketi Birincil Etki Alanı Denetleyicisi'ne (PDC) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="a567a-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="a567a-150">Klasöre sürülmeye bağlı olarak gidin: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 Mayıs 2019 Güncelleştirmesi (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="a567a-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="a567a-151">**İlke** **Tanımları** klasörünü yukarıdaki yolda Yeniden adlandırın.</span><span class="sxs-lookup"><span data-stu-id="a567a-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="a567a-152">**İlke Tanımlar** klasörünü **C:\Windows\SYSVOL\domain\İlkeler'e**kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="a567a-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="a567a-153">Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, PolicyDefinitions'ın içeriğini oraya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a567a-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="a567a-154">İlkenin kullanılabilir olması için Birincil Etki Alanı Denetleyicisini yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="a567a-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="a567a-155">Bu yordam, gelecekteki herhangi bir sürüm için de çalışacaktır.</span><span class="sxs-lookup"><span data-stu-id="a567a-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="a567a-156">Bu noktada, kullanılabilir varsayılan Azure **REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir** ilkesini görebilmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="a567a-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
