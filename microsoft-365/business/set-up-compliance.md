---
title: Microsoft 365 İş Ekstra için tehdit korumasını artırma
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Veri kaybını önlemek ve müşterilerimizin hassas bilgilerini güvende tutmaya yardımcı olmak için uyumluluk özelliklerini ayarlayın.
ms.openlocfilehash: e210787718025c5df29af8d4a2283291dcecc2a8
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912540"
---
# <a name="set-up-compliance-features"></a>Uyumluluk özelliklerini ayarlama

Microsoft 365 İş Ekstra, verilerinizi ve cihazlarınızı korumaya ve müşterilerimizin hassas bilgilerini güvende tutmanıza yardımcı olacak özelliklerle birlikte gelir.

## <a name="set-up-dlp-features"></a>DLP özelliklerini ayarlama

Kişisel [verilerin kaybına karşı korunmak için](../compliance/create-a-dlp-policy-from-a-template.md) bir ilke ayarlama örneği için, şablondan DLP ilkesi oluşturma hakkında bilgi için bkz. 
  
DLP, birçok farklı yerel ayarın kullanımına hazır ilke şablonlarıyla birlikte gelir. Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri, gibi. Tam [liste için DLP ilkesi şablonlarının](../compliance/what-the-dlp-policy-templates-include.md) neler içermesi hakkında bilgi için bkz. Bu şablonların hepsi, PII şablonu örneğine benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Exchange Online Arşivleme ile e-posta bekletmeyi ayarlama

 **Exchange Online Arşivleme lisans** özellikleri, eBulma için e-posta içeriğini koruyarak uyumluluk ve mevzuat standartlarının korunmasına yardımcı olur. Ayrıca, bir sorun olduğu zaman risklerinizi azaltmaya yardımcı olur ve güvenlik ihlali sonrasında veya silinmiş öğeleri kurtarmanız gereken zaman verileri kurtarmak için bir yol sağlar. Bir kullanıcının içeriğinin hepsini korumak için mahkeme tutma veya korumak istediğiniz içeriği özelleştirmek için bekletme ilkelerini kullanabilirsiniz.
  
**Mahkeme tutma:** Silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini, kullanıcının posta kutusunun tamamını mahkemelere koyarak koruyabilirsiniz. 
    
Posta kutusunu mahkeme tutmada tutmak için Yönetim merkezinde:
    
1. Sol gezintide, Kullanıcılar Etkin  \> **kullanıcılar'a gidin.**
    
2. Posta kutusunu mahkeme tutması için kullanmak istediğiniz bir kullanıcı seçin. Kullanıcı bölmesinde Posta ayarlarını genişletin ve **Diğer ayarlar'ın** **yanında** Exchange özelliklerini **düzenle'yi seçin.**
    
3. Kullanıcının posta kutusu sayfasında, sol gezintide ** posta kutusu özellikleri  ** seçin ve ardından Mahkeme tutma altındaki Etkinleştir **bağlantısını seçin.**
    
4. Mahkeme **tutma iletişim kutusunda,** Mahkeme tutma süresi alanında mahkeme tutma **süresini belirtebilirsiniz.** Sonsuz bir tutunma yapmak için alanı boş bırakın. Ayrıca, not ekleyebilir ve posta kutusu sahibini mahkeme tutma hakkında daha fazla açıklamanız gerekten bir web sitesine yönlendirebilirsiniz. \>**Kaydet 'i tıklatın.**
    
**Bekletme:** Örneğin, belirli bir süre boyunca korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz. Daha fazla bilgi edinmek için, bekletme [ilkelerine Genel Bakış'a bakın.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Duyarlılık etiketlerini ayarlama

Duyarlılık etiketleri Azure Information Protection (AIP) Plan 1 ile birlikte gelir ve etiketleri uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur. Etiketler, kurallar ve koşullar tanımlayan yöneticiler, kullanıcılar tarafından el ile veya kullanıcıların önerilerinin verildiği bir birleşim kullanılarak otomatik olarak uygulanabilir.

Duyarlılık etiketlerini ayarlamak için, duyarlılık [etiketleri videosunu oluşturun ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection istemcisini el ile yükleme

AIP istemcisini el ile yüklemek için:

1. Microsoft **AzinfoProtection_UL.exe** [merkezinden indirin.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. Bir Word belgesini görüntüerek ve Giriş sekmesinde Duyarlılık seçeneğinin kullanılabilir olduğundan emin **olarak** yüklemenin çalıştığını **doğruleyebilirsiniz.**
<br/>![Word belgesinde Koruma sekmesi açılan listesinde.](../media/word-sensitivity.png)

Daha fazla bilgi için [bkz. İstemciyi yükleme.](/azure/information-protection/infoprotect-tutorial-step3)