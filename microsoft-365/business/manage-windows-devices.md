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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564963"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="a3d59-103">Etki alanına bağlı Windows 10 cihazlarının Microsoft 365 Business Premium tarafından yönetilmesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="a3d59-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a3d59-104">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a3d59-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="a3d59-105">Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a3d59-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="a3d59-106">Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="a3d59-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="a3d59-107">Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacağına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="a3d59-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="a3d59-108">Başlamadan önce şu adımları tamamladığınızdan emin olun:</span><span class="sxs-lookup"><span data-stu-id="a3d59-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="a3d59-109">Azure AD Connect ile kullanıcıları Azure AD ile senkronize edin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="a3d59-110">Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="a3d59-111">Eşitlediğiniz tüm etki alanı kullanıcılarının Microsoft 365 Business Premium lisansına sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a3d59-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a3d59-112">Bkz. Adımlar için [etki alanı kullanıcılarını Microsoft'a senkronize edin.](manage-domain-users.md)</span><span class="sxs-lookup"><span data-stu-id="a3d59-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="a3d59-113">1. Intune MDM Yetki doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a3d59-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="a3d59-114">portal.azure.com gidin ve Intune için sayfa arama üst kısmında.</span><span class="sxs-lookup"><span data-stu-id="a3d59-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="a3d59-115">Microsoft Intune sayfasında Cihaz **kaydını** seçin ve **Genel Bakış** sayfasında **MDM yetkilisinin** **Intune**olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="a3d59-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="a3d59-116">**MDM yetkisi** **Yok**ise, **Intune**ayarlamak için **MDM yetkisini** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="a3d59-117">**MDM yetkisi** **Microsoft Office 365**ise, **Aygıtlar**Kayıt  >  **aygıtlarına** gidin ve **Intune MDM** yetkilisi ekleme hakkını sağdaki **MDM yetki** ekle iletişim kutusunu kullanın **(MDM Yetkilisi Ekle** iletişim kutusu yalnızca **MDM Yetkilisi** Microsoft Office 365'e ayarlanırsa kullanılabilir).</span><span class="sxs-lookup"><span data-stu-id="a3d59-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="a3d59-118">2. Bilgisayarlara katılmak için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a3d59-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="a3d59-119">Yönetici merkezleri listesinde yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve Azure **Active Directory'yi** seçin (Azure **Admin centers** Etkin Dizini görünmüyorsa tümünü göster'i seçin).</span><span class="sxs-lookup"><span data-stu-id="a3d59-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="a3d59-120">Azure **Etkin Dizin yönetici merkezinde,** **Azure Etkin Dizin'e** gidin, **Aygıtlar'ı** seçin ve ardından **Aygıt ayarlarını seçin.**</span><span class="sxs-lookup"><span data-stu-id="a3d59-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="a3d59-121">**Kullanıcıların Azure AD'de aygıtlara katılıp katılamayada** olabileceğini doğrulayın etkin</span><span class="sxs-lookup"><span data-stu-id="a3d59-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="a3d59-122">Tüm kullanıcıları etkinleştirmek için **Tümü'ne**ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="a3d59-123">Belirli kullanıcıları etkinleştirmek için, belirli bir kullanıcı grubunu etkinleştirmek için **Seçili** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="a3d59-124">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="a3d59-125">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="a3d59-126">3. MDM için Azure AD'nin etkinleştirildiğinden doğrulayın</span><span class="sxs-lookup"><span data-stu-id="a3d59-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="a3d59-127">Yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve **Endpoint Managemen**t'yi seçin **(Endpoint Manager** görünmüyorsa **tümünü göster'i** seçin)</span><span class="sxs-lookup"><span data-stu-id="a3d59-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="a3d59-128">Microsoft **Endpoint Manager yönetici merkezinde,** **Windows**Windows Kayıt Otomatik Kayıt Cihazlar  >  **Windows**  >  **Windows Enrollment**  >  **Automatic Enrollment**gidin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="a3d59-129">MDM kullanıcı kapsamının etkin olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="a3d59-130">Tüm bilgisayarları kaydetmek için, kullanıcılar Windows'a bir iş hesabı eklediğinde Azure AD'ye katılan tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydetmek için **Tümü'ne** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="a3d59-131">Belirli bir kullanıcı grubunun bilgisayarlarını kaydetmek için **Bazıları'na** ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="a3d59-132">Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="a3d59-133">Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="a3d59-134">4. Servis bağlantı noktasını (SCP) ayarlama</span><span class="sxs-lookup"><span data-stu-id="a3d59-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="a3d59-135">Bu [adımlar, karma azure AD birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)yapılandırmabasitleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="a3d59-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="a3d59-136">Adımları tamamlamak için Azure AD Connect'i ve Microsoft 365 Business Premium global yöneticinizi ve Active Directory yönetici parolalarınızı kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a3d59-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="a3d59-137">Azure AD Connect'i başlatın ve sonra **Yapıla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="a3d59-138">Ek **görevler** sayfasında, **aygıtı yapılandır'ı**seçin ve **sonra İleri'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="a3d59-139">Genel **Bakış** sayfasında **İleri'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="a3d59-140">**Azure'a Bağlan AD** sayfasında, Microsoft 365 Business Premium için global bir yöneticinin kimlik bilgilerini girin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="a3d59-141">Aygıt **seçenekleri** sayfasında, **Karma Azure AD birleştirme'yi yapılandır'ı**ve **ardından İleri'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="a3d59-142">**SCP** sayfasında, Azure AD Connect'in SCP'yi yapılandırmasını istediğiniz her orman için aşağıdaki adımları tamamlayın ve **sonra İleri'yi**seçin:</span><span class="sxs-lookup"><span data-stu-id="a3d59-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="a3d59-143">Orman adının yanındaki kutuyu işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-143">Check the box beside the forest name.</span></span> <span data-ttu-id="a3d59-144">Orman, AD alan adınız olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="a3d59-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="a3d59-145">Kimlik **Doğrulama Hizmeti** sütununda açılır dosyayı açın ve eşleşen etki alanı adını seçin (yalnızca tek bir seçenek olmalıdır).</span><span class="sxs-lookup"><span data-stu-id="a3d59-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="a3d59-146">Etki alanı yöneticisi kimlik bilgilerini girmek için **Ekle'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="a3d59-147">Aygıt **işletim sistemleri** sayfasında yalnızca Windows 10 veya daha sonraki etki alanına bağlı aygıtları seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="a3d59-148">**Yapılandırmaya Hazır** **sayfasında, Yapılandırma'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="a3d59-149">Yapılandırma **tam** **sayfasında, Exit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="a3d59-150">5. Intune Kayıt için bir GPO oluşturma – ADMX yöntemi</span><span class="sxs-lookup"><span data-stu-id="a3d59-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="a3d59-151">Kullanın. ADMX şablon dosyası.</span><span class="sxs-lookup"><span data-stu-id="a3d59-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="a3d59-152">AD sunucusunda oturum açın, **Sunucu Yöneticisi**  >  **Araçları**Grup  >  **İlkesi Yönetimi'ni**arayın ve açın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="a3d59-153">**Etki Alanları** altında etki alanı adınızı seçin ve **Yeni'yi**seçmek için **Grup İlkesi Nesneleri'ni** sağ tıklatın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="a3d59-154">Yeni GPO'ya bir ad verin, örneğin "*Cloud_Enrollment*" ve sonra **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="a3d59-155">**Grup İlkesi Nesneleri** altındaki yeni GPO'ya sağ tıklayın ve **Edit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="a3d59-156">Grup **İlkesi Yönetimi**Düzenleyicisi'nde, **Bilgisayar Yapılandırma**  >  **İlkeleri**  >  **Yönetim Şablonları**Windows  >  **Components**  >  **MDM'ye**gidin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="a3d59-157">**Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir'e** sağ tıklatın ve ardından Etkin **Enabled**  >  **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="a3d59-158">Editör penceresini kapatın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a3d59-159">**Varsayılan Azure REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bkz. [Get the latest Administrative Templates](#get-the-latest-administrative-templates)</span><span class="sxs-lookup"><span data-stu-id="a3d59-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="a3d59-160">6. Grup İlkesini Dağıtmak</span><span class="sxs-lookup"><span data-stu-id="a3d59-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="a3d59-161">Sunucu Yöneticisi'nde, **Etki Alanları** > Grup İlkesi nesneleri altında, "Cloud_Enrollment" gibi yukarıdaki Adım 3'ten GPO'yu seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="a3d59-162">GPO'nuz için **Kapsam** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="a3d59-163">GPO'nun Kapsam sekmesinde, **Linkler**altındaki etki alanına bağlantısağ tıklayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="a3d59-164">GPO'yu dağıtmak için **Zorla'yı** seçin ve onay ekranında **Tamam'ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="a3d59-165">En son Yönetim Şablonlarını Alın</span><span class="sxs-lookup"><span data-stu-id="a3d59-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="a3d59-166">**Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bunun nedeni Windows 10, sürüm 1803, sürüm 1809 veya sürüm 1903 için ADMX yüklü değil.</span><span class="sxs-lookup"><span data-stu-id="a3d59-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="a3d59-167">Sorunu gidermek için aşağıdaki adımları izleyin (Not: en son MDM.admx geriye dönük uyumludur):</span><span class="sxs-lookup"><span data-stu-id="a3d59-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="a3d59-168">Indirin: [Windows 10 Mayıs 2019 Güncelleştirmesi (1903) için Yönetim Şablonları (.admx)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="a3d59-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="a3d59-169">Paketi Birincil Etki Alanı Denetleyicisi'ne (PDC) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="a3d59-170">Klasöre sürülmeye bağlı olarak gidin: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 Mayıs 2019 Güncelleştirmesi (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="a3d59-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="a3d59-171">**İlke** **Tanımları** klasörünü yukarıdaki yolda Yeniden adlandırın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="a3d59-172">**İlke Tanımlar** klasörünü **C:\Windows\SYSVOL\domain\İlkeler'e**kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="a3d59-173">Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, PolicyDefinitions'ın içeriğini oraya ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a3d59-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="a3d59-174">İlkenin kullanılabilir olması için Birincil Etki Alanı Denetleyicisini yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="a3d59-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="a3d59-175">Bu yordam, gelecekteki herhangi bir sürüm için de çalışacaktır.</span><span class="sxs-lookup"><span data-stu-id="a3d59-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="a3d59-176">Bu noktada, kullanılabilir varsayılan Azure **REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir** ilkesini görebilmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="a3d59-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

