---
title: Microsoft 365 Business Premium için tehdit koruması artırın
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
search.appverid:
- BCS160
- MET150
description: Veri kaybını önlemek ve sizin ve müşterilerinizin hassas bilgilerinin güvenliğini sağlamaya yardımcı olmak için uyumluluk özellikleri ayarlayın.
ms.openlocfilehash: a3405207cd7d2d6565807ef0f3a51acbcb80409a
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165747"
---
# <a name="set-up-compliance-features"></a>Uyumluluk özelliklerini ayarlama

Microsoft 365 Business Premium'unuz, verilerinizi ve cihazlarınızı koruyan ve sizin ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olacak özelliklerle birlikte gelir.

## <a name="set-up-dlp-features"></a>DLP özelliklerini ayarlama

Bkz. Kişisel olarak tanımlanabilir bilgilere (PII) karşı korumak için bir ilke oluşturma hakkında bir örnek için şablondan Bir [DLP ilkesi oluşturun.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) 
  
DLP, birçok farklı yerel bölge için kullanıma hazır ilke şablonlarıyla birlikte gelir. Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri ve benzeri. Tam liste için [DLP ilkesi şablonlarının neler içerdiğini](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) görün. Bu şablonların tümü, KIŞISEL bilgiler şablonu örneğine benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Exchange Online Arşivleme ile e-posta saklama yı ayarlama

 **Exchange Online Arşivleme** lisansı özellikleri, e-posta içeriğini eDiscovery için koruyarak uyumluluk ve mevzuat standartlarını korumaya yardımcı olur. Ayrıca, bir dava varsa riskinizi azaltmaya yardımcı olur ve bir güvenlik ihlalinden sonra veya silinen öğeleri kurtarmanız gerektiğinde verileri kurtarmanın bir yolunu sağlar. Bir kullanıcının tüm içeriğini korumak için dava tutma yı kullanabilir veya korumak istediğiniz şeyi özelleştirmek için bekletme ilkelerini kullanabilirsiniz.
  
**Dava tutma:** Bir kullanıcının tüm posta kutusunu dava beklemeye alarak silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini koruyabilirsiniz. 
    
Yönetici merkezinde, dava beklemeye bir posta kutusu yerleştirmek için:
    
1. Sol navigasyonda, **Users** \> **Active kullanıcılarına**gidin.
    
2. Dava beklemeye almak istediğiniz posta kutusunu seçin. Kullanıcı **bölmesinde, Posta ayarlarını**genişletin ve **Daha Fazla ayar'ın**yanında **Exchange özelliklerini edit'i**seçin.
    
3. Kullanıcı için posta kutusu sayfasında, sol daki ** posta kutusu özelliklerini seçin ve ardından **Dava bekletme**altında **Etkinleştir** bağlantısını seçin.
    
4. Dava **tutma** iletişim kutusunda, **Dava tutma süresi** alanında dava tutma süresini belirtebilirsiniz. Sonsuz bir tutma yerleştirmek istiyorsanız alanı boş bırakın. Ayrıca notlar ekleyebilir ve posta kutusu sahibini dava tutma hakkında daha fazla açıklama nız gerekebilecek bir web sitesine yönlendirebilirsiniz. \>**Kaydet.**
    
**Bekletme:** Örneğin, belirli bir süre için korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz. Daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

## <a name="set-up-sensitivity-labels"></a>Duyarlılık etiketlerini ayarlama

Duyarlılık etiketleri Azure Bilgi Koruması (AIP) Planı 1 ile birlikte gelir ve etiketler uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur. Etiketler, kuralları ve koşulları tanımlayan yöneticiler tarafından, kullanıcılar tarafından el ile veya kullanıcılara önerilerin verildiği bir kombinasyon kullanılarak otomatik olarak uygulanabilir.

Duyarlılık etiketleri ayarlamak [için, duyarlılık etiketleri videosu oluşturma ve yönetme](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) yi görüntüleyin.



### <a name="install-the-azure-information-protection-client-manually"></a>Azure Bilgi Koruması istemcisini el ile yükleme

AIP istemcisini el ile yüklemek için:

1. [Microsoft indirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzinfoProtection_UL.exe** indirin.
 
2. Yüklemenin bir Word belgesini görüntüleyerek ve **Duyarlılık** seçeneğinin **Giriş** sekmesinde kullanılabilir olduğundan emin olarak çalıştığını doğrulayabilirsiniz.
<br/>![Word belgesinde koruma sekmesi açılır.](../media/word-sensitivity.png)

Daha fazla bilgi için [bkz.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
