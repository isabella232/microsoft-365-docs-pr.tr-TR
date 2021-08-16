---
title: Güvenlik için tehdit korumasını Microsoft 365 İş Ekstra
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Veri kaybını önlemek ve müşterinizin hassas bilgilerini güvende tutmaya yardımcı olmak için uyumluluk özelliklerini ayarlayın.
ms.openlocfilehash: ae5e5727db1f372c40aa4468329021525b6dfc8c5ebbf34705184e461df069e5
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53881864"
---
# <a name="set-up-compliance-features"></a>Uyumluluk özelliklerini ayarlama

Müşterileriniz Microsoft 365 İş Ekstra verilerinizi ve cihazlarınızı korumaya ve sizin ve müşterilerinize hassas bilgilerini güvende tutmanıza yardımcı olacak özelliklerle birlikte gelir.

## <a name="set-up-dlp-features"></a>DLP özelliklerini ayarlama

Kişisel [verilerin kaybından korunmaya yönelik bir](../compliance/create-a-dlp-policy-from-a-template.md) ilke ayarlama hakkında bilgi için bkz. Şablondan DLP ilkesi oluşturma. 
  
DLP, birçok farklı yerel ayarı için kullanıma hazır birçok ilke şablonuyla birlikte gelir. Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgileri Yasası, ABD Finansal Verileri, ve diğer. Tam [liste için bkz. DLP](../compliance/what-the-dlp-policy-templates-include.md) ilkesi şablonlarının şunları içerir. Bu şablonların hepsi, PII şablonu örneğine benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-posta bekletmeyi otomatik olarak Exchange Online Arşivleme

 **Exchange Online Arşivleme** lisans özellikleri, eKbulma için e-posta içeriğini koruyarak uyumluluk ve mevzuat standartlarını korumaya yardımcı olur. Ayrıca, bir güvenlik ihlali durumunda riski azaltmanıza yardımcı olur ve güvenlik ihlali sonrasında veya silinmiş öğeleri kurtarmanız gereken durumlarda verileri kurtarmak için bir yol sağlar. Bir kullanıcının içeriğini korumak için mahkeme saklamayı veya korumak istediğiniz içeriği özelleştirmek için bekletme ilkelerini kullanabilirsiniz.
  
**Mahkeme tutma:** Kullanıcının posta kutusunun tamamını mahkemelere koyarak, silinmiş öğeler de dahil olmak üzere tüm posta kutusu içeriğini koruyabilirsiniz. 
    
Posta kutusunu mahkeme tutma için Yönetim merkezinde tutmak için:
    
1. Sol gezintide Kullanıcılar Etkin **kullanıcılar'a** \> **gidin.**
    
2. Posta kutusunu mahkemelere almak istediğiniz bir kullanıcı seçin. Kullanıcı bölmesinde Posta **ayarları'ni genişletin ve Diğer** ayarlar'ın **yanındaki Posta özelliklerini** **Exchange seçin.**
    
3. Kullanıcının posta kutusu sayfasında, sol gezintide ** posta kutusu özellikleri  ** seçin ve sonra Mahkeme tutma altındaki Etkinleştir **bağlantısını seçin.**
    
4. Mahkeme **tutma iletişim** kutusunda, Mahkeme tutma süresi alanında **mahkeme tutma süresini belirtebilirsiniz.** Sonsuz bir basılı tutmak istediğiniz alanı boş bırakın. Ayrıca, notlar ekleyebilir ve posta kutusu sahibini bir web sitesine yönlendirebilirsiniz ve bu konuda mahkeme tutma hakkında daha fazla açıklamanız gerekir. \>**Kaydet'i tıklatın.**
    
**Bekletme:** Örneğin, belirli bir süre boyunca korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz. Daha fazla bilgi edinmek için [bkz. Bekletme ilkelerine genel bakış.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Duyarlılık etiketlerini ayarlama

Duyarlılık etiketleri Azure Information Protection (AIP) Plan 1 ile gelir ve etiketleri uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur. Etiketler, kurallar ve koşullar tanımlayan yöneticiler tarafından, kullanıcılar tarafından el ile veya kullanıcıların önerilerinin verildiği bir birleşim kullanılarak otomatik olarak uygulanabilir.

Duyarlılık etiketlerini ayarlamak için duyarlılık etiketleri [videosunu oluşturun ve yönetin.](../business-video/create-sensitivity-labels.md)



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Information Protection istemcisini el ile yükleme

AIP istemcisini el ile yüklemek için:

1. Microsoft **AzinfoProtection_UL.exe** [merkezinden indirmeniz gerekir.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. Yüklemenin çalıştığını doğrulamak için bir Word belgesi görüntüleyebilirsiniz ve Giriş sekmesinde Duyarlılık **seçeneğinin** kullanılabilir olduğundan **emin** olun.
<br/>![Word belgesinde Koruma sekmesi açılan listesinde.](../media/word-sensitivity.png)

Daha fazla bilgi için [bkz. İstemciyi yükleme](/azure/information-protection/infoprotect-tutorial-step3).