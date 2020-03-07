---
title: Microsoft 365 Business'ı ayarlama
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Bir etki alanı ve kullanıcı ekleme, güvenlik ilkeleri ayarlama ve daha fazlası dahil olmak üzere Microsoft 365 Business için kurulum adımlarını keşfedin.
ms.openlocfilehash: 99994b6f1e9e817b4858aeafe4ce3ceaaf4c3c37
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561200"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="60db6-103">Kurulum sihirbazında Microsoft 365 Business'ı ayarlama</span><span class="sxs-lookup"><span data-stu-id="60db6-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="60db6-104">Microsoft 365 İş kurulumuna genel bir bakış için bu videoyu izleyin.</span><span class="sxs-lookup"><span data-stu-id="60db6-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="60db6-105">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).  </span><span class="sxs-lookup"><span data-stu-id="60db6-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="60db6-106">Etki alanınızı, kullanıcılarınızı ekleyin ve ilkeler ayarlayın</span><span class="sxs-lookup"><span data-stu-id="60db6-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="60db6-107">[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="60db6-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="60db6-108">Microsoft 365 Business'ı satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında bir etki alanı satın alma seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="60db6-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="60db6-109">Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınız tamamen ayarlanmıştır ve [kullanıcı ekle'ye taşınabilir ve lisans atayabilirsiniz.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="60db6-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="60db6-110">Oturum açma'yı kişiselleştirmek için etki alanınızı ekleyin</span><span class="sxs-lookup"><span data-stu-id="60db6-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="60db6-111">Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 yönetici merkezinde](https://admin.microsoft.com) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="60db6-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="60db6-112">Sihirbazı başlatmak **için kuruluma git'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Kuruluma Git'i seçin.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="60db6-114">Office **uygulamalarınızı yükle** sayfasında, uygulamaları isteğe bağlı olarak kendi bilgisayarınıza yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="60db6-115">Etki **alanı ekle** adımında, kullanmak istediğiniz etki alanı adını girin (contoso.com gibi).</span><span class="sxs-lookup"><span data-stu-id="60db6-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="60db6-116">Kayıt sırasında bir etki alanı satın aldıysanız, burada **bir etki alanı** adımı ekle'yi görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="60db6-117">Bunun yerine [Kullanıcı Ekle'ye](#add-users-and-assign-licenses) gidin.</span><span class="sxs-lookup"><span data-stu-id="60db6-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Oturum açma sayfanızı Kişiselleştir'in ekran görüntüsü.](../media/adddomain.png)

    
4. <span data-ttu-id="60db6-119">Etki alanına sahip olduğunuzu doğrulayan [Office 365 için herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="60db6-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="60db6-120">Etki alanı ana bilgisayarınızı tanıyorsanız, [ana bilgisayara özel yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)de bakın.</span><span class="sxs-lookup"><span data-stu-id="60db6-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="60db6-121">Barındırma sağlayıcınız GoDaddy veya etki [alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yla etkin leştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmanız ve Microsoft'un sizin adınıza kimliğini belirlemesine izin vermeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="60db6-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![GoDaddy Access'i Onayla sayfasında Yetkilendirme'yi seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="60db6-123">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="60db6-123">Add users and assign licenses</span></span>

<span data-ttu-id="60db6-124">Sihirbaza kullanıcı ekleyebilirsiniz, ancak daha sonra yönetici merkezine [de ekleyebilirsiniz.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="60db6-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="60db6-125">Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect'e](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)sahip kullanıcılar ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="60db6-126">Sihirbaza kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="60db6-126">Add users in the wizard</span></span>

<span data-ttu-id="60db6-127">Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak Microsoft 365 Business lisansı atanabilir.</span><span class="sxs-lookup"><span data-stu-id="60db6-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Sihirbazda yeni kullanıcı ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. <span data-ttu-id="60db6-129">Microsoft 365 Business aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect'i kullandıysanız), şimdi onlara lisans atama seçeneğine sahip siniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="60db6-130">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="60db6-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="60db6-131">Kullanıcıları ekledikten sonra, kimlik bilgilerini eklediğiniz yeni kullanıcılarla paylaşma seçeneği de alırsınız.</span><span class="sxs-lookup"><span data-stu-id="60db6-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="60db6-132">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="60db6-133">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="60db6-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="60db6-134">.onmicrosoft etki alanını kullanmayı seçtiyseniz veya kullanıcıları ayarlamak için Azure AD Connect'i kullandıysanız, bu adımı görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="60db6-135">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="60db6-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="60db6-136">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="60db6-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="60db6-137">Yoksa, [office 365'i herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirin.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)</span><span class="sxs-lookup"><span data-stu-id="60db6-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="60db6-138">Varolan DNS kayıtlarınız varsa, örneğin varolan bir web sitesi, ancak [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için DNS ana bilgisayarınız etkinse, benim için kayıt **ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="60db6-139">Çevrimiçi **hizmetleri seç** sayfasında, tüm varsayılanları kabul edin ve **Sonraki'ni**seçin ve DNS ana bilgisayarınızın sayfasında **Yetkilendirme'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="60db6-140">Diğer DNS ana bilgisayarlarıyla varolan DNS kayıtlarınız varsa (etki alanı bağlantısı için etkinleştirildi), varolan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek istersiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="60db6-141">Daha fazla bilgi için [etki alanı temellerine](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bakın.</span><span class="sxs-lookup"><span data-stu-id="60db6-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Kayıtlar sayfasını etkinleştirin.](../media/activaterecords.png)

2. <span data-ttu-id="60db6-143">Sihirbazve e-posta ve diğer hizmetler adımları izleyin sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="60db6-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="60db6-144">Kuruluşunuzu koruyun</span><span class="sxs-lookup"><span data-stu-id="60db6-144">Protect your organization</span></span> 

<span data-ttu-id="60db6-145">Sihirbazda ayarladığınız *ilkeler, Tüm Kullanıcılar*adlı bir [Güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="60db6-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="60db6-146">Ayrıca, yönetici merkezinde ilkeler atamak için ek gruplar oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="60db6-147">Gelişmiş **siber tehditlere karşı korumayı**artırın'da, Office [365 Önceden Tehdit Koruması'nın](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Office uygulamalarındaki dosyaları ve bağlantıları taramasına izin verme varsayılanlarını kabul etmeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="60db6-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Korumayı Artır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. <span data-ttu-id="60db6-149">Hassas **veri sayfasının sızıntılarını önlemede,** Office uygulamalarındaki hassas verileri izlemek ve bunların kuruluşunuz dışında yanlışlıkla paylaşılmasını önlemek için Office 365 Veri Kaybı Önleme'yi (DLP) açma varsayılanlarını kabul edin.</span><span class="sxs-lookup"><span data-stu-id="60db6-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="60db6-150">Mobil sayfa **için Office'teki verileri koru'da** mobil uygulama yönetimini bırakın, ayarları genişletin ve gözden geçirin ve ardından **mobil uygulama yönetimi ilkesi oluştur'u**seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Mobil sayfa için Office'teki verileri koruyun ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="60db6-152">Güvenli Windows 10 cd'leri</span><span class="sxs-lookup"><span data-stu-id="60db6-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="60db6-153">Sol daki gezinmede **Kurulum'u** seçin ve ardından **Sing-in ve security**altında Windows **10 bilgisayarlarınızı güvenli**olarak seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="60db6-154">Başlamak için **Görünüm'u** seçin.</span><span class="sxs-lookup"><span data-stu-id="60db6-154">Choose **View** to get started.</span></span> <span data-ttu-id="60db6-155">Tam talimatlar için [Windows 10 bilgisayarlarınızı güvenli olarak](secure-win-10-pcs.md) görün.</span><span class="sxs-lookup"><span data-stu-id="60db6-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="60db6-156">Office 365 istemci uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="60db6-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="60db6-157">Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar iş kimlik bilgilerini kullanarak Windows aygıtlarından Azure AD'ye oturum açtıktan sonra uygulamalar Windows 10 cihazlarına yüklenir.</span><span class="sxs-lookup"><span data-stu-id="60db6-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="60db6-158">Office'i mobil iOS veya Android cihazlara yüklemek [için](set-up-mobile-devices.md)bkz.</span><span class="sxs-lookup"><span data-stu-id="60db6-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="60db6-159">Office'i tek tek yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60db6-159">You can also install Office individually.</span></span> <span data-ttu-id="60db6-160">Talimatlar için [Office'i pc'ye veya Mac'e yükleyin'](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) e bakın.</span><span class="sxs-lookup"><span data-stu-id="60db6-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="60db6-161">Ayrıca bkz.</span><span class="sxs-lookup"><span data-stu-id="60db6-161">See also</span></span>

[<span data-ttu-id="60db6-162">Microsoft 365 İş eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="60db6-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
