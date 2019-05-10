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
# <a name="set-up-microsoft-365-business"></a>Microsoft 365 Business'ı ayarlama

Başlamadan önce [Microsoft 365 iş almak](get-microsoft-365-business.md) için kayıt ayrıntıları bakın.

Sihirbaz yedekleme ve şirket içi Active Directory olmadığında kümesini kullanarak [Microsoft 365 iş ayarlanması hakkında kısa video](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) izlemek
  

## <a name="overview"></a>Genel Bakış

Kurulum sihirbazındaki adımları ayarlamak çoğu yapılabilir, ancak diğer seçenekler de listelenir.

1. [Etki alanınızın Ekle](#add-your-domain-to-personalize-sign-in) ( [kayıt](sign-up.md)sırasında etki alanı satın aldıysanız, bu adımı zaten yapılır.)
2. Kullanıcıları ekleyin. Herhangi üç yoldan biriyle yapabilirsiniz:
    - [Kur Sihirbazı](#add-users-in-the-wizard)' nda.
    - Eğer yerinde Active directory directory eşitlemesi [Azure AD Connect kullanarak kullanıcı eklemek](#add-users-by-using-azure-ad-connect) için kullanın.
    - [Daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de kullanabilirsiniz.
3. Güvenlik ilkelerini kurun ve aygıtları yapılandırma. Herhangi üç yoldan biriyle yapabilirsiniz:
    - [Kur Sihirbazı](#set-up-policies-in-the-wizard)' nda.  
    - [Yönetim Merkezi](#modify-or-add-policies-in-the-admin-center).
    - [Intune Yönetim Merkezi](https://docs.microsoft.com/intune/what-is-device-management).
4. Kurma ve Windows 10 aygıtları yönetme.

    WIndows 10 aygıt için Azure AD katıldığınızda, tüm ilkeleri, uygulanan.
    - [Kurulum Sihirbazı](#set-up-policies-in-the-wizard)Windows 10 aygıt yapılandırmalarını ayarlayın.
    - [Yeni Windows 10 aygıt](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD için katılın.
    - Bir [Varolan Windows 10 aygıt](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) Azure AD için katılın.
1. Office 365 iş yükleyin.
    - [Kurulum Sihirbazı](#set-up-policies-in-the-wizard)' nı kullanarak Windows aygıtlardan Office otomatik olarak yükleyebilir.
    - Otomatik olarak [Office yükleme](auto-install-or-uninstall-office.md) Yönetim Merkezi'nden.
    - Kullanıcıların [Office uygulamaları yüklemek](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows ve aygıtlar için olanak sağlar.
     
1. Ek güvenlik ayarlarını ayarlayın.
    - Kurulum Sihirbazı'nı aygıtlarınızın güvenliğini sağlamak için ilkeler ekler ancak [ek güvenlik](#additional-security-settings) yeteneklerinden güvenli yardımcı olur, veri, hesapları ve e-postaları alabilir. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanı, kullanıcı eklemek ve ilkelerini kurun

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Microsoft 365 iş satın aldığınızda, size ait olan bir etki alanı kullanarak ya da sırasında satın seçeneğiniz [Kaydolma](sign-up.md).

- Siz oturum açtığınızda yeni bir etki alanı satın aldıysanız, etki alanınızın tüm yedekleme kümesidir ve [lisanslar atayabilir ve kullanıcıları eklemek](#add-users-and-assign-licenses)için taşıyabilirsiniz.

### <a name="add-your-domain-to-personalize-sign-in"></a>Oturum kişiselleştirmek için etki alanı ekleme

1. [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) genel yönetici kimlik bilgilerinizi kullanarak oturum açın. 

2. **Bir etki alanı Ekle** Sihirbazı'nı başlatmak için seçin.

    ![Bir etki alanına Ekle'yi seçin.](media/addadomainadmincenter.png)
    
3. Sihirbazda, (contoso.com gibi) kullanmak istediğiniz etki alanı adını girin.


    ![Oturum açma sayfası kişiselleştirme ekran görüntüsü.](media/personalizesignin.png)

    
4. Doğrulayan etki alanı sahibi [herhangi bir DNS barındırma sağlayıcı için Office 365 oluşturmak DNS kayıtları](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) için sihirbazdaki adımları izleyin. Ayrıca, etki alanı ana biliyorsanız, [ana bilgisayar belirli yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)bakın.

    GoDaddy barındırma sağlayıcınıza ise, kolay bir işlemdir ve sizden oturum açıp Microsoft'un sizin adınıza kimliğini otomatik olarak istenecektir:

    ![GoDaddy erişimi Onayla sayfasında, Authorize seçeneğini seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Kullanıcı ekleme ve lisans atama

Sihirbazda kullanıcılar ekleyebilirsiniz, ancak [daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de olabilir. Ayrıca, yerel etki alanı denetleyicisi varsa, [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ile kullanıcılar ekleyebilirsiniz.

#### <a name="add-users-in-the-wizard"></a>Kullanıcı Ekleme Sihirbazı'nda

Sihirbazda eklediğiniz kullanıcılar Microsoft 365 işletme lisans otomatik olarak atanan.
[Azure AD Connect kullanarak ggg kullanıcılara](#add-users-by-using-azure-ad-connect)yerel etki alanı denetleyicisi varsa ve Active Directory kullanıyorsanız, bkz.

![Ekle yeni kullanıcılar Sayfa Sihirbazı'nda ekran görüntüsü](media/addnewuserspage.png)

1. Microsoft 365 İş aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect kullandıysanız), bu kullanıcılara hemen lisans atamanızı sağlayan bir seçenek görürsünüz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

3. Kullanıcıları ekledikten sonra kimlik bilgileri eklediğiniz yeni kullanıcıları ile paylaşmak için bir seçenek de alırsınız. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

4. E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin. 

    Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.

#### <a name="add-users-by-using-azure-ad-connect"></a>Azure AD Connect kullanarak kullanıcıları ekleyin.

 Active Directory ile yerel etki alanı denetleyiciniz varsa, kullanıcılarınızın Microsoft 365 iş [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)kullanarak eşitleyin. Kurulum Sihirbazı'nı başlatmadan önce bunu tamamlayın. Yönetim Merkezi'nde yükleyebilirsiniz:

- **Kullanıcılar** Git \> **Etkin kullanıcılar**, sayfanın en üstündeki elips seçin ve sonra **dizin eşitleme** Azure AD Connect karşıdan yüklemek için seçin.

    ![Etkin Kullanıcılar sayfasında ellipses > Directory snchronization seçin.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Bu şekilde kullanıcılar oluşturursanız, lisans Yönetim Merkezi'nde atayabilirsiniz gerekecektir.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Etki alanına katılmış apps ve aygıtları erişmeye devam

Apps etki alanına katılmış ve aygıtları erişmeye devam etmek istiyorsanız, iki farklı şekilde, etkinleştirme için aşağıdaki makaleleri okuyun:
  
- [Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme](manage-windows-devices.md)
    - Bu, önerilen yoldur.

- [Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları](access-resources.md)

### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> .Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Connect kullanıcıları ayarlamak için kullanılan, bu adımı göremez.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Varolan bir web sitesi gibi varolan DNS kayıtları varsa, varolan Hizmetleri bağlı kalmak emin olmak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz. [Etki alanı temelleri](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) daha fazla bilgi için bkz.

        ![Etki alanınızı Bağlan sayfası ben kendi DNS kayıtlarını yönetmek.](media/connectyourdomainpage.png)

2. Sihirbazı'ndaki adımları izleyin ve e-posta ve diğer hizmetleri sizin için ayarlanır.

### <a name="set-up-security-policies-and-device-configurations"></a>Güvenlik ilkeleri ve aygıt yapılandırmaları ayarlama 

Bu ilkeler her kullanıcı için geçerli bir kullanıcı kümesi için farklı ilkeler atamak karar verirseniz, bir lisans veya bir kullanıcı grubu için verin.

#### <a name="set-up-policies-in-the-wizard"></a>Sihirbazdaki ilkeleri ayarlama

Sihirbazda ayarladığınız ilkeleri *Tüm kullanıcıları*adlı bir [güvenlik grubu](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır.

1. **Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** **mobil cihazlarda iş dosyalarınızı korumak** üzerinde seçeneği varsayılan olarak seçilidir. **Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek**bırakma seçeneği vardır ve bu önerilir.

    ![Mobil aygıtlar sayfasında, ekran görüntüsü korumaya çalışma dosyaları.](media/protectworkfilesondevices.png)

     - **Aygıtları kaybolur veya çalınırsa, koruma çalışma dosyaları**' nı genişletin, [varsayılan değerleri](protect-work-files-on-lost-or-stolen-device.md) önceden seçilen şunlardır:

        ![Ekran görüntüsü aygıtlarında kayıp dosyaları korumak için varsayılan değerler.](media/protectworkfilesondevicesdefault.png)

    - **Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek** seçip genişletin, [varsayılan değerleri](manage-user-access-on-mobile-devices.md) gösterilir. Android, iOS ve Windows 10 için tüm kullanıcılar için geçerli olan uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz. Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.

        ![Mobile Office dosyaları için koruma ayarları ekran görüntüsü.](media/useraccessonmobile.png)

2. Son adımda, veri koruma ve aygıtları Windows 10 aygıtlar güvenli hale getirmek için ilkeler ayarlamanıza olanak sağlar. Kuruluşunuzda bir kullanıcının Windows 10 bağlandığında, bu ayarları otomatik olarak uygulanır. **Güvenli Windows 10 aygıtları** görmek ve [varsayılan değerlerini](secure-windows-10-devices.md)değiştirmek için genişletebilirsiniz.
3. Windows 10 cihazlarda [Office otomatik olarak yüklemek](install-office-on-windows-10-during-setup.md) için seçebilirsiniz.

    ![Ekran görüntüsünü Windows 10 aygıt yapılandırma sayfası ayarlayın.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Değiştirme veya Yönetim Merkezi'nde ilkeleri ekleme

İlkeleri görüntülemek ve aygıt ve uygulama koruması değiştirmek nasıl konulara bağlantılar için bkz: [Microsoft 365 iş yönetme](manage.md) ve nasıl verilerinden kaldırabilir veya kullanıcı aygıtı sıfırlayın.

## <a name="deploy-and-manage-windows-10"></a>Dağıtmak ve yönetmek Windows 10
Azure AD, varolan bilgisayarlarda oturum profilini değiştirerek veya yeni bilgisayarlar için Kurulum sırasında ya da el ile bağlanmak için [Microsoft 365 iş kullanıcıları için Windows aygıt ayarlama](set-up-windows-devices.md) konusuna bakın. 

### <a name="use-autopilot-to-set-up-new-devices"></a>Yeni aygıtları için AutoPilot kullanın

[Windows Autopilot](add-autopilot-devices-and-profile.md) otomatik olarak **Yeni** bir kullanıcı Windows 10 aygıtları önceden yapılandırmak için kullanabilirsiniz, ancak sizin için bunu yapmak için bir [ortak](https://www.microsoft.com/solution-providers/search) almak daha kolay olabilir. [Microsoft mağaza](https://go.microsoft.com/fwlink/?linkid=874598) ve yeni aygıtlar için satın bir bulut teknoloji uzmanı ayarlamak isteyin.

### <a name="access-on-premises-resources"></a>Şirket içi kaynaklara erişmek

Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz. Bunu ayarlamak için [Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış Windows 10 aygıtları etkinleştirme](manage-windows-devices.md) adımlarını izleyin. Tercih edilen yöntem budur ve bu durumda aygıtları karma Azure adı verilen AD alanına bağlı aygıtlar.

Bazı içeren Active Directory yerinde kaynaklar (örneğin, dosya paylaşımları ve yazıcılar), bu kaynakların Azure AD alanına bağlı aygıtlara erişiminizi burada adımları izleyerek verebilirsiniz İşletmenizde yerel varsa: [erişim şirket içi kaynaklardan bir 365 işletmede Azure AD alanına bağlı aygıt](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamaları dağıtma

Otomatik olarak yedekleme kümesi sırasında Office uygulamaları yüklemek seçerseniz, kullanıcılar için Azure AD iş kimlik bilgilerini Windows aygıtlarına gelen oturum açtıktan sonra Windows 10 aygıtlarda apps yükleyecektir.
Office mobile IOS veya Android aygıtları yüklemek için [Microsoft 365 iş kullanıcıları için mobil aygıtları ayarlayın](set-up-mobile-devices.md)bkz.

Office ayrı olarak da yükleyebilirsiniz. [Bir PC veya Mac Office yükleme](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) yönergeleri için bkz.

## <a name="additional-security-settings"></a>Ek güvenlik ayarları

Güvenlik ve Kurulum Sihirbazı'ndaki Uyumluluk ayarına ek olarak, aşağıdaki ek ayarlar de ayarlayabilirsiniz:
  
- **E-posta zararlı yazılımlara karşı koruma**
- **Gelişmiş tehdit Koruması (ATP) güvenli ekler**
- **ATP güvenli bağlantılar**
- **APT anti-phishing**
- **Exchange Online Arşivleme**
- **Veri kaybını önleme (DLP)**
- **Azure bilgi koruma** (Plan 1)
- **Intune portal kullanılabilirliği**

Almak için bkz: [Gelişmiş güvenlik ilkelerini kurun](set-up-advanced-security.md)başladı.

Ayrıca bkz: [Microsoft 365 işletmenizin güvenliğini sağlamak için üst 10 yolu](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) için bir yol haritası, en iyi güvenlik yöntemleri.