---
title: Microsoft 365 Business'ı kurulum sihirbazını kullanarak ayarlama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Dört adımları izleyerek Microsoft 365 iş kurmayı öğrenin.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982200"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="9e18e-103">Microsoft 365 Business'ı kurulum sihirbazını kullanarak ayarlama</span><span class="sxs-lookup"><span data-stu-id="9e18e-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="9e18e-104">1-4 aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="9e18e-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="9e18e-105">Microsoft 365 İş'i ayarlama</span><span class="sxs-lookup"><span data-stu-id="9e18e-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="9e18e-106">Microsoft 365 iş yerinde Active Directory olmadığında ayarlanması hakkında bir video izleyin:</span><span class="sxs-lookup"><span data-stu-id="9e18e-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="9e18e-p101">Bilgi içeren Active Directory yerel kurulumları için kurulum adımları içerir. Etki alanına katılmış bir aygıtlar erişmeye devam etmek istiyorsanız, iki farklı şekilde, etkinleştirme için aşağıdaki makaleleri okuyun ve Kurulum Sihirbazı'nı çalıştırmadan önce adımları tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="9e18e-p101">The set-up steps include information for setups that include local Active Directory. If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="9e18e-109">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="9e18e-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="9e18e-110">-Bu, önerilen yoldur.</span><span class="sxs-lookup"><span data-stu-id="9e18e-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="9e18e-111">Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları</span><span class="sxs-lookup"><span data-stu-id="9e18e-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="9e18e-112">Adım 1: kayıt kişiselleştirin</span><span class="sxs-lookup"><span data-stu-id="9e18e-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="9e18e-p102">Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Business](https://portal.microsoft.com)'da oturum açın. Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="9e18e-115">Sihirbazı başlatmak için yönetim merkezinde **Kuruluma başla**'yı seçin (durumunuza bağlı olarak bunun yerine **Kuruluma devam et** ifadesini de görebilirsiniz).</span><span class="sxs-lookup"><span data-stu-id="9e18e-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="9e18e-116">Kullanmak istediğiniz etki alanı adını (contoso.com gibi) girin.</span><span class="sxs-lookup"><span data-stu-id="9e18e-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="9e18e-p103">Devam edin ve Azure AD bağlan, örneğin kullanırken doğruladıktan bile, etki alanınızı girin. Etki alanınızın doğrulamak için Azure AD Connect kullandıysanız aşağıdaki iki adımı sizin için geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p103">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example. The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="9e18e-119">Doğrulayan etki alanı sahibi [herhangi bir DNS barındırma sağlayıcı için Office 365 oluşturmak DNS kayıtları](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) için sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="9e18e-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="9e18e-p104">Bir örnek video görüntüleyebilirsiniz [Video: Yeni Yönetim Merkezi'ndeki Kurulum Office 365](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Not Bu video 365 iş Microsoft veri koruma adımları içermez.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p104">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="9e18e-123">Adım 2: kullanıcı eklemek ve lisansları atama</span><span class="sxs-lookup"><span data-stu-id="9e18e-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="9e18e-124">Kullanıcıları şimdi burada ekleyebilirsiniz veya yönetim merkezinde [kullanıcıları daha sonra da ekleyebilirsiniz](add-users-m365b.md).</span><span class="sxs-lookup"><span data-stu-id="9e18e-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="9e18e-125">Eklediğiniz tüm kullanıcılara otomatik olarak Microsoft 365 İş lisansı atanır.</span><span class="sxs-lookup"><span data-stu-id="9e18e-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="9e18e-p105">Microsoft 365 İş aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect kullandıysanız), bu kullanıcılara hemen lisans atamanızı sağlayan bir seçenek görürsünüz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="9e18e-p106">Ayrıca kimlik bilgilerini, eklediğiniz yeni kullanıcılarla paylaşmak için bir seçenek de görürsünüz. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="9e18e-130">E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="9e18e-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="9e18e-131">Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9e18e-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="9e18e-133">Adım 3: etki alanınızı Bağlan</span><span class="sxs-lookup"><span data-stu-id="9e18e-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="9e18e-134">.Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Bağlan kullanılır, bu adımı göremez.</span><span class="sxs-lookup"><span data-stu-id="9e18e-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="9e18e-135">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="9e18e-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="9e18e-p107">Kurulum Sihirbazı'nı genellikle, kaydedici algılar ve bağlantıyı registrar Web sitesinde, NS kayıtları güncelleştirmek için adım adım yönergeler sağlar. Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="9e18e-p107">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website. If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="9e18e-138">E-posta ve diğer hizmetler sizin için ayarlanır</span><span class="sxs-lookup"><span data-stu-id="9e18e-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="9e18e-139">Adım 4: aygıtları yönetme ve dosyaları çalışma</span><span class="sxs-lookup"><span data-stu-id="9e18e-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="9e18e-p108">**Koruma çalışma dosyaları taşınabilir aygıtlarınızda** sayfasında hem **aygıtları kaybolur veya çalınırsa, koruma çalışma dosyaları** ve ayarları **kullanıcıların mobil cihazlarda Office dosyalarının nasıl eriştiğini yönetme** **üzerinde**ayarlayın. Her her ayarın yanındaki köşeli çift tıklatarak alt ayar da erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p108">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**. You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="9e18e-142">Tüm lisanslı kullanıcılarınızın çalışma dosyaları şimdi IOS ve Android aygıtlarda, bunlar en erken korunan [Office uygulamaları yükleyin](set-up-mobile-devices.md) (ve bunların Microsoft 365 iş kimlik bilgileriyle kimlik doğrulaması).</span><span class="sxs-lookup"><span data-stu-id="9e18e-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="9e18e-144">**Set Windows 10 aygıt yapılandırması** sayfasında, **Güvenli Windows 10 aygıtları** **üzerinde**ayarı.</span><span class="sxs-lookup"><span data-stu-id="9e18e-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="9e18e-145">Her yanındaki köşeli çift ayraç tıklatarak alt ayar da erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9e18e-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="9e18e-p109">Kullanıcılarınızın tümü Windows 10 bilgisayarlar varsa ve varolan hiçbir Office yükler **Evet** veya Tıklat-Çalıştır Office yüklemeleri için **Office 10 aygıtlarda Windows yükleme** ayarını belirleyin. Durum bu değilse, bu seçenek **Hayır**olarak ayarlayın. Kullanıcı bilgisayarlarında hazırladıktan sonra Yönetim Merkezi'nden daha sonra [otomatik olarak Office yüklemek](auto-install-or-uninstall-office.md) olabilir. Yönergeler için bkz: [Office İstemcisi yüklemesine hazırlamak](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="9e18e-p109">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs. If this is not the case, set this option to **No**. You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers. For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="9e18e-150">Lisanslı kullanıcıları çalışma dosyalarını Windows 10 aygıtlarda hemen bunlar öngörülen 365 Microsoft Business Azure AD etki alanı veya aynı anda Microsoft 365 katılma sırasında [Windows 10 yeni bir bilgisayara yüklemek](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) için [Windows 10 aygıtları katılın](set-up-windows-devices.md) İş Azure AD etki alanı.</span><span class="sxs-lookup"><span data-stu-id="9e18e-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="9e18e-151">**İleri** ' yi tıklatın ve kurulum ile yapılır.</span><span class="sxs-lookup"><span data-stu-id="9e18e-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="9e18e-152">Lütfen bize görüşlerinizi deneyimini geliştirmemize yardımcı olmak üzere, bu adımı bırakın.</span><span class="sxs-lookup"><span data-stu-id="9e18e-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="9e18e-154">Ek güvenlik ayarları</span><span class="sxs-lookup"><span data-stu-id="9e18e-154">Additional security settings</span></span>

<span data-ttu-id="9e18e-155">Güvenlik ve Kurulum Sihirbazı'ndaki Uyumluluk ayarına ek olarak, aşağıdaki ek ayarlar de ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="9e18e-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="9e18e-p110">Güvenli olmayan ekleri karşı koruma ayarlayın. **Gelişmiş tehdit koruması** (ATP), kötü amaçlı içerik tanımlar ve balık avlama ve ransomware bulaşmalarını karşı korunmasına yardımcı olma teslim güvenli olmayan ekleri engeller. Eki korumasını etkinleştirmek için bkz: [Office 365 KM güvenli ekler ilkelerini kurun](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="9e18e-p110">Set up protection against unsafe attachments. **Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections. To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="9e18e-p111">Kullanıcılar kötü niyetli bağlantıları tıklattığınızda ortamınızı korumak. ATP bunları kullanıcının tıklattığı zaman e-posta içindeki bağlantıları inceler. Bağlantı güvenli ise, kullanıcı siteyi ziyaret değil bir uyarı veya sitesinde engellenmiş haberdar. Bu balık avlama karşı korunmasına yardımcı olur. [Office 365 KM güvenli bağlantıları ilkelerini kurun](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) veya [Office 365 KM güvenli bağlantıları ilkelerini kurun](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="9e18e-p111">Protect your environment when users click malicious links. ATP examines links in email at the time a user clicks them. If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked. This helps protect against phishing schemes. [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="9e18e-p112">Bir kullanıcının tüm posta **tutun dava**üzerinde koyarak silinmiş öğeleri de dahil olmak üzere tüm posta kutusu içeriği koruyabilirsiniz. Yönergeler için bkz.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p112">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**. For instructions, see</span></span> 
- <span data-ttu-id="9e18e-166">[E-posta bekletme çevrimiçi Exchange arşivleme ile ayarlayın](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="9e18e-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="9e18e-p113">Örneğin, özelleştirilmiş **bekletme ilkeleri**, belirli bir süre korumak veya içeriği saklama dönemi sonunda kalıcı olarak silmek için ayarlayın. Menkul kıymetler ve uyumluluk Merkezi'nde, **veri yönetim** için gidin özelleştirilmiş bekletme ilkeleri etkinleştirebilirsiniz \> **bekletme**ve sonra sihirbazdaki adımları izleyin. Daha fazla bilgi için [Bekletme İlkeleri'ne genel bakış](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="9e18e-p113">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period. You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard. To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="9e18e-170">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="9e18e-170">Next steps</span></span>

<span data-ttu-id="9e18e-171">Kendi lisansı olan kullanıcılar için aygıtlarını kurabileceğiniz sonraki adımdır.</span><span class="sxs-lookup"><span data-stu-id="9e18e-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="9e18e-172">Bkz: [Microsoft 365 iş kullanıcıları için Windows aygıtları kurmak](set-up-windows-devices.md) ve [mobil aygıtlar Microsoft 365 iş kullanıcıları için ayarlayın](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="9e18e-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="9e18e-173">[Microsoft 365 iş yönetme](manage.md) ilkeleri aygıt ve uygulama koruması nasıl konulara bağlantılar için bkz: ve nasıl kullanıcı aygıtlardan verileri kaldırmak.</span><span class="sxs-lookup"><span data-stu-id="9e18e-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  


