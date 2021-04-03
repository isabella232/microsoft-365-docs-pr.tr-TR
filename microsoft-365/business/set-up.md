---
title: Microsoft 365 İş Ekstra'ya ayarlama
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
description: Etki alanı ve kullanıcı ekleme, güvenlik ilkelerini ayarlama ve daha fazlası gibi Microsoft 365 İş Ekstra kurulum adımlarını keşfedin.
ms.openlocfilehash: c8e2ca94f4947d4f9c69915d2fef410a6075bfed
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579924"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="db2de-103">Kurulum sihirbazında Microsoft 365 İş Ekstra'ya ayarlama</span><span class="sxs-lookup"><span data-stu-id="db2de-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="db2de-104">Microsoft 365 İş Ekstra kurulumuna genel bakış için bu videoyu izleyin.</span><span class="sxs-lookup"><span data-stu-id="db2de-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="db2de-105">Etki alanınızı, kullanıcılarınızı ekleme ve ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="db2de-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="db2de-106">Microsoft 365 İş Ekstra'ı satın alırken, sahip olduğunuz bir etki alanını kullanma veya kayıt sırasında bir etki alanı [satın alma seçeneğiniz vardır.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="db2de-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="db2de-107">Kayıt olurken yeni bir etki alanı satın aldıysanız, etki alanınız ayarlanmıştır ve Kullanıcı ekle'ye geçebilirsiniz [ve lisans atabilirsiniz.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="db2de-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="db2de-108">Oturum açmanızı kişiselleştirmek için etki alanınızı ekleme</span><span class="sxs-lookup"><span data-stu-id="db2de-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="db2de-109">Genel yönetici [kimlik bilgilerinizi kullanarak Microsoft 365](https://admin.microsoft.com) yönetim merkezinde oturum açma.</span><span class="sxs-lookup"><span data-stu-id="db2de-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="db2de-110">Sihirbazı **başlatmak için Kuruluma** git'i seçin.</span><span class="sxs-lookup"><span data-stu-id="db2de-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Kuruluma git'i seçin.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="db2de-112">Office **uygulamalarınızı yükleyin sayfasında,** isteğe bağlı olarak uygulamaları kendi bilgisayarınıza yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="db2de-113">Etki alanı **ekle adımlarında,** kullanmak istediğiniz etki alanı adını girin (örneğin, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="db2de-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="db2de-114">Kayıt sırasında bir etki alanı satın yaptıysanız, Buraya etki alanı ekle **adımını** görmeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="db2de-115">Bunun yerine [Kullanıcı ekle'ye](#add-users-and-assign-licenses) gidin.</span><span class="sxs-lookup"><span data-stu-id="db2de-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Oturum açma sayfanızı kişiselleştirin sayfasının ekran görüntüsü.](../media/adddomain.png)

    
4. <span data-ttu-id="db2de-117">[Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) için etki alanının sahibinizi doğrulayanın herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için sihirbazda yer alan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="db2de-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="db2de-118">Etki alanı ana nızı biliyorsanız, ana bilgisayarla ilgili [yönergelere de bakın.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="db2de-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="db2de-119">Barındırma sağlayıcınız GoDaddy veya etki alanı [](/office365/admin/get-help-with-domains/domain-connect)bağlantısıyla etkinleştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmalı ve Sizin adınıza Microsoft'un kimlik doğrulamasına izin vermeniz istenmektedir.</span><span class="sxs-lookup"><span data-stu-id="db2de-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![GoDaddy Erişimi Onayla sayfasında Yetkilendir'i seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="db2de-121">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="db2de-121">Add users and assign licenses</span></span>

<span data-ttu-id="db2de-122">Sihirbaza kullanıcı eklemekle birlikte, kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de eklemeniz de gerekir.</span><span class="sxs-lookup"><span data-stu-id="db2de-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="db2de-123">Buna ek olarak, yerel bir etki alanı denetleyiciniz [varsa, Azure AD Connect'i olan kullanıcıları ekleyebilirsiniz.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="db2de-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="db2de-124">Sihirbaza kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="db2de-124">Add users in the wizard</span></span>

<span data-ttu-id="db2de-125">Sihirbaza ekley istediğiniz kullanıcılara otomatik olarak bir Microsoft 365 İş Ekstra lisansı atanır.</span><span class="sxs-lookup"><span data-stu-id="db2de-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Sihirbazda Yeni kullanıcı ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. <span data-ttu-id="db2de-127">Microsoft 365 İş Ekstra aboneliğinizin mevcut kullanıcıları varsa (örneğin, Azure AD Connect kullandınız), bu kullanıcılara şimdi lisans atama seçeneğiniz olur.</span><span class="sxs-lookup"><span data-stu-id="db2de-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="db2de-128">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="db2de-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="db2de-129">Kullanıcıları ekledikten sonra, kimlik bilgilerini kendi ekledikten sonra yeni kullanıcılarla paylaşma seçeneği de elde olur.</span><span class="sxs-lookup"><span data-stu-id="db2de-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="db2de-130">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="db2de-131">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="db2de-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="db2de-132">Kullanıcıları ayarlamak için .onmicrosoft etki alanını kullanmayı seçtiy veya Azure AD Connect'i kullandınız, bu adımı görmeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="db2de-133">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="db2de-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="db2de-134">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="db2de-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="db2de-135">Bunu bilmiyorsa, Microsoft [365'i](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirme.</span><span class="sxs-lookup"><span data-stu-id="db2de-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="db2de-136">Mevcut DNS kayıtlarınız, örneğin var olan bir web siteniz [](/office365/admin/get-help-with-domains/domain-connect)varsa, ancak etki alanı bağlantısı için DNS barındırma etkinleştirilmişse, Kayıtları benim için **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="db2de-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="db2de-137">Çevrimiçi **hizmetlerinizi seçin sayfasında,** tüm varsayılanları kabul edin ve  Sonraki'ni seçin ve DNS barındırma barındırma hizmet nizin sayfasında Yetkilendir'i seçin.</span><span class="sxs-lookup"><span data-stu-id="db2de-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="db2de-138">Diğer DNS ana bilgisayarlarında var olan DNS kayıtlarınız varsa (etki alanı bağlantısı için etkin değil), mevcut hizmetlerin bağlı kalacağından emin olmak için kendi DNS kayıtlarınızı yönetmek istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="db2de-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="db2de-139">Daha [fazla bilgi için etki alanı](/office365/admin/get-help-with-domains/dns-basics) temel bilgilerine bakın.</span><span class="sxs-lookup"><span data-stu-id="db2de-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Kayıtları etkinleştirme sayfası.](../media/activaterecords.png)

2. <span data-ttu-id="db2de-141">Sihirbazda adımları izleyin; e-posta ve diğer hizmetler sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="db2de-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="db2de-142">Organizasyonlarınızı koruyun</span><span class="sxs-lookup"><span data-stu-id="db2de-142">Protect your organization</span></span> 

<span data-ttu-id="db2de-143">Sihirbazda ayarlanıyor olan ilkeler, Tüm Kullanıcılar adlı [Güvenlik grubuna otomatik](/office365/admin/create-groups/compare-groups#security-groups) olarak *uygulanır.*</span><span class="sxs-lookup"><span data-stu-id="db2de-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="db2de-144">Ayrıca, yönetim merkezinde ilke atamak için ek gruplar da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="db2de-145">Gelişmiş siber **tehditlere karşı** korumayı artırarak, [Office 365'in](../security/office-365-security/defender-for-office-365.md) Tehdit Koruması'nın Office uygulamalarına dosya ve bağlantı taramasına izin verme varsayılanlarını kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="db2de-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Korumayı artır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. <span data-ttu-id="db2de-147">Hassas veri **sızıntılarını** önle sayfasında, Office uygulamaları içinde hassas verileri izlemek ve bunların kuruluş dışında yanlışlıkla paylaşımını önlemek için Office 365 Veri Kaybı Önleme'nin (DLP) varsayılanlarını kabul edin.</span><span class="sxs-lookup"><span data-stu-id="db2de-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="db2de-148">Mobil cihazlar **için Office'te** verileri koru sayfasında, mobil uygulama yönetimini açık bırakın, ayarları genişletin ve gözden geçirin ve ardından Mobil uygulama **yönetimi ilkesi oluştur'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="db2de-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Mobil için Office sayfasındaki verileri koru sayfasının ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="db2de-150">Windows 10 bilgisayarlarında güvenlik sağlama</span><span class="sxs-lookup"><span data-stu-id="db2de-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="db2de-151">Sol gezintide Kurulum'u **seçin** ve ardından Oturum açma ve güvenlik altında Windows **10** bilgisayarlarınızı güvenli hale seçin.</span><span class="sxs-lookup"><span data-stu-id="db2de-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="db2de-152">Başlamak **için** Görüntüle'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="db2de-152">Choose **View** to get started.</span></span> <span data-ttu-id="db2de-153">Eksiksiz [yönergeler için Windows 10 bilgisayarlarınızı](secure-win-10-pcs.md) güvenli hale bakın.</span><span class="sxs-lookup"><span data-stu-id="db2de-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="db2de-154">Office 365 istemci uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="db2de-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="db2de-155">Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi tercih edersiniz, kullanıcılar Windows cihazlarından Azure AD'de oturum açmaları için iş kimlik bilgilerini kullanarak Windows 10 cihazlarına yüklenir.</span><span class="sxs-lookup"><span data-stu-id="db2de-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="db2de-156">Office'i mobil iOS veya Android cihazlara yüklemek için Bkz. [Microsoft 365 İş Ekstra](set-up-mobile-devices.md)kullanıcıları için mobil cihazları ayarlama.</span><span class="sxs-lookup"><span data-stu-id="db2de-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="db2de-157">Office'i tek tek de yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="db2de-157">You can also install Office individually.</span></span> <span data-ttu-id="db2de-158">Yönergeler [için BKZ. PC veya Mac bilgisayara Office](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) yükleme.</span><span class="sxs-lookup"><span data-stu-id="db2de-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="db2de-159">Ayrıca bk.</span><span class="sxs-lookup"><span data-stu-id="db2de-159">See also</span></span>

[<span data-ttu-id="db2de-160">İş için Microsoft 365 eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="db2de-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
