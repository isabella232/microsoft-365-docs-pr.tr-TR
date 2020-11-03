---
title: Microsoft 365 Business Premium için tehdit korumasını arttırın
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
description: Veri kaybını önlemek ve müşterilerinizin hassas bilgilerinin güvenliğini sağlamak için uyumluluk özelliklerini ayarlayın.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841183"
---
# <a name="set-up-compliance-features"></a>Uyumluluk özelliklerini ayarlama

Microsoft 365 Iş ekstra, verilerinizi ve aygıtlarınızı korumaya yönelik özelliklerle birlikte gelir ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olur.

## <a name="set-up-dlp-features"></a>DLP özelliklerini ayarlama

Kişisel verilerin kaybolmasını önlemek amacıyla ilke ayarlama hakkında örnek için bir [ŞABLONDAN DLP Ilkesi oluşturma](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) konusuna bakın. 
  
DLP, birçok farklı yerel ayar için kullanıma hazır birçok ilke şablonlarıyla gelir. Örneğin, Avustralya finansal verileri, Kanada kişisel bilgileri, ABD finansal verileri vb. Tam liste için [DLP ilkesi şablonlarının neler olduğunu](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) görün. Bu şablonların tümü, PII şablon örneğine benzer şekilde etkinleştirilebilir. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Exchange Online Arşivleme ile e-posta bekletmesini ayarlama

 **Exchange Online arşivleme** lisansı özellikleri, eBulma için e-posta içeriğini koruyarak uyumluluk ve mevzuat standartlarını korumanıza yardımcı olur. Ayrıca, bir avda olması durumunda riskin azaltılmasına yardımcı olur ve bir güvenlik ihlalinin ardından silinmiş öğeleri kurtarmanız gerektiğinde verilerin kurtarılması için bir yol sağlar. Bir kullanıcının içeriğinin tümünü korumak veya korumak istediğiniz öğeyi özelleştirmek için bekletme ilkeleri 'ni kullanabilirsiniz.
  
Dava **tutma:** Bir kullanıcının tüm posta kutusunu dava tutma ile birlikte bırakarak silinmiş öğeler dahil tüm posta kutusu içeriğini koruyabilirsiniz. 
    
Posta kutusunu, bir posta kutusu
    
1. Sol gezintide, **Kullanıcılar** \> **etkin kullanıcılarına** gidin.
    
2. Posta kutusunu basılı tutma için yerleştirmek istediğiniz kullanıcıyı seçin. Kullanıcı bölmesinde **posta ayarlarını** genişletin ve **daha fazla ayar** 'Nın yanında **Exchange özelliklerini Düzenle** 'yi seçin.
    
3. Kullanıcının posta kutusu sayfasında, sol gezinti bölmesinde * * posta kutusu özellikleri * * seçeneğini belirleyin ve sonra da bir bağlantı altında **saklama** bağlantısını **Etkinleştir** 'i seçin.
    
4. **Katmanlama bekletme** iletişim kutusunda, dava tutma **süresi** alanında dava tutma süresini belirtebilirsiniz. Sonsuz bir bekletme yerleştirmek istiyorsanız alanı boş bırakın. Ayrıca not ekleyebilir ve posta kutusu sahibini bir Web sitesine yönlendirebilirsiniz, bir dava alma hakkında daha fazla bilgi edinebilirsiniz. \>**Kaydetme**.
    
**Bekletme:** Özel bekletme ilkelerini, örneğin belirli bir süre boyunca korumak veya saklama döneminin sonunda içeriği kalıcı olarak silmek için etkinleştirebilirsiniz. Daha fazla bilgi edinmek için [bekletme Ilkelerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)konusuna bakın.

## <a name="set-up-sensitivity-labels"></a>Duyarlılık etiketlerini ayarlama

Duyarlılık etiketleri Azure bilgi koruması (AıP) plan 1 ile gelir ve etiket uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumaya yardımcı olur. Etiketler, kuralları ve koşulları tanımlayan ve kullanıcılar tarafından el ile veya kullanıcıların öneri verdiği bileşimi kullanarak otomatik olarak uygulanabilir.

Duyarlılık etiketlerini ayarlamak için, [duyarlılık etiketleri oluşturma ve yönetme](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videosu.



### <a name="install-the-azure-information-protection-client-manually"></a>Azure bilgi Koruması istemcisini el ile yükleme

AıP istemcisini el ile yüklemek için:

1. [Microsoft İndirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzinfoProtection_UL.exe** indirin.
 
2. Bir Word belgesini görüntüleyerek ve **giriş** sekmesinde **duyarlılık** seçeneğinin kullanılabilir olduğundan emin olmak için yüklemenin çalıştığını doğrulayabilirsiniz.
<br/>![Word belgesinde koruma sekmesi açılır.](../media/word-sensitivity.png)

Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
