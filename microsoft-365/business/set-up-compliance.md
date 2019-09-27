---
title: Microsoft 365 Business için tehdit korumayı artırın
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş Tehdit Koruması'nı ayarlayın ve hassas verileri koruyun.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288755"
---
# <a name="set-up-compliance-features"></a>Uyumluluk özelliklerini ayarlama

Microsoft 365 Business'ınız verilerinizi ve cihazlarınızı koruyan ve sizin ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olan özelliklerle birlikte gelir.

## <a name="set-up-dlp-features"></a>DLP özelliklerini ayarlama

Bkz. Kişisel olarak tanımlanabilir bilgilere (PII) karşı korumak için bir ilke oluşturma hakkında bir örnek için şablondan Bir [DLP ilkesi oluşturun.](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) 
  
DLP, birçok farklı yerel bölge için kullanıma hazır ilke şablonlarıyla birlikte gelir. Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri, vb. Tam liste için [DLP ilkesi şablonlarının neler içerdiğini](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) görün. Bu şablonların tümü, KIŞISEL bilgiler şablonu örneğine benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Exchange Online Arşivleme ile e-posta saklama yı ayarlama

 **Exchange Online Arşivleme** lisansı özellikleri, e-posta içeriğini eDiscovery için koruyarak uyumluluk ve mevzuat standartlarını korumaya yardımcı olur. Ayrıca, bir dava durumunda riskinizi azaltmaya yardımcı olur ve bir güvenlik ihlalinden sonra veya silinen öğeleri kurtarmanız gerektiğinde verileri kurtarmanın bir yolunu sağlar. Bir kullanıcının tüm içeriğini korumak için dava tutma yı kullanabilir veya korumak istediğiniz şeyi özelleştirmek için bekletme ilkelerini kullanabilirsiniz.
  
**Dava tutma:** Bir kullanıcının tüm posta kutusunu dava beklemeye alarak silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini koruyabilirsiniz. 
    
Yönetici merkezinde, dava beklemeye bir posta kutusu yerleştirmek için:
    
1. Sol navigasyonda, **Users** \> **Active kullanıcılarına**gidin.
    
2. Dava beklemeye ve kullanıcı bölmesine yerleştirmek istediğiniz posta kutusunu seçin **Posta ayarlarını** genişletin ve **Daha Fazla ayar** yanında Exchange özelliklerini **düzenleyin'** i seçin.
    
3. Kullanıcı için posta kutusu sayfasında, sol daki ** posta kutusu özelliklerini seçin ve ardından **Dava bekletme**altında **Etkinleştir** bağlantısını seçin.
    
4. Dava **tutma** iletişim kutusunda, **dava bekleme süresi** alanında dava tutma süresini belirtebilir, sonsuz bir bekleme yerleştirmek istiyorsanız alanı boş bırakabilirsiniz. Ayrıca notlar ekleyebilir ve posta kutusu sahibini \> **kaydet**davası hakkında daha fazla açıklama yapmak zorunda kabileceğiniz bir web sitesine yönlendirebilirsiniz.
    
**Bekletme:** Örneğin, belirli bir süre için korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz. Daha fazla bilgi için [bkz.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)

## <a name="set-up-azure-information-protection-features"></a>Azure Bilgi Koruması özelliklerini ayarlama

Azure Bilgi Koruması (AIP), etiketler uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur. Etiketler, kuralları ve koşulları tanımlayan yöneticiler tarafından, kullanıcılar tarafından el ile veya kullanıcılara önerilerin verildiği bir kombinasyon kullanılarak otomatik olarak uygulanabilir.

Web'deki Outlook'ta e-postalarınıza aşağıdaki yerleşik etiketleri ve kısıtlamaları uygulayabilirsiniz:
  
- **İletme :** Alıcılar iletiyi okuyabilir, ancak içeriği iletemez, yazdıramaz veya kopyalayamaz
    
- **Şifrele**: İletinin tamamı şifrelenir. Alıcıların şifreli içeriğe erişmeden önce kimliklerini doğrulamaları ve şifrelemeyi kaldıramamaları gerekir.
    
- **Gizli**: Kuruluşunuzdaki çalışanlara e-posta içeriği ne kadar e-posta içeriğine ve ekleri için tam izin verir, ancak kuruluşunuz dışındaki kişilere tam izin verir. Veri sahipleri herhangi bir noktada içeriği izleyebilir ve iptal edebilir.
    
- **Son Derece Gizli**: Bu kısıtlama, çalışanların verileri görüntülemesine, görüntülemesine ve yanıtlamasına izin veren, ancak verileri iletmeme, yazdırmama veya kopyalamama olanağı tanıyan son derece gizli verilere uygulanabilir. Veri sahipleri herhangi bir noktada içeriği izleyebilir ve iptal edebilir.

### <a name="make-sure-azure-information-protection-is-activated"></a>Azure Bilgi Korumasının etkinleştirildiğinden emin olun

AIP'nin etkinleştirildiğini doğrulamak için:

1. Azure [portalında](https://portal.azure.com/)oturum açın.

2. **Tüm hizmetleri** seçin ve **Arama Kutusu'nda**Azure *Bilgi Koruması* yazın.

3. Sonuçlar görüntülendikten sonra, sık kullanılan ve daha sonra kolayca bulunmasını sağlamak için **Azure Bilgi Koruması'nın** yanındaki başlat'ı tıklatın.

4. **Azure Bilgi Koruması** \> **Koruması etkinleştirmesini** seçin ve durumun etkinleştirilecek şekilde ayarlandıklarına emin olun. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Azure Bilgi Koruması ilkesini ve varsayılan etiketleri görüntüleyin 

Varolan etiketleri görüntülemek ve değiştirmek için:

1. Azure Bilgi Koruması panosunda Sınıflandırma \> **Etiketleri'ni**seçin. **** <br/>![Azure Bilgi Koruması için standart etiketler.](media/AIPLabels.png)

2. Seçenekleri görüntülemek için herhangi bir etiket seçebilirsiniz, ekran adını, renkleri, vb değiştirebilirsiniz.
 
3. Bkz. Kendi etiketinizi oluşturmak istiyorsanız [Değiştir ve yeni etiketler oluşturun.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) 

### <a name="install-the-azure-information-protection-client-manually"></a>Azure Bilgi Koruması istemcisini el ile yükleme

AIP istemcisini el ile yüklemek için:

1. [Microsoft indirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzInfoProtection.exe** indirin.
 
2. Yüklemenin bir Word belgesini görüntüleyerek ve **Koruma** seçeneğinin **Ana sayfa** sekmesinde kullanılabilir olduğundan emin olarak çalıştığını doğrulayabilirsiniz. <br/>![Word belgesinde koruma sekmesi açılır.](media/Word_Protect.png)

Daha fazla bilgi için bkz: [Istemciyi yükleyin.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
