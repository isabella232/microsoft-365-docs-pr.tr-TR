---
title: Microsoft 365 Business Premium 'u ayarlama
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Etki alanı ve Kullanıcı ekleme, güvenlik ilkelerini ayarlama gibi Microsoft 365 Iş ekstra için kurulum adımlarını keşfedin.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324506"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="d8974-103">Kurulum sihirbazında Microsoft 365 Business Premium 'u ayarlama</span><span class="sxs-lookup"><span data-stu-id="d8974-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="d8974-104">Microsoft 365 Business Premium kurulumuna genel bir bakış için bu videoyu izleyin.</span><span class="sxs-lookup"><span data-stu-id="d8974-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="d8974-105">Etki alanınızı, kullanıcılarınızı ve kurulum ilkelerini ekleme</span><span class="sxs-lookup"><span data-stu-id="d8974-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="d8974-106">Microsoft 365 Business Premium satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında satın alma seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="d8974-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="d8974-107">Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınızın tümü ayarlanır ve [Kullanıcı ekleme ve lisans atama](#add-users-and-assign-licenses)'ya taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="d8974-108">Kişiselleştirme oturum açma</span><span class="sxs-lookup"><span data-stu-id="d8974-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="d8974-109">Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) 'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="d8974-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="d8974-110">Sihirbazı başlatmak için **Kuruluma git** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Kuruluma git 'i seçin.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="d8974-112">**Office uygulamalarınızı yükleyin** sayfasında isteğe bağlı olarak uygulamaları kendi bilgisayarınıza yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="d8974-113">**Etki alanı Ekle** adımında, kullanmak istediğiniz etki alanı adını girin (contoso.com gibi).</span><span class="sxs-lookup"><span data-stu-id="d8974-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="d8974-114">Kayıt sırasında bir etki alanı satın aldıysanız, burada **etki alanı adımı ekle** seçeneğini görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="d8974-115">Bunun yerine [Kullanıcı ekleme](#add-users-and-assign-licenses) bölümüne gidin.</span><span class="sxs-lookup"><span data-stu-id="d8974-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Oturum açma sayfanızı kişiselleştirin sayfasının ekran görüntüsü.](../media/adddomain.png)

    
4. <span data-ttu-id="d8974-117">[Microsoft 365 için herhangi BIR DNS barındırma sağlayıcısında](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) etki alanının sahibi olduğunuzu doğrulayan DNS kayıtlarını oluşturmak için sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="d8974-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="d8974-118">Etki alanı konağını biliyorsanız, ayrıca [ana bilgisayara özgü yönergelere](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)bakın.</span><span class="sxs-lookup"><span data-stu-id="d8974-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="d8974-119">Barındırma sağlayıcınız GoDaddy veya [etki alanı Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)ile başka bir ana bilgisayar etkinleştirilmişse, süreç kolaydır ve oturum açmanız ve Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d8974-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![GoDaddy erişimini Onayla sayfasında Yetkilendir 'i seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="d8974-121">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="d8974-121">Add users and assign licenses</span></span>

<span data-ttu-id="d8974-122">Sihirbazda kullanıcı ekleyebilirsiniz, ancak bunları [daha sonra](add-users-m365b.md) Yönetim merkezinde ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="d8974-123">Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ile kullanıcı ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="d8974-124">Sihirbazda Kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="d8974-124">Add users in the wizard</span></span>

<span data-ttu-id="d8974-125">Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak Microsoft 365 Business Premium Lisansı atanır.</span><span class="sxs-lookup"><span data-stu-id="d8974-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Sihirbazdaki yeni kullanıcılar Ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. <span data-ttu-id="d8974-127">Microsoft 365 Business Premium aboneliğiniz var olan kullanıcılara sahipse (örneğin, Azure AD Connect kullandıysanız), onlara şimdi lisans atama seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="d8974-128">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="d8974-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="d8974-129">Kullanıcıları ekledikten sonra, eklediğiniz yeni kullanıcılarla kimlik bilgilerini paylaşma seçeneği de alırsınız.</span><span class="sxs-lookup"><span data-stu-id="d8974-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="d8974-130">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="d8974-131">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="d8974-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="d8974-132">Kullanıcıları ayarlamak için. adımmicrosoft etki alanını kullanmayı seçtiyseniz veya Azure AD Connect 'i kullandıysanız, bu adımı görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="d8974-133">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d8974-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="d8974-134">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="d8974-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="d8974-135">Desteklemiyorsa, [ad sunucularını değiştirerek etki alanı kayıt kaydediciyle Microsoft 365 'i ayarlayın](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="d8974-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="d8974-136">Var olan bir Web sitesi gibi DNS kayıtlarınız varsa ancak DNS ana bilgisayarı [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için etkinleştirilmişse, **benim için kayıt Ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="d8974-137">**Çevrimiçi hizmetler 'ı seçin** sayfasında tüm varsayılanları kabul edin ve ileri 'Yi ve **ardından**DNS ana bilgisayarınızın sayfasında **Yetkilendir** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="d8974-138">Başka DNS ana bilgisayarlarıyla (etki alanı bağlantısı için etkinleştirilmemiş) DNS kayıtlarınız varsa, var olan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="d8974-139">Daha fazla bilgi için [etki alanı temel](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bilgilerine bakın.</span><span class="sxs-lookup"><span data-stu-id="d8974-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Kayıtları etkinleştir sayfası.](../media/activaterecords.png)

2. <span data-ttu-id="d8974-141">Sihirbazdaki ve e-postadaki adımları izleyin ve diğer hizmetler sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="d8974-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="d8974-142">Kuruluşunuzu koruma</span><span class="sxs-lookup"><span data-stu-id="d8974-142">Protect your organization</span></span> 

<span data-ttu-id="d8974-143">Sihirbazda ayarladığınız ilkeler, *tüm kullanıcılar*adındaki bir [güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="d8974-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="d8974-144">Yönetim merkezinde ilke atamak için ek gruplar da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="d8974-145">**Gelişmiş siber tehditlerden korunma koruması**üzerinde, [Office 365 öncelikli tehdit koruması](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Office uygulamalarında dosya ve bağlantıları taratmak için varsayılanları kabul etmeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="d8974-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Korumayı arttır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. <span data-ttu-id="d8974-147">**Hassas verileri sızıntıları önle** sayfasında, Office uygulamalarında hassas verileri izlemek ve kuruluşunuzun dışından bunları yanlışlıkla paylaşmayı önleyen Office 365 veri kaybı önleme (DLP) özelliğini açmak için varsayılanları kabul edin.</span><span class="sxs-lookup"><span data-stu-id="d8974-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="d8974-148">**Mobil Için Office 'te verileri koruyarak** sayfasında mobil uygulama yönetimi 'nden çıkın, ayarlar 'ı genişletin ve ardından **mobil uygulama yönetim ilkesi oluştur**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Mobil için Office 'te verileri korumama ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="d8974-150">Windows 10 bilgisayarlarında güvenli</span><span class="sxs-lookup"><span data-stu-id="d8974-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="d8974-151">Sol gezintide, **Kurulum 'u** seçin ve ardından **oturum açma ve güvenlik**altında **Windows 10 bilgisayarlarınızı güvenli**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="d8974-152">Başlamak için **görüntüle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d8974-152">Choose **View** to get started.</span></span> <span data-ttu-id="d8974-153">Tüm yönergeler için [Windows 10 bilgisayarlarınızın güvenliğini sağlama](secure-win-10-pcs.md) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="d8974-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="d8974-154">Office 365 istemci uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="d8974-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="d8974-155">Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar Windows cihazlarında Azure AD 'de oturum açtıktan sonra iş kimlik bilgilerini kullanarak uygulamalar Windows 10 aygıtlarına yüklenir.</span><span class="sxs-lookup"><span data-stu-id="d8974-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="d8974-156">Office 'i mobil iOS veya Android cihazlarda yüklemek için, [Microsoft 365 Business Premium kullanıcıları için mobil cihazları ayarlama](set-up-mobile-devices.md)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d8974-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="d8974-157">Ayrıca Office 'i tek tek da yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8974-157">You can also install Office individually.</span></span> <span data-ttu-id="d8974-158">Yönergeler için [PC veya Mac 'e Office yükleme](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="d8974-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="d8974-159">Ayrıca bkz.</span><span class="sxs-lookup"><span data-stu-id="d8974-159">See also</span></span>

[<span data-ttu-id="d8974-160">Microsoft 365 iş eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="d8974-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
