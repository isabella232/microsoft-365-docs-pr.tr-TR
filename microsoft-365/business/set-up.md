---
title: Microsoft 365 Business'ı ayarlama
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
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 iş kurmayı öğrenin.
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966988"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="7028f-103">Kur Sihirbazı'nda Microsoft 365 işletmeniz ayarlama</span><span class="sxs-lookup"><span data-stu-id="7028f-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="7028f-104">Etki alanı, kullanıcılar, ekleme ve ilkelerini kurun</span><span class="sxs-lookup"><span data-stu-id="7028f-104">Add your domain, users, and set up policies</span></span>

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="7028f-106">Microsoft 365 iş satın aldığınızda, size ait olan bir etki alanı kullanarak ya da sırasında satın seçeneğiniz [Kaydolma](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="7028f-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="7028f-107">Siz oturum açtığınızda yeni bir etki alanı satın aldıysanız, etki alanınızın tüm yedekleme kümesidir ve [lisanslar atayabilir ve kullanıcıları eklemek](#add-users-and-assign-licenses)için taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="7028f-108">Oturum kişiselleştirmek için etki alanı ekleme</span><span class="sxs-lookup"><span data-stu-id="7028f-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="7028f-109">[Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) genel yönetici kimlik bilgilerinizi kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="7028f-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="7028f-110">**Ekle bir etki alanı** veya **Kullanıcı Ekle** Sihirbazı'nı başlatmak için seçin.</span><span class="sxs-lookup"><span data-stu-id="7028f-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="7028f-111">Kayıt sırasında bir etki alanı satın aldıysanız, değil bkz: **etki alanı eklemek** adım burada olur.</span><span class="sxs-lookup"><span data-stu-id="7028f-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="7028f-112">Bunun yerine, [Kullanıcı Ekle](#add-users-and-assign-licenses) gidin.</span><span class="sxs-lookup"><span data-stu-id="7028f-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Bir etki alanına Ekle'yi seçin.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="7028f-114">Sihirbazda, (contoso.com gibi) kullanmak istediğiniz etki alanı adını girin.</span><span class="sxs-lookup"><span data-stu-id="7028f-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Oturum açma sayfası kişiselleştirme ekran görüntüsü.](media/personalizesignin.png)

    
4. <span data-ttu-id="7028f-116">Doğrulayan etki alanı sahibi [herhangi bir DNS barındırma sağlayıcı için Office 365 oluşturmak DNS kayıtları](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) için sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="7028f-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="7028f-117">Ayrıca, etki alanı ana biliyorsanız, [ana bilgisayar belirli yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)bakın.</span><span class="sxs-lookup"><span data-stu-id="7028f-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="7028f-118">GoDaddy barındırma sağlayıcınıza ise, kolay bir işlemdir ve sizden oturum açıp Microsoft'un sizin adınıza kimliğini otomatik olarak istenecektir:</span><span class="sxs-lookup"><span data-stu-id="7028f-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy erişimi Onayla sayfasında, Authorize seçeneğini seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="7028f-120">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="7028f-120">Add users and assign licenses</span></span>

<span data-ttu-id="7028f-121">Sihirbazda kullanıcılar ekleyebilirsiniz, ancak [daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de olabilir.</span><span class="sxs-lookup"><span data-stu-id="7028f-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="7028f-122">Ayrıca, yerel etki alanı denetleyicisi varsa, [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ile kullanıcılar ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="7028f-123">Kullanıcı Ekleme Sihirbazı'nda</span><span class="sxs-lookup"><span data-stu-id="7028f-123">Add users in the wizard</span></span>

<span data-ttu-id="7028f-124">Sihirbazda eklediğiniz kullanıcılar Microsoft 365 işletme lisans otomatik olarak atanan.</span><span class="sxs-lookup"><span data-stu-id="7028f-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Ekle yeni kullanıcılar Sayfa Sihirbazı'nda ekran görüntüsü](media/addnewuserspage.png)

1. <span data-ttu-id="7028f-126">Varolan kullanıcıların (örneğin, Azure AD Connect kullandıysanız) Microsoft 365 iş aboneliğiniz varsa, lisansları şimdi onlara atamak için bir seçenek alın.</span><span class="sxs-lookup"><span data-stu-id="7028f-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="7028f-127">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="7028f-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="7028f-128">Kullanıcıları ekledikten sonra kimlik bilgileri eklediğiniz yeni kullanıcıları ile paylaşmak için bir seçenek de alırsınız.</span><span class="sxs-lookup"><span data-stu-id="7028f-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="7028f-129">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="7028f-130">E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7028f-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="7028f-131">Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="7028f-132">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="7028f-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="7028f-133">.Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Connect kullanıcıları ayarlamak için kullanılan, bu adımı göremez.</span><span class="sxs-lookup"><span data-stu-id="7028f-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="7028f-134">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="7028f-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="7028f-135">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="7028f-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="7028f-136">Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="7028f-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="7028f-137">Varolan bir web sitesi gibi varolan DNS kayıtları varsa, varolan Hizmetleri bağlı kalmak emin olmak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="7028f-138">[Etki alanı temelleri](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="7028f-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Etki alanınızı Bağlan sayfası ben kendi DNS kayıtlarını yönetmek.](media/connectyourdomainpage.png)

2. <span data-ttu-id="7028f-140">Sihirbazı'ndaki adımları izleyin ve e-posta ve diğer hizmetleri sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="7028f-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="7028f-141">Güvenlik ilkeleri ve aygıt yapılandırmaları ayarlama</span><span class="sxs-lookup"><span data-stu-id="7028f-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="7028f-142">Sihirbazda ayarladığınız ilkeleri *Tüm kullanıcıları*adlı bir [güvenlik grubu](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="7028f-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="7028f-143">Yönetim Merkezi için ilkeleri atamak için ek grupları da oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="7028f-144">**Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** **mobil cihazlarda iş dosyalarınızı korumak** üzerinde seçeneği varsayılan olarak seçilidir.</span><span class="sxs-lookup"><span data-stu-id="7028f-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="7028f-145">**Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek**bırakma seçeneği vardır ve bu önerilir.</span><span class="sxs-lookup"><span data-stu-id="7028f-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Mobil aygıtlar sayfasında, ekran görüntüsü korumaya çalışma dosyaları.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="7028f-147">**Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** [varsayılan değerleri](protect-work-files-on-lost-or-stolen-device.md)görüntülemek için genişlet:</span><span class="sxs-lookup"><span data-stu-id="7028f-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Ekran görüntüsü aygıtlarında kayıp dosyaları korumak için varsayılan değerler.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="7028f-149">**Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini Yönet** ' i seçin ve [varsayılan değerlerini](manage-user-access-on-mobile-devices.md)görüntülemek için genişletin.</span><span class="sxs-lookup"><span data-stu-id="7028f-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="7028f-150">Android, IOS ve Windows 10 uygulama ilkeleri oluşturmak için Kurulum sırasında tüm kullanıcılar için geçerli varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="7028f-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="7028f-151">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-151">You can create more policies after setup completes.</span></span>

        ![Mobile Office dosyaları için koruma ayarları ekran görüntüsü.](media/useraccessonmobile.png)

2. <span data-ttu-id="7028f-153">Son adımda, veri koruma ve aygıtları Windows 10 aygıtlar güvenli hale getirmek için ilkeler ayarlamanıza olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="7028f-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="7028f-154">Kuruluşunuzda bir kullanıcının Windows 10 bağlandığında, bu ayarları otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="7028f-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="7028f-155">**Güvenli Windows 10 aygıtları** görmek ve [varsayılan değerlerini](secure-windows-10-devices.md)değiştirmek için genişletebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="7028f-156">Windows 10 cihazlarda [Office otomatik olarak yüklemek](install-office-on-windows-10-during-setup.md) için seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Ekran görüntüsünü Windows 10 aygıt yapılandırma sayfası ayarlayın.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="7028f-158">Office 365 istemci uygulamaları dağıtma</span><span class="sxs-lookup"><span data-stu-id="7028f-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="7028f-159">Otomatik olarak yedekleme kümesi sırasında Office uygulamaları yüklemek seçerseniz, kullanıcılar için Azure AD iş kimlik bilgilerini Windows aygıtlarına gelen oturum açtıktan sonra Windows 10 aygıtlarda apps yükleyecektir.</span><span class="sxs-lookup"><span data-stu-id="7028f-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="7028f-160">Office mobile IOS veya Android aygıtları yüklemek için [Microsoft 365 iş kullanıcıları için mobil aygıtları ayarlayın](set-up-mobile-devices.md)bkz.</span><span class="sxs-lookup"><span data-stu-id="7028f-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="7028f-161">Office ayrı olarak da yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7028f-161">You can also install Office individually.</span></span> <span data-ttu-id="7028f-162">[Bir PC veya Mac Office yükleme](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) yönergeleri için bkz.</span><span class="sxs-lookup"><span data-stu-id="7028f-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
