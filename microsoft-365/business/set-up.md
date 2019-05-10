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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660919"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="50fac-103">Microsoft 365 Business'ı ayarlama</span><span class="sxs-lookup"><span data-stu-id="50fac-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="50fac-104">Başlamadan önce [Microsoft 365 iş almak](get-microsoft-365-business.md) için kayıt ayrıntıları bakın.</span><span class="sxs-lookup"><span data-stu-id="50fac-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="50fac-105">Sihirbaz yedekleme ve şirket içi Active Directory olmadığında kümesini kullanarak [Microsoft 365 iş ayarlanması hakkında kısa video](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) izlemek</span><span class="sxs-lookup"><span data-stu-id="50fac-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="50fac-106">Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="50fac-106">Overview</span></span>

<span data-ttu-id="50fac-107">Kurulum sihirbazındaki adımları ayarlamak çoğu yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="50fac-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="50fac-108">[Etki alanınızın Ekle](#add-your-domain-to-personalize-sign-in) ( [kayıt](sign-up.md)sırasında etki alanı satın aldıysanız, bu adımı zaten yapılır.)</span><span class="sxs-lookup"><span data-stu-id="50fac-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="50fac-109">Kullanıcıları ekleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-109">Add users.</span></span> <span data-ttu-id="50fac-110">Herhangi üç yoldan biriyle yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="50fac-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="50fac-111">[Kur Sihirbazı](#add-users-in-the-wizard)' nda.</span><span class="sxs-lookup"><span data-stu-id="50fac-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="50fac-112">Eğer yerinde Active directory directory eşitlemesi [Azure AD Connect kullanarak kullanıcı eklemek](#add-users-by-using-azure-ad-connect) için kullanın.</span><span class="sxs-lookup"><span data-stu-id="50fac-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="50fac-113">[Daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="50fac-114">Güvenlik ilkelerini kurun ve aygıtları yapılandırma.</span><span class="sxs-lookup"><span data-stu-id="50fac-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="50fac-115">Herhangi üç yoldan biriyle yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="50fac-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="50fac-116">[Kur Sihirbazı](#set-up-policies-in-the-wizard)' nda.</span><span class="sxs-lookup"><span data-stu-id="50fac-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="50fac-117">[Yönetim Merkezi](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="50fac-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="50fac-118">[Intune Yönetim Merkezi](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="50fac-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="50fac-119">Kurma ve Windows 10 aygıtları yönetme.</span><span class="sxs-lookup"><span data-stu-id="50fac-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="50fac-120">WIndows 10 aygıt için Azure AD katıldığınızda, tüm ilkeleri, uygulanan.</span><span class="sxs-lookup"><span data-stu-id="50fac-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="50fac-121">[Kurulum Sihirbazı](#set-up-policies-in-the-wizard)Windows 10 aygıt yapılandırmalarını ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="50fac-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="50fac-122">[Yeni Windows 10 aygıt](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD için katılın.</span><span class="sxs-lookup"><span data-stu-id="50fac-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="50fac-123">Bir [Varolan Windows 10 aygıt](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) Azure AD için katılın.</span><span class="sxs-lookup"><span data-stu-id="50fac-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="50fac-124">Office 365 iş yükleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="50fac-125">[Kurulum Sihirbazı](#set-up-policies-in-the-wizard)' nı kullanarak Windows aygıtlardan Office otomatik olarak yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="50fac-126">Otomatik olarak [Office yükleme](auto-install-or-uninstall-office.md) Yönetim Merkezi'nden.</span><span class="sxs-lookup"><span data-stu-id="50fac-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="50fac-127">Kullanıcıların [Office uygulamaları yüklemek](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows ve aygıtlar için olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="50fac-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="50fac-128">Ek güvenlik ayarlarını ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="50fac-128">Set up additional security.</span></span>
    - <span data-ttu-id="50fac-129">Kurulum Sihirbazı'nı aygıtlarınızın güvenliğini sağlamak için ilkeler ekler ancak [ek güvenlik](#additional-security-settings) yeteneklerinden güvenli yardımcı olur, veri, hesapları ve e-postaları alabilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="50fac-130">Etki alanı, kullanıcı eklemek ve ilkelerini kurun</span><span class="sxs-lookup"><span data-stu-id="50fac-130">Add your domain, users and set up policies</span></span>

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="50fac-132">Microsoft 365 iş satın aldığınızda, size ait olan bir etki alanı kullanarak ya da sırasında satın seçeneğiniz [Kaydolma](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="50fac-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="50fac-133">Siz oturum açtığınızda yeni bir etki alanı satın aldıysanız, etki alanınızın tüm yedekleme kümesidir ve [lisanslar atayabilir ve kullanıcıları eklemek](#add-users-and-assign-licenses)için taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="50fac-134">Oturum kişiselleştirmek için etki alanı ekleme</span><span class="sxs-lookup"><span data-stu-id="50fac-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="50fac-135">[Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) genel yönetici kimlik bilgilerinizi kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="50fac-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="50fac-136">**Bir etki alanı Ekle** Sihirbazı'nı başlatmak için seçin.</span><span class="sxs-lookup"><span data-stu-id="50fac-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Bir etki alanına Ekle'yi seçin.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="50fac-138">Sihirbazda, (contoso.com gibi) kullanmak istediğiniz etki alanı adını girin.</span><span class="sxs-lookup"><span data-stu-id="50fac-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Oturum açma sayfası kişiselleştirme ekran görüntüsü.](media/personalizesignin.png)

    
4. <span data-ttu-id="50fac-140">Doğrulayan etki alanı sahibi [herhangi bir DNS barındırma sağlayıcı için Office 365 oluşturmak DNS kayıtları](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) için sihirbazdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="50fac-141">Ayrıca, etki alanı ana biliyorsanız, [ana bilgisayar belirli yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)bakın.</span><span class="sxs-lookup"><span data-stu-id="50fac-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="50fac-142">GoDaddy barındırma sağlayıcınıza ise, kolay bir işlemdir ve sizden oturum açıp Microsoft'un sizin adınıza kimliğini otomatik olarak istenecektir:</span><span class="sxs-lookup"><span data-stu-id="50fac-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy erişimi Onayla sayfasında, Authorize seçeneğini seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="50fac-144">Kullanıcı ekleme ve lisans atama</span><span class="sxs-lookup"><span data-stu-id="50fac-144">Add users and assign licenses</span></span>

<span data-ttu-id="50fac-145">Sihirbazda kullanıcılar ekleyebilirsiniz, ancak [daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de olabilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="50fac-146">Ayrıca, yerel etki alanı denetleyicisi varsa, [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ile kullanıcılar ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="50fac-147">Kullanıcı Ekleme Sihirbazı'nda</span><span class="sxs-lookup"><span data-stu-id="50fac-147">Add users in the wizard</span></span>

<span data-ttu-id="50fac-148">Sihirbazda eklediğiniz kullanıcılar Microsoft 365 işletme lisans otomatik olarak atanan.</span><span class="sxs-lookup"><span data-stu-id="50fac-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="50fac-149">[Azure AD Connect kullanarak ggg kullanıcılara](#add-users-by-using-azure-ad-connect)yerel etki alanı denetleyicisi varsa ve Active Directory kullanıyorsanız, bkz.</span><span class="sxs-lookup"><span data-stu-id="50fac-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Ekle yeni kullanıcılar Sayfa Sihirbazı'nda ekran görüntüsü](media/addnewuserspage.png)

1. <span data-ttu-id="50fac-p106">Microsoft 365 İş aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect kullandıysanız), bu kullanıcılara hemen lisans atamanızı sağlayan bir seçenek görürsünüz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.</span><span class="sxs-lookup"><span data-stu-id="50fac-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="50fac-153">Kullanıcıları ekledikten sonra kimlik bilgileri eklediğiniz yeni kullanıcıları ile paylaşmak için bir seçenek de alırsınız.</span><span class="sxs-lookup"><span data-stu-id="50fac-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="50fac-154">Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="50fac-155">E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="50fac-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="50fac-156">Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="50fac-157">Azure AD Connect kullanarak kullanıcıları ekleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="50fac-158">Active Directory ile yerel etki alanı denetleyiciniz varsa, kullanıcılarınızın Microsoft 365 iş [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)kullanarak eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="50fac-159">Kurulum Sihirbazı'nı başlatmadan önce bunu tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="50fac-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="50fac-160">Yönetim Merkezi'nde yükleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="50fac-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="50fac-161">**Kullanıcılar** Git \> **Etkin kullanıcılar**, sayfanın en üstündeki elips seçin ve sonra **dizin eşitleme** Azure AD Connect karşıdan yüklemek için seçin.</span><span class="sxs-lookup"><span data-stu-id="50fac-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Etkin Kullanıcılar sayfasında ellipses > Directory snchronization seçin.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="50fac-163">Bu şekilde kullanıcılar oluşturursanız, lisans Yönetim Merkezi'nde atayabilirsiniz gerekecektir.</span><span class="sxs-lookup"><span data-stu-id="50fac-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="50fac-164">Etki alanına katılmış apps ve aygıtları erişmeye devam</span><span class="sxs-lookup"><span data-stu-id="50fac-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="50fac-165">Apps etki alanına katılmış ve aygıtları erişmeye devam etmek istiyorsanız, iki farklı şekilde, etkinleştirme için aşağıdaki makaleleri okuyun:</span><span class="sxs-lookup"><span data-stu-id="50fac-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="50fac-166">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="50fac-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="50fac-167">Bu, önerilen yoldur.</span><span class="sxs-lookup"><span data-stu-id="50fac-167">This is the recommended way.</span></span>

- [<span data-ttu-id="50fac-168">Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları</span><span class="sxs-lookup"><span data-stu-id="50fac-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="50fac-169">Etki alanınızı bağlama</span><span class="sxs-lookup"><span data-stu-id="50fac-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="50fac-170">.Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Connect kullanıcıları ayarlamak için kullanılan, bu adımı göremez.</span><span class="sxs-lookup"><span data-stu-id="50fac-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="50fac-171">Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="50fac-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="50fac-172">Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir.</span><span class="sxs-lookup"><span data-stu-id="50fac-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="50fac-173">Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="50fac-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="50fac-174">Varolan bir web sitesi gibi varolan DNS kayıtları varsa, varolan Hizmetleri bağlı kalmak emin olmak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="50fac-175">[Etki alanı temelleri](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="50fac-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Etki alanınızı Bağlan sayfası ben kendi DNS kayıtlarını yönetmek.](media/connectyourdomainpage.png)

2. <span data-ttu-id="50fac-177">Sihirbazı'ndaki adımları izleyin ve e-posta ve diğer hizmetleri sizin için ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="50fac-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="50fac-178">Güvenlik ilkeleri ve aygıt yapılandırmaları ayarlama</span><span class="sxs-lookup"><span data-stu-id="50fac-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="50fac-179">Bu ilkeler her kullanıcı için geçerli bir kullanıcı kümesi için farklı ilkeler atamak karar verirseniz, bir lisans veya bir kullanıcı grubu için verin.</span><span class="sxs-lookup"><span data-stu-id="50fac-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="50fac-180">Sihirbazdaki ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="50fac-180">Set up policies in the wizard</span></span>

<span data-ttu-id="50fac-181">Sihirbazda ayarladığınız ilkeleri *Tüm kullanıcıları*adlı bir [güvenlik grubu](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="50fac-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="50fac-182">**Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** **mobil cihazlarda iş dosyalarınızı korumak** üzerinde seçeneği varsayılan olarak seçilidir.</span><span class="sxs-lookup"><span data-stu-id="50fac-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="50fac-183">**Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek**bırakma seçeneği vardır ve bu önerilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Mobil aygıtlar sayfasında, ekran görüntüsü korumaya çalışma dosyaları.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="50fac-185">**Aygıtları kaybolur veya çalınırsa, koruma çalışma dosyaları**' nı genişletin, [varsayılan değerleri](protect-work-files-on-lost-or-stolen-device.md) önceden seçilen şunlardır:</span><span class="sxs-lookup"><span data-stu-id="50fac-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Ekran görüntüsü aygıtlarında kayıp dosyaları korumak için varsayılan değerler.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="50fac-187">**Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek** seçip genişletin, [varsayılan değerleri](manage-user-access-on-mobile-devices.md) gösterilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="50fac-188">Android, iOS ve Windows 10 için tüm kullanıcılar için geçerli olan uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="50fac-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="50fac-189">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-189">You can create more policies after setup completes.</span></span>

        ![Mobile Office dosyaları için koruma ayarları ekran görüntüsü.](media/useraccessonmobile.png)

2. <span data-ttu-id="50fac-191">Son adımda, veri koruma ve aygıtları Windows 10 aygıtlar güvenli hale getirmek için ilkeler ayarlamanıza olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="50fac-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="50fac-192">Kuruluşunuzda bir kullanıcının Windows 10 bağlandığında, bu ayarları otomatik olarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="50fac-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="50fac-193">**Güvenli Windows 10 aygıtları** görmek ve [varsayılan değerlerini](secure-windows-10-devices.md)değiştirmek için genişletebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="50fac-194">Windows 10 cihazlarda [Office otomatik olarak yüklemek](install-office-on-windows-10-during-setup.md) için seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Ekran görüntüsünü Windows 10 aygıt yapılandırma sayfası ayarlayın.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="50fac-196">Değiştirme veya Yönetim Merkezi'nde ilkeleri ekleme</span><span class="sxs-lookup"><span data-stu-id="50fac-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="50fac-197">İlkeleri görüntülemek ve aygıt ve uygulama koruması değiştirmek nasıl konulara bağlantılar için bkz: [Microsoft 365 iş yönetme](manage.md) ve nasıl verilerinden kaldırabilir veya kullanıcı aygıtı sıfırlayın.</span><span class="sxs-lookup"><span data-stu-id="50fac-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="50fac-198">Dağıtmak ve yönetmek Windows 10</span><span class="sxs-lookup"><span data-stu-id="50fac-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="50fac-199">Azure AD, varolan bilgisayarlarda oturum profilini değiştirerek veya yeni bilgisayarlar için Kurulum sırasında ya da el ile bağlanmak için [Microsoft 365 iş kullanıcıları için Windows aygıt ayarlama](set-up-windows-devices.md) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="50fac-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="50fac-200">Yeni aygıtları için AutoPilot kullanın</span><span class="sxs-lookup"><span data-stu-id="50fac-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="50fac-201">[Windows Autopilot](add-autopilot-devices-and-profile.md) otomatik olarak **Yeni** bir kullanıcı Windows 10 aygıtları önceden yapılandırmak için kullanabilirsiniz, ancak sizin için bunu yapmak için bir [ortak](https://www.microsoft.com/solution-providers/search) almak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="50fac-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="50fac-202">[Microsoft mağaza](https://go.microsoft.com/fwlink/?linkid=874598) ve yeni aygıtlar için satın bir bulut teknoloji uzmanı ayarlamak isteyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="50fac-203">Şirket içi kaynaklara erişmek</span><span class="sxs-lookup"><span data-stu-id="50fac-203">Access on-premises resources</span></span>

<span data-ttu-id="50fac-204">Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="50fac-205">Bunu ayarlamak için [Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış Windows 10 aygıtları etkinleştirme](manage-windows-devices.md) adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="50fac-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="50fac-206">Tercih edilen yöntem budur ve bu durumda aygıtları karma Azure adı verilen AD alanına bağlı aygıtlar.</span><span class="sxs-lookup"><span data-stu-id="50fac-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="50fac-207">Bazı içeren Active Directory yerinde kaynaklar (örneğin, dosya paylaşımları ve yazıcılar), bu kaynakların Azure AD alanına bağlı aygıtlara erişiminizi burada adımları izleyerek verebilirsiniz İşletmenizde yerel varsa: [erişim şirket içi kaynaklardan bir 365 işletmede Azure AD alanına bağlı aygıt](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="50fac-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="50fac-208">Office 365 istemci uygulamaları dağıtma</span><span class="sxs-lookup"><span data-stu-id="50fac-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="50fac-209">Otomatik olarak yedekleme kümesi sırasında Office uygulamaları yüklemek seçerseniz, kullanıcılar için Azure AD iş kimlik bilgilerini Windows aygıtlarına gelen oturum açtıktan sonra Windows 10 aygıtlarda apps yükleyecektir.</span><span class="sxs-lookup"><span data-stu-id="50fac-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="50fac-210">Office mobile IOS veya Android aygıtları yüklemek için [Microsoft 365 iş kullanıcıları için mobil aygıtları ayarlayın](set-up-mobile-devices.md)bkz.</span><span class="sxs-lookup"><span data-stu-id="50fac-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="50fac-211">Office ayrı olarak da yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50fac-211">You can also install Office individually.</span></span> <span data-ttu-id="50fac-212">[Bir PC veya Mac Office yükleme](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) yönergeleri için bkz.</span><span class="sxs-lookup"><span data-stu-id="50fac-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="50fac-213">Ek güvenlik ayarları</span><span class="sxs-lookup"><span data-stu-id="50fac-213">Additional security settings</span></span>

<span data-ttu-id="50fac-214">Güvenlik ve Kurulum Sihirbazı'ndaki Uyumluluk ayarına ek olarak, aşağıdaki ek ayarlar de ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="50fac-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="50fac-215">**E-posta zararlı yazılımlara karşı koruma**</span><span class="sxs-lookup"><span data-stu-id="50fac-215">**Email malware protection**</span></span>
- <span data-ttu-id="50fac-216">**Gelişmiş tehdit Koruması (ATP) güvenli ekler**</span><span class="sxs-lookup"><span data-stu-id="50fac-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="50fac-217">**ATP güvenli bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="50fac-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="50fac-218">**APT anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="50fac-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="50fac-219">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="50fac-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="50fac-220">**Veri kaybını önleme (DLP)**</span><span class="sxs-lookup"><span data-stu-id="50fac-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="50fac-221">**Azure bilgi koruma** (Plan 1)</span><span class="sxs-lookup"><span data-stu-id="50fac-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="50fac-222">**Intune portal kullanılabilirliği**</span><span class="sxs-lookup"><span data-stu-id="50fac-222">**Intune portal availability**</span></span>

<span data-ttu-id="50fac-223">Almak için bkz: [Gelişmiş güvenlik ilkelerini kurun](set-up-advanced-security.md)başladı.</span><span class="sxs-lookup"><span data-stu-id="50fac-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="50fac-224">Ayrıca bkz: [Microsoft 365 işletmenizin güvenliğini sağlamak için üst 10 yolu](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) için bir yol haritası, en iyi güvenlik yöntemleri.</span><span class="sxs-lookup"><span data-stu-id="50fac-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>