---
title: Microsoft 365 İş Ekstra'ya ayarlama
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
description: Etki alanı ve kullanıcı ekleme, güvenlik ilkelerini ayarlama ve daha fazlası dahil olmak üzere Microsoft 365 İş Ekstra için kurulum adımlarını keşfedin.
ms.openlocfilehash: 5b082e78f3dc4067dcce4a96a8088b2347bc3af4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912580"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Kurulum sihirbazında Microsoft 365 İş Ekstra'ya ayarlama

Microsoft 365 İş Ekstra kurulumuna genel bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanınızı, kullanıcılarınızı ekleme ve ilkeleri ayarlama

Microsoft 365 İş Ekstra'ı satın alırken, sahip olduğunuz bir etki alanını kullanma veya kayıt sırasında bir etki alanı [satın alma seçeneğiniz vardır.](sign-up.md)

- Kayıt olurken yeni bir etki alanı satın aldıysanız, etki alanınız ayarlanmıştır ve Kullanıcı ekle'ye geçebilirsiniz [ve lisans atabilirsiniz.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Oturum açmanızı kişiselleştirmek için etki alanınızı ekleme

1. Genel yönetici [kimlik bilgilerinizi kullanarak Microsoft 365](https://admin.microsoft.com) yönetim merkezinde oturum açma. 

2. Sihirbazı **başlatmak için Kuruluma** git'i seçin.

    ![Kuruluma git'i seçin.](../media/gotosetupinadmincenter.png)

3. Office **uygulamalarınızı yükleyin sayfasında,** isteğe bağlı olarak uygulamaları kendi bilgisayarınıza yükleyebilirsiniz.
    
4. Etki alanı **ekle adımlarında,** kullanmak istediğiniz etki alanı adını girin (örneğin, contoso.com).

    > [!IMPORTANT]
    > Kayıt sırasında bir etki alanı satın yaptıysanız, Buraya etki alanı ekle **adımını** görmeyebilirsiniz. Bunun yerine [Kullanıcı ekle'ye](#add-users-and-assign-licenses) gidin.

    ![Oturum açma sayfanızı kişiselleştirin sayfasının ekran görüntüsü.](../media/adddomain.png)

    
4. [Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) için etki alanının sahibinizi doğrulayanın herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için sihirbazda yer alan adımları izleyin. Etki alanı ana nızı biliyorsanız, ana bilgisayarla ilgili [yönergelere de bakın.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Barındırma sağlayıcınız GoDaddy veya etki alanı [](/office365/admin/get-help-with-domains/domain-connect)bağlantısıyla etkinleştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmanız ve Sizin adnıza Microsoft'un kimlik doğrulamasına izin vermeniz istenmektedir.

    ![GoDaddy Erişimi Onayla sayfasında Yetkilendir'i seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Kullanıcı ekleme ve lisans atama

Sihirbaza kullanıcı eklemekle birlikte, kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de eklemeniz de gerekir. Buna ek olarak, yerel bir etki alanı denetleyiciniz [varsa, Azure AD Connect'i olan kullanıcıları ekleyebilirsiniz.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Sihirbaza kullanıcı ekleme

Sihirbaza ekley istediğiniz kullanıcılara otomatik olarak bir Microsoft 365 İş Ekstra lisansı atanır.

![Sihirbazda Yeni kullanıcı ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. Microsoft 365 İş Ekstra aboneliğinizin mevcut kullanıcıları varsa (örneğin, Azure AD Connect kullandınız), bu kullanıcılara şimdi lisans atama seçeneğiniz olur. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

2. Kullanıcıları ekledikten sonra, kimlik bilgilerini kendi ekledikten sonra yeni kullanıcılarla paylaşma seçeneği de elde olur. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> Kullanıcıları ayarlamak için .onmicrosoft etki alanını kullanmayı seçtiy veya Azure AD Connect'i kullandınız, bu adımı görmeyebilirsiniz.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Bunu yoksa, Microsoft [365'i](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirme. 

    - Mevcut DNS kayıtlarınız, örneğin var olan bir web siteniz [](/office365/admin/get-help-with-domains/domain-connect)varsa, ancak ETKI alanı bağlantısı için DNS barındırma etkinleştirilmişse, Kayıtları benim için **ekle'yi seçin.** Çevrimiçi **hizmetlerinizi seçin sayfasında,** tüm varsayılanları kabul edin ve  Sonraki'ni seçin ve DNS barındırma barındırma hizmet nizin sayfasında Yetkilendir'i seçin.
    - Diğer DNS ana bilgisayarlarında mevcut DNS kayıtlarınız varsa (etki alanı bağlantısı için etkin değil), mevcut hizmetlerin bağlı kalacağından emin olmak için kendi DNS kayıtlarınızı yönetmek istemeniz gerekir. Daha [fazla bilgi için etki alanı](/office365/admin/get-help-with-domains/dns-basics) temel bilgilerine bakın.

        ![Kayıtları etkinleştirme sayfası.](../media/activaterecords.png)

2. Sihirbazda adımları izleyin; e-posta ve diğer hizmetler sizin için ayarlanır.

### <a name="protect-your-organization"></a>Organizasyonlarınızı koruyun 

Sihirbazda ayarlanıyor olan ilkeler, Tüm Kullanıcılar adlı [Güvenlik grubuna otomatik](/office365/admin/create-groups/compare-groups#security-groups) olarak *uygulanır.* Ayrıca, yönetim merkezinde ilke atamak için ek gruplar da oluşturabilirsiniz.

1. Gelişmiş siber **tehditlere karşı** korumayı artırarak, [Office 365'in](../security/office-365-security/office-365-atp.md) Tehdit Koruması'nın Office uygulamalarına dosya ve bağlantı taramasına izin verme varsayılanlarını kabul etmenizi öneririz.

    ![Korumayı artır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. Hassas veri **sızıntılarını** önle sayfasında, Office uygulamaları içinde hassas verileri izlemek ve bunların kuruluş dışında yanlışlıkla paylaşımını önlemek için Office 365 Veri Kaybı Önleme'nin (DLP) varsayılanlarını kabul edin.

3. Mobil cihazlar **için Office'te** verileri koru sayfasında, mobil uygulama yönetimini açık bırakın, ayarları genişletin ve gözden geçirin ve ardından Mobil uygulama **yönetimi ilkesi oluştur'a tıklayın.**

    ![Mobil için Office sayfasındaki verileri koru sayfasının ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10 bilgisayarlarında güvenlik sağlama

Sol gezintide Kurulum'u **seçin** ve ardından Oturum açma ve güvenlik altında Windows **10** bilgisayarlarınızı güvenli hale seçin. Başlamak **için** Görüntüle'yi seçin. Eksiksiz [yönergeler için Windows 10 bilgisayarlarınızı](secure-win-10-pcs.md) güvenli hale bakın.

## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamalarını dağıtma

Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi tercih edersiniz, kullanıcılar Windows cihazlarından Azure AD'de oturum açmaları için iş kimlik bilgilerini kullanarak Windows 10 cihazlarına yüklenir.

Office'i mobil iOS veya Android cihazlara yüklemek için Bkz. [Microsoft 365 İş Ekstra](set-up-mobile-devices.md)kullanıcıları için mobil cihazları ayarlama.

Office'i tek tek de yükleyebilirsiniz. Yönergeler [için BKZ. PC veya Mac bilgisayara Office](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) yükleme.

## <a name="see-also"></a>Ayrıca bkz.

[İş için Microsoft 365 eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)