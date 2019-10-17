---
title: Microsoft 365 Business'ı ayarlama
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business'ı nasıl ayarlayın öğrenin.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575558"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="39f0b-103">Kurulum sihirbazında Microsoft 365 Business'ı ayarlama</span><span class="sxs-lookup"><span data-stu-id="39f0b-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="39f0b-104">Etki alanınızı, kullanıcılarınızı ekleyin ve ilkeler ayarlayın</span><span class="sxs-lookup"><span data-stu-id="39f0b-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="39f0b-105">[![Yönetici merkezinin değiştiğini bildirmek için etiket ve aka.ms/aboutM365preview daha fazla ayrıntı bulabilirsiniz.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="39f0b-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="39f0b-106">Microsoft 365 Business'ı satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında bir etki alanı satın alma seçeneğiniz vardır.</span><span class="sxs-lookup"><span data-stu-id="39f0b-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="39f0b-107">Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınız tamamen ayarlanmıştır ve [kullanıcı ekle'ye taşınabilir ve lisans atayabilirsiniz.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="39f0b-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="39f0b-108">Oturum açma'yı kişiselleştirmek için etki alanınızı ekleyin</span><span class="sxs-lookup"><span data-stu-id="39f0b-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="39f0b-109">Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 yönetici merkezinde](https://admin.microsoft.com) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="39f0b-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="39f0b-110">Sihirbazı başlatmak için **etki alanı ekle** veya kullanıcı **ekle'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="39f0b-111">Kayıt sırasında bir etki alanı satın aldıysanız, burada **bir etki alanı** adımı ekle'yi görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="39f0b-112">Bunun yerine [Kullanıcı Ekle'ye](#add-users-and-assign-licenses) gidin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Kuruluma Git'i seçin.](media/gotosetupinadmincenter.png)
    
3. <span data-ttu-id="39f0b-114">Sihirbazda, kullanmak istediğiniz alan adını girin (contoso.com gibi).</span><span class="sxs-lookup"><span data-stu-id="39f0b-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Oturum açma sayfanızı Kişiselleştir'in ekran görüntüsü.](media/personalizesignin.png)

    
4. <span data-ttu-id="39f0b-116">Etki alanına sahip olduğunuzu doğrulayan [Office 365 için herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="39f0b-117">Etki alanı ana bilgisayarınızı tanıyorsanız, [ana bilgisayara özel yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)de bakın.</span><span class="sxs-lookup"><span data-stu-id="39f0b-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="39f0b-118">Barındırma sağlayıcınız GoDaddy veya [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yla etkin leştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmanız ve Microsoft'un sizin adınıza kimlik doğrulamasına izin vermeniz istenir:</span><span class="sxs-lookup"><span data-stu-id="39f0b-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy Access'i Onayla sayfasında Yetkilendirme'yi seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="39f0b-120">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="39f0b-120">Add users and assign licenses</span></span>

<span data-ttu-id="39f0b-121">Sihirbaza kullanıcı ekleyebilirsiniz, ancak daha sonra yönetici merkezine [de ekleyebilirsiniz.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="39f0b-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="39f0b-122">Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect'e](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)sahip kullanıcılar ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="39f0b-123">Sihirbaza kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="39f0b-123">Add users in the wizard</span></span>

<span data-ttu-id="39f0b-124">Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak microsoft 365 Business lisansı atanabilir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Sihirbazda yeni kullanıcı ekle sayfasının ekran görüntüsü](media/addnewuserspage.png)

1. <span data-ttu-id="39f0b-126">Microsoft 365 Business aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect'i kullandıysanız) artık onlara lisans atama seçeneğine sahip olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="39f0b-127">Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-127">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="39f0b-128">Kullanıcıları ekledikten sonra, eklediğiniz yeni kullanıcılarla kimlik bilgilerini paylaşma seçeneği de alırsınız.</span><span class="sxs-lookup"><span data-stu-id="39f0b-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="39f0b-129">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-129">You can choose to print them out, email them, or download them.</span></span>

3. <span data-ttu-id="39f0b-130">Kuruluşunuz için Ekipler Oluştur'da, Takımlar eklemeyi ve onlara kullanıcı eklemeyi seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-130">On the Create Teams for your organization, you can choose to add Teams and add users to them.</span></span> <span data-ttu-id="39f0b-131">Bunu daha sonra da yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-131">You can also do this later.</span></span> <span data-ttu-id="39f0b-132">Daha fazla bilgi için [bkz.](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3)</span><span class="sxs-lookup"><span data-stu-id="39f0b-132">For more information, see [create a company-wide Team](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span></span>

4. <span data-ttu-id="39f0b-133">E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-133">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="39f0b-134">Başka bir e-posta sağlayıcısından taşınıyorsanız ve verilerinizi daha sonra kopyalamak istiyorsanız, [e-posta ve kişileri Office 365'e geçirebilirsiniz.](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)</span><span class="sxs-lookup"><span data-stu-id="39f0b-134">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="39f0b-135">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="39f0b-135">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="39f0b-136">.onmicrosoft etki alanını kullanmayı seçtiyseniz veya kullanıcıları ayarlamak için Azure AD Connect'i kullandıysanız, bu adımı görmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-136">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="39f0b-137">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-137">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="39f0b-138">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-138">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="39f0b-139">Yoksa, [office 365'i herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirin.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)</span><span class="sxs-lookup"><span data-stu-id="39f0b-139">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="39f0b-140">Varolan DNS kayıtlarınız varsa, örneğin varolan bir web sitesi, ancak [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için DNS ana bilgisayarınız etkinse, benim için kayıt **ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-140">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="39f0b-141">Çevrimiçi **hizmetleri seç** sayfasında, tüm varsayılanları kabul edin ve **Sonraki'ni**seçin ve DNS ana bilgisayarınızın sayfasında **Yetkilendirme'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-141">On the **Choose your online services** page, accept all the defaults, and choose **Next**,and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="39f0b-142">Diğer DNS ana bilgisayarlarıyla varolan DNS kayıtlarınız varsa (etki alanı bağlantısı için etkinleştirilmez), varolan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek istersiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-142">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="39f0b-143">Daha fazla bilgi için [etki alanı temellerine](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bakın.</span><span class="sxs-lookup"><span data-stu-id="39f0b-143">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Etki alanı sayfanızı kendi DNS kayıtlarımı yönetirim.](media/connectyourdomainpage.png)

2. <span data-ttu-id="39f0b-145">Sihirbazve e-posta ve diğer hizmetler adımları izleyin sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="39f0b-145">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-data-and-devices"></a><span data-ttu-id="39f0b-146">Verileri ve cihazları koruma</span><span class="sxs-lookup"><span data-stu-id="39f0b-146">Protect data and devices</span></span> 

<span data-ttu-id="39f0b-147">Sihirbazda ayarladığınız *ilkeler, Tüm Kullanıcılar*adlı bir [Güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="39f0b-147">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="39f0b-148">Ayrıca, yönetici merkezinde ilkeler atamak için ek gruplar oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-148">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="39f0b-149">Mobil **cihazlardaki iş dosyalarınızı koru** **seçeneği, aygıtlar kaybolduğunda veya çalındığında iş dosyalarını koruyun** seçeneği varsayılan olarak seçilir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-149">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="39f0b-150">**Kullanıcıların mobil cihazlardaki Office dosyalarına nasıl erişirlerini yönet'i**açma seçeneğiniz vardır ve bu önerilir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-150">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Mobil cihazlar sayfasındaki çalışma dosyalarını koru ekran görüntüsü.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="39f0b-152">**Aygıtlar kaybolduğunda veya çalındığında varsayılan** [değerleri](protect-work-files-on-lost-or-stolen-device.md)görüntülemek için iş dosyalarını koruyun'u genişletin:</span><span class="sxs-lookup"><span data-stu-id="39f0b-152">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Kayıp aygıtlarda dosyaları korumak için varsayılan değerlerin ekran görüntüsü.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="39f0b-154">**Kullanıcıların mobil cihazlardaki Office dosyalarına nasıl eriştürün** ünü yönet'i seçin ve varsayılan [değerleri](manage-user-access-on-mobile-devices.md)görüntülemek için genişletin.</span><span class="sxs-lookup"><span data-stu-id="39f0b-154">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="39f0b-155">Tüm kullanıcılar için geçerli olan Android, iOS ve Windows 10 için uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-155">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="39f0b-156">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-156">You can create more policies after setup completes.</span></span>

        ![Mobil cihazlardaki Office dosyaları için koruma ayarlarının ekran görüntüsü.](media/useraccessonmobile.png)

2. <span data-ttu-id="39f0b-158">Verileri ve aygıtları koruma konusundaki son adım, Windows 10 aygıtlarını korumak için ilkeler ayarlamanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="39f0b-158">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="39f0b-159">Bu ayarlar, bir kullanıcının Windows 10'u kuruluşunuza bağlandığında otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="39f0b-159">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="39f0b-160">[Varsayılan değerleri](secure-windows-10-devices.md)görmek ve değiştirmek için Güvenli **Windows 10 aygıtlarını** genişletebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-160">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="39f0b-161">Office'i Windows 10 aygıtlarına [otomatik olarak yüklemeyi](install-office-on-windows-10-during-setup.md) de seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-161">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Set Windows 10 aygıt yapılandırma sayfasının ekran görüntüsü.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="39f0b-163">Office 365 istemci uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="39f0b-163">Deploy Office 365 client apps</span></span>

<span data-ttu-id="39f0b-164">Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar windows aygıtlarından Iş kimlik bilgileriyle Azure AD'ye oturum açtıktan sonra uygulamalar Windows 10 cihazlarına yüklenir.</span><span class="sxs-lookup"><span data-stu-id="39f0b-164">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="39f0b-165">Office'i mobil iOS veya Android cihazlara yüklemek [için](set-up-mobile-devices.md)bkz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-165">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="39f0b-166">Office'i tek tek yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="39f0b-166">You can also install Office individually.</span></span> <span data-ttu-id="39f0b-167">Talimatlar için [Office'i pc'ye veya Mac'e yükleyin'](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) e bakın.</span><span class="sxs-lookup"><span data-stu-id="39f0b-167">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
