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
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Kur Sihirbazı'nda Microsoft 365 işletmeniz ayarlama

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanı, kullanıcılar, ekleme ve ilkelerini kurun

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Microsoft 365 iş satın aldığınızda, size ait olan bir etki alanı kullanarak ya da sırasında satın seçeneğiniz [Kaydolma](sign-up.md).

- Siz oturum açtığınızda yeni bir etki alanı satın aldıysanız, etki alanınızın tüm yedekleme kümesidir ve [lisanslar atayabilir ve kullanıcıları eklemek](#add-users-and-assign-licenses)için taşıyabilirsiniz.

### <a name="add-your-domain-to-personalize-sign-in"></a>Oturum kişiselleştirmek için etki alanı ekleme

1. [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) genel yönetici kimlik bilgilerinizi kullanarak oturum açın. 

2. **Ekle bir etki alanı** veya **Kullanıcı Ekle** Sihirbazı'nı başlatmak için seçin.
    > [!IMPORTANT]
    > Kayıt sırasında bir etki alanı satın aldıysanız, değil bkz: **etki alanı eklemek** adım burada olur. Bunun yerine, [Kullanıcı Ekle](#add-users-and-assign-licenses) gidin.

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

![Ekle yeni kullanıcılar Sayfa Sihirbazı'nda ekran görüntüsü](media/addnewuserspage.png)

1. Varolan kullanıcıların (örneğin, Azure AD Connect kullandıysanız) Microsoft 365 iş aboneliğiniz varsa, lisansları şimdi onlara atamak için bir seçenek alın. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

3. Kullanıcıları ekledikten sonra kimlik bilgileri eklediğiniz yeni kullanıcıları ile paylaşmak için bir seçenek de alırsınız. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

4. E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin. 

    Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.


### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> .Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Connect kullanıcıları ayarlamak için kullanılan, bu adımı göremez.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Varolan bir web sitesi gibi varolan DNS kayıtları varsa, varolan Hizmetleri bağlı kalmak emin olmak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz. [Etki alanı temelleri](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) daha fazla bilgi için bkz.

        ![Etki alanınızı Bağlan sayfası ben kendi DNS kayıtlarını yönetmek.](media/connectyourdomainpage.png)

2. Sihirbazı'ndaki adımları izleyin ve e-posta ve diğer hizmetleri sizin için ayarlanır.

### <a name="set-up-security-policies-and-device-configurations"></a>Güvenlik ilkeleri ve aygıt yapılandırmaları ayarlama 

Sihirbazda ayarladığınız ilkeleri *Tüm kullanıcıları*adlı bir [güvenlik grubu](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır. Yönetim Merkezi için ilkeleri atamak için ek grupları da oluşturabilirsiniz.

1. **Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** **mobil cihazlarda iş dosyalarınızı korumak** üzerinde seçeneği varsayılan olarak seçilidir. **Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek**bırakma seçeneği vardır ve bu önerilir.

    ![Mobil aygıtlar sayfasında, ekran görüntüsü korumaya çalışma dosyaları.](media/protectworkfilesondevices.png)

     - **Çalışma dosyaları koruma aygıtları kaybolur veya çalınırsa,** [varsayılan değerleri](protect-work-files-on-lost-or-stolen-device.md)görüntülemek için genişlet:

        ![Ekran görüntüsü aygıtlarında kayıp dosyaları korumak için varsayılan değerler.](media/protectworkfilesondevicesdefault.png)

    - **Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini Yönet** ' i seçin ve [varsayılan değerlerini](manage-user-access-on-mobile-devices.md)görüntülemek için genişletin. Android, IOS ve Windows 10 uygulama ilkeleri oluşturmak için Kurulum sırasında tüm kullanıcılar için geçerli varsayılan değerleri kabul etmenizi öneririz. Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.

        ![Mobile Office dosyaları için koruma ayarları ekran görüntüsü.](media/useraccessonmobile.png)

2. Son adımda, veri koruma ve aygıtları Windows 10 aygıtlar güvenli hale getirmek için ilkeler ayarlamanıza olanak sağlar. Kuruluşunuzda bir kullanıcının Windows 10 bağlandığında, bu ayarları otomatik olarak uygulanır. **Güvenli Windows 10 aygıtları** görmek ve [varsayılan değerlerini](secure-windows-10-devices.md)değiştirmek için genişletebilirsiniz.
3. Windows 10 cihazlarda [Office otomatik olarak yüklemek](install-office-on-windows-10-during-setup.md) için seçebilirsiniz.

    ![Ekran görüntüsünü Windows 10 aygıt yapılandırma sayfası ayarlayın.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamaları dağıtma

Otomatik olarak yedekleme kümesi sırasında Office uygulamaları yüklemek seçerseniz, kullanıcılar için Azure AD iş kimlik bilgilerini Windows aygıtlarına gelen oturum açtıktan sonra Windows 10 aygıtlarda apps yükleyecektir.
Office mobile IOS veya Android aygıtları yüklemek için [Microsoft 365 iş kullanıcıları için mobil aygıtları ayarlayın](set-up-mobile-devices.md)bkz.

Office ayrı olarak da yükleyebilirsiniz. [Bir PC veya Mac Office yükleme](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) yönergeleri için bkz.
