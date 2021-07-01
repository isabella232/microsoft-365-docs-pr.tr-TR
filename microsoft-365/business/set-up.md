---
title: Ayarlama Microsoft 365 İş Ekstra
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Etki alanı ve kullanıcı ekleme Microsoft 365 İş Ekstra, güvenlik ilkelerini ayarlama ve daha fazlası için kurulum adımlarını keşfedin.
ms.openlocfilehash: 74a98e915577cf86ec32a706bd3b8f558f49db95
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227649"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="e4ad7-103">Kurulum Microsoft 365 İş Ekstra ayarları</span><span class="sxs-lookup"><span data-stu-id="e4ad7-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

## <a name="watch-overview-of-microsoft-365-setup"></a><span data-ttu-id="e4ad7-104">İzle: Kuruluma genel Microsoft 365 görünümü</span><span class="sxs-lookup"><span data-stu-id="e4ad7-104">Watch: Overview of Microsoft 365 setup</span></span>

<span data-ttu-id="e4ad7-105">Kurulumla ilgili genel bir bakış için bu Microsoft 365 İş Ekstra izleyin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-105">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="e4ad7-106">Etki alanınızı ve kullanıcıları ekleme ve ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="e4ad7-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="e4ad7-107">E-Microsoft 365 İş Ekstra satın alırken, sahip olduğunuz bir etki alanını kullanma veya kayıt sırasında bir etki alanı [satın alma seçeneğiniz vardır.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="e4ad7-108">Kayıt olurken yeni bir etki alanı satın aldısanız, etki alanınız ayarlanır ve Kullanıcı ekleme ve lisans atama ['ya geçebilirsiniz.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="e4ad7-109">Oturum açmanızı kişiselleştirmek için etki alanınızı ekleme</span><span class="sxs-lookup"><span data-stu-id="e4ad7-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="e4ad7-110">Genel yönetici [Microsoft 365 yönetim merkezi](https://admin.microsoft.com) kullanarak e-posta oturum açma.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="e4ad7-111">Sihirbazı **başlatmak için Kuruluma** git'i seçin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Kuruluma git'i seçin.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="e4ad7-113">Office **uygulamalarınızı** yükleyin sayfasında, isteğe bağlı olarak uygulamaları kendi bilgisayarınıza yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="e4ad7-114">Etki alanı **ekle adımını,** kullanmak istediğiniz etki alanı adını girin (örneğin, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e4ad7-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="e4ad7-115">Kayıt sırasında etki alanı satın yaptıysanız, burada Etki alanı adımı **ekle'yi** görmeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="e4ad7-116">Bunun yerine Kullanıcı [ekle'ye](#add-users-and-assign-licenses) gidin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Oturum açmanızı kişiselleştirin sayfasının ekran görüntüsü.](../media/adddomain.png)

    
4. <span data-ttu-id="e4ad7-118">Etki alanının size ait olduğunu doğru yapan herhangi bir DNS barındırma [sağlayıcısında DNS](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) Microsoft 365 için sihirbazda yer alan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="e4ad7-119">Etki alanı barındırmanızı biliyorsanız, bkz. Etki [alanına etki alanı Microsoft 365.](/microsoft-365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-119">If you know your domain host, see also [Add a domain to Microsoft 365](/microsoft-365/admin/setup/add-domain).</span></span>

    <span data-ttu-id="e4ad7-120">Barındırma sağlayıcınız GoDaddy veya etki alanı bağlantısı özelliği etkinleştirilmiş başka bir ana bilgisayarsa [işlem](/office365/admin/get-help-with-domains/domain-connect)kolaydır ve otomatik olarak oturum açmalı ve Microsoft'un sizin adına kimlik doğrulamasına izin vermelisiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![GoDaddy Erişimi Onayla sayfasında Yetkilendir'i seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="e4ad7-122">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="e4ad7-122">Add users and assign licenses</span></span>

<span data-ttu-id="e4ad7-123">Sihirbaza kullanıcı eklemekle birlikte, kullanıcıları daha sonra [yönetim merkezinden](../admin/add-users/add-users.md) de ebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-123">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="e4ad7-124">Buna ek olarak, yerel bir etki alanı denetleyicisiniz varsa Azure AD etki alanı denetleyicisi [olan kullanıcıları Bağlan.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="e4ad7-125">Sihirbaza kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="e4ad7-125">Add users in the wizard</span></span>

<span data-ttu-id="e4ad7-126">Sihirbaza ekley istediğiniz kullanıcılara otomatik olarak lisans Microsoft 365 İş Ekstra atanır.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Sihirbazda Yeni kullanıcı ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. <span data-ttu-id="e4ad7-128">Microsoft 365 İş Ekstra aboneliğinizin mevcut kullanıcıları varsa (örneğin, Azure AD Bağlan kullandıysanız), bu kullanıcılara şimdi lisans atama seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="e4ad7-129">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="e4ad7-130">Kullanıcıları ekledikten sonra, kimlik bilgilerini kendi ekledikten sonra yeni kullanıcılarla paylaşma seçeneği de elde olur.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="e4ad7-131">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="e4ad7-132">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="e4ad7-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="e4ad7-133">Kullanıcıları ayarlamak için .onmicrosoft etki alanını veya Azure AD Bağlan'i kullandıysanız bu adımı görmeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="e4ad7-134">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="e4ad7-135">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="e4ad7-136">Bunu yoksa, herhangi bir etki alanı kayıt şirketiyle Microsoft 365 [ad sunucularını değiştirebilirsiniz.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="e4ad7-137">Mevcut DNS kayıtlarınız, örneğin var olan bir web siteniz [](/office365/admin/get-help-with-domains/domain-connect)varsa, ancak DNS barındırma etki alanı bağlantısı için etkinleştirilmişse, Kayıtları benim için **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="e4ad7-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="e4ad7-138">Çevrimiçi **hizmetlerinizi seçin sayfasında,** tüm varsayılanları kabul edin ve  Sonraki 'yi seçin ve DNS barındırma hizmet barındırması sayfasında Yetkilendir'i seçin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="e4ad7-139">Diğer DNS ana bilgisayarlarında mevcut DNS kayıtlarınız varsa (etki alanı bağlantısı için etkin değil), var olan hizmetlerin bağlı kalacağından emin olmak için kendi DNS kayıtlarınızı yönetmek istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="e4ad7-140">Daha [fazla bilgi için etki alanı](/office365/admin/get-help-with-domains/dns-basics) temel bilgilerine bakın.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-140">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Kayıtları etkinleştirme sayfası.](../media/activaterecords.png)

2. <span data-ttu-id="e4ad7-142">Sihirbazda adımları izleyin; sizin için e-posta ve diğer hizmetler ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="e4ad7-143">Organizasyonlarınızı koruma</span><span class="sxs-lookup"><span data-stu-id="e4ad7-143">Protect your organization</span></span> 

<span data-ttu-id="e4ad7-144">Sihirbazda ayar ilkeleri, Tüm Kullanıcılar adında bir [Güvenlik grubuna otomatik](/office365/admin/create-groups/compare-groups#security-groups) olarak *uygulanır.*</span><span class="sxs-lookup"><span data-stu-id="e4ad7-144">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="e4ad7-145">Ayrıca, yönetim merkezinde ilke atamak için ek gruplar da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="e4ad7-146">Gelişmiş **siber tehditlere karşı** korumayı artır ' ise Tehdit Koruması'nın, Office 365 uygulamalarına yönelik dosyaları ve bağlantıları taramasına izin verme varsayılanlarını kabul Office önerilir. [](../security/office-365-security/defender-for-office-365.md)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Korumayı artır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. <span data-ttu-id="e4ad7-148">Hassas veri **sızıntılarını** önle sayfasında, Office uygulamaları içinde hassas verileri izlemek ve bunların yanlışlıkla kuruluş dışında paylaşımını önlemek için Office 365 Veri Kaybı Önleme 'i (DLP) açmak için varsayılanları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="e4ad7-149">Mobil cihazlar **için Office** sayfasında, mobil uygulama yönetimini açık bırakın, ayarları genişletin ve gözden geçirin ve ardından Mobil uygulama yönetimi ilkesi oluştur **öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="e4ad7-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Mobil için Mobil cihazlar sayfasındaki Office ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="e4ad7-151">Bilgisayarlarda Windows 10 sağlama</span><span class="sxs-lookup"><span data-stu-id="e4ad7-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="e4ad7-152">Sol gezintide Kurulum'u **seçin** ve oturum açma ve güvenlik altında Bilgisayarlarınızı güvende Windows 10 **seçin.**</span><span class="sxs-lookup"><span data-stu-id="e4ad7-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="e4ad7-153">Çalışmaya **başlamak için** Görüntüle'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-153">Choose **View** to get started.</span></span> <span data-ttu-id="e4ad7-154">Tüm [yönergeler için Windows 10 bilgisayarlarınızı](secure-win-10-pcs.md) güvenlik altına almak için bkz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="e4ad7-155">Office 365 istemci uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="e4ad7-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="e4ad7-156">Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiysanız, kullanıcılar Windows cihazlarından Azure AD'de iş kimlik bilgileriyle oturum attıktan sonra uygulamalar Windows 10 cihazlarına yüklenir.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="e4ad7-157">Mobil iOS Office Android cihazlarına kullanıcı yüklemek için bkz. Mobil [cihazları Microsoft 365 İş Ekstra ayarlama](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="e4ad7-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="e4ad7-158">Ayrıca e-Office yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-158">You can also install Office individually.</span></span> <span data-ttu-id="e4ad7-159">Yönergeler [için Office PC veya Mac bilgisayara yükleme](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) hakkında bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="e4ad7-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="related-content"></a><span data-ttu-id="e4ad7-160">İlgili içerik</span><span class="sxs-lookup"><span data-stu-id="e4ad7-160">Related content</span></span>

<span data-ttu-id="e4ad7-161">[Microsoft 365 eğitim videoları için giriş](../business-video/index.yml) (bağlantı sayfası)</span><span class="sxs-lookup"><span data-stu-id="e4ad7-161">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
