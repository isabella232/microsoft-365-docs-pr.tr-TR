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
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533795"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="9ca85-103">Etki alanına bağlı Windows 10 cihazlarının Microsoft 365 Business Premium tarafından yönetilmesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="9ca85-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="9ca85-104">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9ca85-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="9ca85-105">Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9ca85-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="9ca85-106">Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="9ca85-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="9ca85-107">Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacağına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="9ca85-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="9ca85-108">Başlamadan önce şu adımları tamamladığınızdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="9ca85-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="9ca85-109">Azure AD Connect ile kullanıcıları Azure AD ile senkronize edin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="9ca85-110">Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="9ca85-111">Eşitlediğiniz tüm etki alanı kullanıcılarının Microsoft 365 Business Premium lisansına sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ca85-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="9ca85-112">Bkz. Adımlar için [etki alanı kullanıcılarını Microsoft'a senkronize edin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="9ca85-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="9ca85-113">1. Intune MDM Yetki doğrulayın</span><span class="sxs-lookup"><span data-stu-id="9ca85-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="9ca85-114">portal.azure.com gidin ve Intune için sayfa arama üst kısmında.</span><span class="sxs-lookup"><span data-stu-id="9ca85-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="9ca85-115">Microsoft Intune sayfasında Cihaz **kaydını** seçin ve **Genel Bakış** sayfasında **MDM yetkilisinin** **Intune**olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ca85-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="9ca85-116">**MDM yetkisi** **Yok**ise, **Intune**ayarlamak için **MDM yetkisini** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="9ca85-117">**MDM yetkisi** **Microsoft Office 365**ise, **Aygıtlar**Kayıt  >  **aygıtlarına** gidin ve **Intune MDM** yetkilisi ekleme hakkını sağdaki **MDM yetki** ekle iletişim kutusunu kullanın **(MDM Yetkilisi Ekle** iletişim kutusu yalnızca **MDM Yetkilisi** Microsoft Office 365'e ayarlanırsa kullanılabilir).</span><span class="sxs-lookup"><span data-stu-id="9ca85-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="9ca85-118">2. Bilgisayarlara katılmak için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="9ca85-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="9ca85-119">Yönetici merkezleri listesinde yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve Azure **Active Directory'yi** seçin (Azure **Admin centers** Etkin Dizini görünmüyorsa tümünü göster'i seçin).</span><span class="sxs-lookup"><span data-stu-id="9ca85-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="9ca85-120">Azure **Etkin Dizin yönetici merkezinde,** **Azure Etkin Dizin'e** gidin, **Aygıtlar'ı** seçin ve ardından **Aygıt ayarlarını seçin.**</span><span class="sxs-lookup"><span data-stu-id="9ca85-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="9ca85-121">**Kullanıcıların Azure AD'de aygıtlara katılıp katılamayada** olabileceğini doğrulayın etkin</span><span class="sxs-lookup"><span data-stu-id="9ca85-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="9ca85-122">Tüm kullanıcıları etkinleştirmek için **Tümü'ne**ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="9ca85-123">Belirli kullanıcıları etkinleştirmek için, belirli bir kullanıcı grubunu etkinleştirmek için **Seçili** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="9ca85-124">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="9ca85-125">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="9ca85-126">3. MDM için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="9ca85-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="9ca85-127">Yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve **Endpoint Managemen**t'yi seçin **(Endpoint Manager** görünmüyorsa **tümünü göster'i** seçin)</span><span class="sxs-lookup"><span data-stu-id="9ca85-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="9ca85-128">Microsoft **Endpoint Manager yönetici merkezinde,** **Windows**Windows Kayıt Otomatik Kayıt Cihazlar  >  **Windows**  >  **Windows Enrollment**  >  **Automatic Enrollment**gidin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="9ca85-129">MDM kullanıcı kapsamının etkin olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="9ca85-130">Tüm bilgisayarları kaydetmek için, kullanıcılar Windows'a bir iş hesabı eklediğinde Azure AD'ye katılan tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydetmek için **Tümü'ne** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="9ca85-131">Belirli bir kullanıcı grubunun bilgisayarlarını kaydetmek için **Bazıları'na** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="9ca85-132">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="9ca85-133">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="9ca85-134">4. Gerekli kaynakları oluşturma</span><span class="sxs-lookup"><span data-stu-id="9ca85-134">4. Create the required resources</span></span> 

<span data-ttu-id="9ca85-135">[Karma Azure AD birleştirmeyapılandırmak](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) için gerekli görevlerin yerine getirilmesi, [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'inin kullanımı yla basitleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="9ca85-135">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="9ca85-136">Bu cmdlet'i çağırdığınızda, gerekli servis bağlantı noktası ve grup ilkesini oluşturur ve yapılandıracaktır.</span><span class="sxs-lookup"><span data-stu-id="9ca85-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="9ca85-137">PowerShell örneğinden aşağıdakileri çağırarak bu modülü yükleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="9ca85-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="9ca85-138">Bu modülü Azure AD Connect çalıştıran Windows Server'a yüklemeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="9ca85-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="9ca85-139">Gerekli servis bağlantı noktası ve grup ilkesini oluşturmak için [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırırsınız.</span><span class="sxs-lookup"><span data-stu-id="9ca85-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="9ca85-140">Bu görevi yerine getirirken Microsoft 365 Business Premium global yönetici kimlik bilgilerinize ihtiyacınız olacaktır.</span><span class="sxs-lookup"><span data-stu-id="9ca85-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="9ca85-141">Kaynakları oluşturmaya hazır olduğunuzda aşağıdakileri çağırın:</span><span class="sxs-lookup"><span data-stu-id="9ca85-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="9ca85-142">İlk komut Microsoft bulutuyla bir bağlantı kurar ve sizden istendiğinde Microsoft 365 Business Premium global yönetici kimlik bilgilerinizi belirtin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="9ca85-143">5. Grup İlkesini Bağla</span><span class="sxs-lookup"><span data-stu-id="9ca85-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="9ca85-144">Grup İlkesi Yönetim Konsolu'nda (GPMC), politikayı bağlamak istediğiniz konuma sağ tıklayın ve bağlam menüsünden *varolan bir GPO'yu bağlayın...* seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="9ca85-145">Yukarıdaki adımda oluşturulan ilkeyi seçin ve **ardından Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="9ca85-146">En son Yönetim Şablonlarını Alın</span><span class="sxs-lookup"><span data-stu-id="9ca85-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="9ca85-147">**Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bunun nedeni Windows 10, sürüm 1803, sürüm 1809 veya sürüm 1903 için ADMX yüklü değil.</span><span class="sxs-lookup"><span data-stu-id="9ca85-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="9ca85-148">Sorunu gidermek için aşağıdaki adımları izleyin (Not: en son MDM.admx geriye dönük uyumludur):</span><span class="sxs-lookup"><span data-stu-id="9ca85-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="9ca85-149">Indirin: [Windows 10 Mayıs 2019 Güncelleştirmesi (1903) için Yönetim Şablonları (.admx)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="9ca85-149">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="9ca85-150">Paketi Birincil Etki Alanı Denetleyicisi'ne (PDC) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-150">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="9ca85-151">Klasöre sürülmeye bağlı olarak gidin: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 Mayıs 2019 Güncelleştirmesi (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="9ca85-151">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="9ca85-152">**İlke** **Tanımları** klasörünü yukarıdaki yolda Yeniden adlandırın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="9ca85-153">**İlke Tanımlar** klasörünü **C:\Windows\SYSVOL\domain\İlkeler'e**kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-153">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="9ca85-154">Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, PolicyDefinitions'ın içeriğini oraya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="9ca85-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="9ca85-155">İlkenin kullanılabilir olması için Birincil Etki Alanı Denetleyicisini yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="9ca85-155">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="9ca85-156">Bu yordam, gelecekteki herhangi bir sürüm için de çalışacaktır.</span><span class="sxs-lookup"><span data-stu-id="9ca85-156">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="9ca85-157">Bu noktada, kullanılabilir varsayılan Azure **REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir** ilkesini görebilmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="9ca85-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
