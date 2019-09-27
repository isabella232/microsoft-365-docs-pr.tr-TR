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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business'ı nasıl ayarlayın öğrenin.
ms.openlocfilehash: d33839693001f36fbb56541775015f739300b043
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288505"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Kurulum sihirbazında Microsoft 365 Business'ı ayarlama

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanınızı, kullanıcılarınızı ekleyin ve ilkeler ayarlayın

[![Yönetici merkezinin değiştiğini bildirmek için etiket ve aka.ms/aboutM365preview daha fazla ayrıntı bulabilirsiniz.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Microsoft 365 Business'ı satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında bir etki alanı satın alma seçeneğiniz vardır.

- Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınız tamamen ayarlanmıştır ve [kullanıcı ekle'ye taşınabilir ve lisans atayabilirsiniz.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Oturum açma'yı kişiselleştirmek için etki alanınızı ekleyin

1. Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 yönetici merkezinde](https://admin.microsoft.com) oturum açın. 

2. Sihirbazı başlatmak için **etki alanı ekle** veya kullanıcı **ekle'yi** seçin.
    > [!IMPORTANT]
    > Kayıt sırasında bir etki alanı satın aldıysanız, burada **bir etki alanı** adımı ekle'yi görmezsiniz. Bunun yerine [Kullanıcı Ekle'ye](#add-users-and-assign-licenses) gidin.

    ![Etki alanı ekle'yi seçin.](media/addadomainadmincenter.png)
    
3. Sihirbazda, kullanmak istediğiniz alan adını girin (contoso.com gibi).


    ![Oturum açma sayfanızı Kişiselleştir'in ekran görüntüsü.](media/personalizesignin.png)

    
4. Etki alanına sahip olduğunuzu doğrulayan [Office 365 için herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sihirbazdaki adımları izleyin. Etki alanı ana bilgisayarınızı tanıyorsanız, [ana bilgisayara özel yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)de bakın.

    Barındırma sağlayıcınız GoDaddy veya [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yla etkin leştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmanız ve Microsoft'un sizin adınıza kimlik doğrulamasına izin vermeniz istenir:

    ![GoDaddy Access'i Onayla sayfasında Yetkilendirme'yi seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Kullanıcı ekleme ve lisans atama

Sihirbaza kullanıcı ekleyebilirsiniz, ancak daha sonra yönetici merkezine [de ekleyebilirsiniz.](add-users-m365b.md) Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect'e](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)sahip kullanıcılar ekleyebilirsiniz.

#### <a name="add-users-in-the-wizard"></a>Sihirbaza kullanıcı ekleme

Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak microsoft 365 Business lisansı atanabilir.

![Sihirbazda yeni kullanıcı ekle sayfasının ekran görüntüsü](media/addnewuserspage.png)

1. Microsoft 365 Business aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect'i kullandıysanız) artık onlara lisans atama seçeneğine sahip olabilirsiniz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

3. Kullanıcıları ekledikten sonra, eklediğiniz yeni kullanıcılarla kimlik bilgilerini paylaşma seçeneği de alırsınız. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

4. E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin. 

    Başka bir e-posta sağlayıcısından taşınıyorsanız ve verilerinizi daha sonra kopyalamak istiyorsanız, [e-posta ve kişileri Office 365'e geçirebilirsiniz.](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)


### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> .onmicrosoft etki alanını kullanmayı seçtiyseniz veya kullanıcıları ayarlamak için Azure AD Connect'i kullandıysanız, bu adımı görmezsiniz.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Yoksa, [office 365'i herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirin.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2) 

    - Varolan DNS kayıtlarınız varsa, örneğin varolan bir web sitesi, ancak [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için DNS ana bilgisayarınız etkinse, benim için kayıt **ekle'yi**seçin. 
    - Diğer DNS ana bilgisayarlarıyla varolan DNS kayıtlarınız varsa (etki alanı bağlantısı için etkinleştirilmez), varolan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek istersiniz. Daha fazla bilgi için [etki alanı temellerine](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bakın.

        ![Etki alanı sayfanızı kendi DNS kayıtlarımı yönetirim.](media/connectyourdomainpage.png)

2. Sihirbazve e-posta ve diğer hizmetler adımları izleyin sizin için ayarlanır.

### <a name="set-up-security-policies-and-device-configurations"></a>Güvenlik ilkeleri ve aygıt yapılandırmaları ayarlama 

Sihirbazda ayarladığınız *ilkeler, Tüm Kullanıcılar*adlı bir [Güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır. Ayrıca, yönetici merkezinde ilkeler atamak için ek gruplar oluşturabilirsiniz.

1. Mobil **cihazlardaki iş dosyalarınızı koru** **seçeneği, aygıtlar kaybolduğunda veya çalındığında iş dosyalarını koruyun** seçeneği varsayılan olarak seçilir. **Kullanıcıların mobil cihazlardaki Office dosyalarına nasıl erişirlerini yönet'i**açma seçeneğiniz vardır ve bu önerilir.

    ![Mobil cihazlar sayfasındaki çalışma dosyalarını koru ekran görüntüsü.](media/protectworkfilesondevices.png)

     - **Aygıtlar kaybolduğunda veya çalındığında varsayılan** [değerleri](protect-work-files-on-lost-or-stolen-device.md)görüntülemek için iş dosyalarını koruyun'u genişletin:

        ![Kayıp aygıtlarda dosyaları korumak için varsayılan değerlerin ekran görüntüsü.](media/protectworkfilesondevicesdefault.png)

    - **Kullanıcıların mobil cihazlardaki Office dosyalarına nasıl eriştürün** ünü yönet'i seçin ve varsayılan [değerleri](manage-user-access-on-mobile-devices.md)görüntülemek için genişletin. Tüm kullanıcılar için geçerli olan Android, iOS ve Windows 10 için uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz. Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.

        ![Mobil cihazlardaki Office dosyaları için koruma ayarlarının ekran görüntüsü.](media/useraccessonmobile.png)

2. Verileri ve aygıtları koruma konusundaki son adım, Windows 10 aygıtlarını korumak için ilkeler ayarlamanıza olanak tanır. Bu ayarlar, bir kullanıcının Windows 10'u kuruluşunuza bağlandığında otomatik olarak uygulanır. [Varsayılan değerleri](secure-windows-10-devices.md)görmek ve değiştirmek için Güvenli **Windows 10 aygıtlarını** genişletebilirsiniz.
3. Office'i Windows 10 aygıtlarına [otomatik olarak yüklemeyi](install-office-on-windows-10-during-setup.md) de seçebilirsiniz.

    ![Set Windows 10 aygıt yapılandırma sayfasının ekran görüntüsü.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamalarını dağıtma

Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar windows aygıtlarından Iş kimlik bilgileriyle Azure AD'ye oturum açtıktan sonra uygulamalar Windows 10 cihazlarına yüklenir.
Office'i mobil iOS veya Android cihazlara yüklemek [için](set-up-mobile-devices.md)bkz.

Office'i tek tek yükleyebilirsiniz. Talimatlar için [Office'i pc'ye veya Mac'e yükleyin'](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) e bakın.
