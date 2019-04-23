---
title: Microsoft 365 Business'ı kurulum sihirbazını kullanarak ayarlama
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
description: Dört adımları izleyerek Microsoft 365 iş kurmayı öğrenin.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283961"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Microsoft 365 Business'ı kurulum sihirbazını kullanarak ayarlama

1-4 aşağıdaki adımları tamamlayın.
  
### <a name="set-up-microsoft-365-business"></a>Microsoft 365 Business'ı ayarlama

Microsoft 365 iş yerinde Active Directory olmadığında ayarlanması hakkında bir video izleyin:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Bilgi içeren Active Directory yerel kurulumları için kurulum adımları içerir. Etki alanına katılmış bir aygıtlar erişmeye devam etmek istiyorsanız, iki farklı şekilde, etkinleştirme için aşağıdaki makaleleri okuyun ve Kurulum Sihirbazı'nı çalıştırmadan önce adımları tamamlayın:
  
- [Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme](manage-windows-devices.md)
    
    -Bu, önerilen yoldur.
    
- [Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Adım 1: kayıt kişiselleştirin

1. Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Business](https://portal.microsoft.com)'da oturum açın. Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin. 
    
2. Sihirbazı başlatmak için yönetim merkezinde **Kuruluma başla**'yı seçin (durumunuza bağlı olarak bunun yerine **Kuruluma devam et** ifadesini de görebilirsiniz). 
    
3. Kullanmak istediğiniz etki alanı adını (contoso.com gibi) girin.
    
    Etki alanınızı girerek işleme devam edin. Örneğin, Azure AD Connect'i kullanırken etki alanınızı doğrulamış olsanız bile bunu yapmanız gerekir. Etki alanınızın doğrulamak için Azure AD Connect kullandıysanız aşağıdaki iki adımı sizin için geçerli değildir.
    
4. Doğrulayan etki alanı sahibi [herhangi bir DNS barındırma sağlayıcı için Office 365 oluşturmak DNS kayıtları](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) için sihirbazdaki adımları izleyin. 
    
    Bir örnek video görüntüleyebilirsiniz [Video: Yeni Yönetim Merkezi'ndeki Kurulum Office 365](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Bu videonun Microsoft 365 İş üzerinde veri korumaya ilişkin adımları içermediğini unutmayın.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Adım 2: kullanıcı eklemek ve lisansları atama

1. Kullanıcıları şimdi burada ekleyebilirsiniz veya yönetim merkezinde [kullanıcıları daha sonra da ekleyebilirsiniz](add-users-m365b.md). 
    
    Eklediğiniz tüm kullanıcılara otomatik olarak Microsoft 365 İş lisansı atanır.
    
2. Microsoft 365 İş aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect kullandıysanız), bu kullanıcılara hemen lisans atamanızı sağlayan bir seçenek görürsünüz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.
    
3. Ayrıca kimlik bilgilerini, eklediğiniz yeni kullanıcılarla paylaşmak için bir seçenek de görürsünüz. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.
    
4. E-posta iletilerini geçirmeyi atlayın ve **E-posta iletilerini geçir** sayfasında **İleri**'yi seçin. 
    
    Eğer başka bir e-posta Sağlayıcısı'ndan taşıma ve verilerinizi daha sonra kopyalamak istediğiniz [geçiş e-posta ve kişiler Office 365'e](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e)kaydedebilirsiniz.
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Adım 3: etki alanınızı Bağlan

> [!NOTE]
> .Onmicrosoft etki alanı kullanmayı seçtiniz veya Azure AD Bağlan kullanılır, bu adımı göremez. 
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Seçili değilse, [herhangi bir etki alanı Kaydedicisi ile Office 365 ayarlamak için değişiklik nameservers](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. E-posta ve diğer hizmetler sizin için ayarlanır
    
### <a name="step-4-manage-devices-and-work-files"></a>Adım 4: aygıtları yönetme ve dosyaları çalışma

1. **Koruma çalışma dosyaları taşınabilir aygıtlarınızda** sayfasında hem **aygıtları kaybolur veya çalınırsa, koruma çalışma dosyaları** ve ayarları **kullanıcıların mobil cihazlarda Office dosyalarının nasıl eriştiğini yönetme** **üzerinde**ayarlayın. Her her ayarın yanındaki köşeli çift tıklatarak alt ayar da erişebilirsiniz.
  
  Tüm lisanslı kullanıcılarınızın çalışma dosyaları şimdi IOS ve Android aygıtlarda, bunlar en erken korunan [Office uygulamaları yükleyin](set-up-mobile-devices.md) (ve bunların Microsoft 365 iş kimlik bilgileriyle kimlik doğrulaması). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. **Set Windows 10 aygıt yapılandırması** sayfasında, **Güvenli Windows 10 aygıtları** **üzerinde**ayarı.
  
   Her yanındaki köşeli çift ayraç tıklatarak alt ayar da erişebilirsiniz.
  
3. Kullanıcılarınızın tümü Windows 10 bilgisayarlar varsa ve varolan hiçbir Office yükler **Evet** veya Tıklat-Çalıştır Office yüklemeleri için **Office 10 aygıtlarda Windows yükleme** ayarını belirleyin. Durum bu değilse, bu seçenek **Hayır**olarak ayarlayın. Kullanıcı bilgisayarlarında hazırladıktan sonra Yönetim Merkezi'nden daha sonra [otomatik olarak Office yüklemek](auto-install-or-uninstall-office.md) olabilir. Yönergeler için bkz: [Office İstemcisi yüklemesine hazırlamak](prepare-for-office-client-deployment.md).
  
    Lisanslı kullanıcıları çalışma dosyalarını Windows 10 aygıtlarda hemen bunlar öngörülen 365 Microsoft Business Azure AD etki alanı veya aynı anda Microsoft 365 katılma sırasında [Windows 10 yeni bir bilgisayara yüklemek](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) için [Windows 10 aygıtları katılın](set-up-windows-devices.md) İş Azure AD etki alanı. 
  
4. **İleri** ' yi tıklatın ve kurulum ile yapılır. 
  
    Lütfen bize görüşlerinizi deneyimini geliştirmemize yardımcı olmak üzere, bu adımı bırakın.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Ek güvenlik ayarları

Güvenlik ve Kurulum Sihirbazı'ndaki Uyumluluk ayarına ek olarak, aşağıdaki ek ayarlar de ayarlayabilirsiniz:
  
- Güvenli olmayan ekleri karşı koruma ayarlayın. **Gelişmiş tehdit koruması** (ATP), kötü amaçlı içerik tanımlar ve balık avlama ve ransomware bulaşmalarını karşı korunmasına yardımcı olma teslim güvenli olmayan ekleri engeller. Eki korumasını etkinleştirmek için bkz: [Office 365 KM güvenli ekler ilkelerini kurun](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Kullanıcılar kötü niyetli bağlantıları tıklattığınızda ortamınızı korumak. ATP bunları kullanıcının tıklattığı zaman e-posta içindeki bağlantıları inceler. Bağlantı güvenli ise, kullanıcı siteyi ziyaret değil bir uyarı veya sitesinde engellenmiş haberdar. Bu balık avlama karşı korunmasına yardımcı olur. [Office 365 KM güvenli bağlantıları ilkelerini kurun](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) veya [Office 365 KM güvenli bağlantıları ilkelerini kurun](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Bir kullanıcının tüm posta **tutun dava**üzerinde koyarak silinmiş öğeleri de dahil olmak üzere tüm posta kutusu içeriği koruyabilirsiniz. Yönergeler için bkz. 
- [E-posta bekletme çevrimiçi Exchange arşivleme ile ayarlayın](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Örneğin, özelleştirilmiş **bekletme ilkeleri**, belirli bir süre korumak veya içeriği saklama dönemi sonunda kalıcı olarak silmek için ayarlayın. Menkul kıymetler ve uyumluluk Merkezi'nde, **veri yönetim** için gidin özelleştirilmiş bekletme ilkeleri etkinleştirebilirsiniz \> **bekletme**ve sonra sihirbazdaki adımları izleyin. Daha fazla bilgi için [Bekletme İlkeleri'ne genel bakış](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)konusuna bakın.
    
## <a name="next-steps"></a>Sonraki adımlar

Kendi lisansı olan kullanıcılar için aygıtlarını kurabileceğiniz sonraki adımdır.<br/> Bkz: [Microsoft 365 iş kullanıcıları için Windows aygıtları kurmak](set-up-windows-devices.md) ve [mobil aygıtlar Microsoft 365 iş kullanıcıları için ayarlayın](set-up-mobile-devices.md). <br/>[Microsoft 365 iş yönetme](manage.md) ilkeleri aygıt ve uygulama koruması nasıl konulara bağlantılar için bkz: ve nasıl kullanıcı aygıtlardan verileri kaldırmak. 
  


