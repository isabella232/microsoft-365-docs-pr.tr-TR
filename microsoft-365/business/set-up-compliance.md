---
title: Microsoft 365 iş için tehdit koruma artırın
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş tehdit koruma sisteminizi kurma ve hassas verilerinizi korumak.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086412"
---
# <a name="set-up-compliance-features"></a>Uyumluluk Özellikleri Kurma

Microsoft 365 iş verilerinizi ve aygıtları korumak ve sizin ve müşterilerinizin önemli bilgilerin güvenliğini sağlamanıza yardımcı olmak için özellikler bulunur.

## <a name="set-up-dlp-features"></a>DLP özellikleri kurma

[Bir şablondan bir DLP ilkesi oluşturma](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) kişisel olarak tanımlanabilen bilgiler (PII) karşı korumak için bir ilke ayarlama konusunda bir örnek için bkz. 
  
DLP birçok farklı yerel ayarlar için birçok hazır kullanım ilkesi şablonuyla birlikte gelir. Örneğin, Avustralya mali verileri, kişisel bilgi Act Kanada, ABD finansal veriler, vb.. [Ne DLP ilke şablonları dahil](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) tam bir listesi için bkz. Tüm bu şablonları PII şablon örneğe benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-posta bekletme çevrimiçi Exchange arşivleme ile ayarlama

 **Exchange Online arşivleme** lisans özellikleri, uyumluluk ve yasal standartlar tarafından e-posta koruma eBulma için içerik sağlamak yardımcı olur. Ayrıca, bir açtığı dava sonucunda durumunda riskini azaltmaya yardımcı olur ve sonra bir güvenlik ihlali veya silinmiş öğeleri kurtarmak gereksinim duyduğunuzda verileri kurtarmak için bir yol sağlar. Tüm kullanıcı içeriğini korumak için dava tutma kullanın veya korumak istediğiniz özelleştirmek için bekletme ilkeleri kullanın.
  
**Dava tutun:** Dava üzerinde bir kullanıcının tüm posta koyarak dahil silinmiş öğeleri tutma tüm posta kutusu içeriğini koruyabilirsiniz. 
    
Dava Tutuluyor, Yönetim Merkezi bir posta kutusu yerleştirmek için:
    
1. Sol nav uygulamasında, **Kullanıcılar** için giderek \> **Etkin kullanıcılar**.
    
2. Dava üzerinde yerleştirmek istediğiniz alıcının posta kutusu tutun bir kullanıcı seçin ve kullanıcı Bölmesi'nde **posta ayarları** ' nı genişletin ve **Exchange düzenleme özellikleri**yanında **daha fazla ayar** seçin.
    
3. Kullanıcının posta kutusu sayfasında seçin ** posta kutusu özellikleri ** üzerinde sol nav ve **dava tutun**altında **Etkinleştir** bağlantısını seçin.
    
4. **Dava tutun** dava belirtebileceğiniz iletişim kutusunu **dava tutma süresi** alanında süre basılı tutun, alan sonsuz bir ayrı tutma yerleştirmek isterseniz boş bırakın. Ayrıca notlar ekleyin ve posta kutusu sahibi dava hakkında daha fazla tutun açıklamak için sahip olabileceği bir Web sitesine doğrudan \> **kaydedin**.
    
**Tutma:** Belirli bir süre korumak veya içeriği saklama dönemi sonunda kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz. Daha fazla bilgi için [Bekletme İlkeleri'ne genel bakış](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)konusuna bakın.

## <a name="set-up-azure-information-protection-features"></a>Azure bilgi koruma özellikleri kurma

Azure bilgi koruma (AIP) sınıflandırmak ve etiketleri uygulayarak belgeler ve e-postalar, isteğe bağlı olarak, korunmasına yardımcı olur. Kural ve koşulları tanımlamak yöneticileri tarafından el ile kullanıcılar tarafından veya kullanıcılara öneriler burada verilmiştir bir birleşimini kullanarak etiketleri otomatik olarak uygulanabilir.

Outlook Web, e-postalar için aşağıdaki yerleşik etiketlerini ve kısıtlamaları uygulayabilirsiniz:
  
- **İletme**: alıcılar bu iletiyi okuyabilir, ancak bunlar iletemez, yazdıramaz, veya içerik kopyalama
    
- **Şifreleme**: iletinin tamamını şifrelenir. Alıcılar şifrelenmiş içeriği erişmeden önce kimliklerini onaylamak gerekir ve şifrelemeyi kaldıramazsınız.
    
- **Gizli**: e-posta içeriğini ve eklerini, ancak kuruluşunuzun dışındaki kişilere, kuruluşunuzdaki çalışanların tam izinleri verir. Veri sahipleri izleyebilir ve içerik herhangi bir noktada iptal edin.
    
- **Oldukça gizli**: oldukça gizli verileri görüntülemek, düzenlemek ve Yanıtla, ancak değil iletmek, yazdırmak veya verileri kopyalamak çalışanların izin vererek, bu kısıtlamayı uygulanabilir. Veri sahipleri izleyebilir ve içerik herhangi bir noktada iptal edin.

### <a name="make-sure-azure-information-protection-is-activated"></a>Azure bilgi koruma etkinleştirilmiş olduğundan emin olun

AIP etkinleştirilmiş olduğunu doğrulamak için:

1. [Azure portal](https://portal.azure.com/)oturum açın.

2. **Arama kutusu** *Azure bilgi koruma* **tüm hizmetleri** ve türünü seçin.

3. Sonuçları görüntüledikten sonra sık yapmak için **Azure bilginin korunması** için İleri ve kolayca bulabilmek için Başlat'ı tıklatın.

4. **Azure bilgi koruma** seçin \> **korumasını etkinleştirme** ve marka emin durumu ayarlanır için etkinleştirilmiş. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Azure bilgi koruma İlkesi ve varsayılan etiketleri görüntüleme 

Görüntülemek ve değiştirmek için varolan etiketleri:

1. Azure bilgi koruma Panosu üzerinde **sınıflandırmaları** seçin \> **etiketleri**. <br/>![Azure bilginin korunması için standart etiketler.](media/AIPLabels.png)

2. Tüm etiket seçeneklerini görüntülemek için seçebilirsiniz, ancak değiştirebilirsiniz görünen ad, renkler vb..
 
3. Bkz: [Değiştir ve yeni etiketler oluşturmak](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) kendi oluşturmak istiyorsanız. 

### <a name="install-the-azure-information-protection-client-manually"></a>Azure bilgi koruma İstemcisi'ni el ile yükleme

AIP istemciyi el ile yüklemek için:

1. **AzInfoProtection.exe** , [Microsoft Yükleme Merkezi'ndeki](https://www.microsoft.com/download/details.aspx?id=53018)karşıdan yükleyin.
 
2. Yükleme Word belgesi görüntüleme ve **Koru** seçeneği **Giriş** sekmesinde kullanılabilir durumda olmasını sağlayarak çalışılan doğrulayabilirsiniz. <br/>![Koruma sekmesini aşağı açılan bir Word belgesinde.](media/Word_Protect.png)

Daha fazla bilgi için bkz: [İstemci Yükleme](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
