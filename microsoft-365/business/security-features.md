---
title: Microsoft 365 İş Ekstra güvenlik ve uyumluluk özellikleri
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: BILGISAYAR, telefon ve tabletlerde verilerinizi korumaya yardımcı olmak için Microsoft 365 İş Ekstra ile birlikte gelen güvenlik özellikleri hakkında bilgi alın.
ms.openlocfilehash: d641fc66e27f3c5e0a7c8609e4fa25fac93d8561
ms.sourcegitcommit: 956176ed7c8b8427fdc655abcd1709d86da9447e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51052264"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 İş Ekstra güvenlik ve uyumluluk özellikleri

Microsoft 365 İş Ekstra pc, telefon ve tabletlerde verilerinizi korumaya yardımcı olmak için basitleştirilmiş güvenlik özellikleri sunar.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 yönetim merkezi güvenlik özellikleri

Yönetim merkezinde microsoft 365 İş Ekstra güvenlik özelliklerinin çoğunu yöneterek bu özellikleri basitleştirilmiş bir şekilde açamaz veya kapatamazsiniz. Yönetim merkezinde şunları yapabilirsiniz:
  
- [Android veya iOS cihazları için uygulama yönetimi ayarlarını yapın.](app-protection-settings-for-android-and-ios.md) 
    
    Bu ayarlar arasında, belirli bir süre sonra etkin olmayan bir cihazdan dosya silme, iş dosyalarını şifreleme ve kullanıcıların PIN ayarlamalarını gerektirme gibi ayarlar yer içerir.
    
- [Windows 10 cihazları için uygulama koruma ayarlarını yapın.](protection-settings-for-windows-10-devices.md) 
    
    Bu ayarlar hem şirkete ait hem de kişisel olarak sahip olunan cihazlardaki şirket verilerine uygulanabilir.
    
- [Windows 10 cihazları için cihaz koruma ayarlarını yapın.](protection-settings-for-windows-10-pcs.md) 
    
    Bir cihaz kaybolur veya çalınırsa verilerin korunmasına yardımcı olmak için [BitLocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) şifrelemesini etkinleştirebilirsiniz ve [Windows Exploit Guard'ın](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) fidye yazılımlarına karşı gelişmiş koruma sağlamasını sebilirsiniz. 
    
- [Cihazlardan şirket verilerini kaldırma](remove-company-data.md)
    
    Bir cihaz kaybolur, çalınırsa veya bir çalışan şirketten ayrılırsa şirket verilerini uzaktan temizleyebilirsiniz.
    
- [Windows 10 cihazlarını fabrika ayarlarına sıfırlayın.](reset-devices-to-factory-settings.md) 
    
    Cihaz koruma ayarları uygulanmış tüm Windows 10 cihazlarını sıfırlayabilirsiniz.
    
## <a name="additional-security-features"></a>Ek güvenlik özellikleri 

Microsoft 365 İş Ekstra'daki gelişmiş özellikler, siber tehditlere karşı işlerinizi korumanıza ve hassas bilgileri korumaya yardımcı olmak için kullanılabilir.
  
- **[Office 365 için Microsoft Defender](../security/defender-365-security/defender-for-office-365.md)**
    
    Office 365 için Microsoft Defender, çalışan veya müşteri bilgilerini tehlikeye atarak tasarlanmış gelişmiş kimlik avı ve fidye yazılımı saldırılarına karşı işlerinizi korumanıza yardımcı olur. Özellikler şunlardır:
    
  - Tehlikeli iletileri tespit etmek ve atmak için gelişmiş ek taraması ve yapay zeka destekli çözümleme.
    
  - Kimlik avı düzeninin bir parçası olup olmadığını değerlendirmek için e-postada bağlantıların otomatik denetimleri. Bu, güvenli olmayan web sitelerine erişmenizi sağlar.

- **[Azure portalında Intune'ın tüm özellikleri](/mem/intune/fundamentals/what-is-intune)**
    
    Azure portalında Intune yönetim merkezine erişim, MacOS cihazları, iPhone ve Android cihazlarının yönetimi gibi ek güvenlik özelliklerini ayarlamanın yanı sıra Microsoft 365 yönetim merkezi aracılığıyla edinilen Windows için gelişmiş cihaz yönetimi de ayarlamaya olanak tanır.
- **Azure AD [Premium](/azure/active-directory/conditional-access/overview) P1 planıyla aynı Koşullu Erişim**


    Koşullu Erişim, kuruma oturum açma risklerinden, beklenmeyen bir ağ veya yerel bağlantıdan erişim girişimlerine, riskli cihaz türlerinden erişim girişimlerine ve buna gibi çeşitli risklerden korunmanıza yardımcı olabilir. Koşullu Erişim ilkeleri, ilk kimlik doğrulaması tamamlandıktan sonra uygulanır ve ilk kimlik doğrulama olayından gelen sinyalleri kullanarak, denenen erişimin onaylandır mı, redded mi olacağını veya daha fazla kanıt (ikinci kimlik formu gibi) gerek olup olmadığını belirler.

    Koşullu erişim özellikleri şunlardır:

    - Kullanıcı adı, grup ve role göre erişim
    - Uygulamaya [dayalı erişim](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Konuma göre erişim](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  yalnızca güvenilen IP aralıklarından veya belirli ülkelerden erişime izin ver 
    - Erişim için MFA gerektirme
    - Eski kimlik doğrulamayı kullanan [uygulamalara erişimi engelleme](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Uygulamaların [Intune uygulama korumasını kullanmasını gerektirme](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Üçüncü taraf sağlayıcılarla MFA gibi özel kimlik doğrulaması (DUO gibi).
   
    Diğer özellikler:
    - [Karma](/azure/active-directory/authentication/concept-sspr-customization) Azure AD için self servis parola sıfırlama
    
## <a name="compliance-features"></a>Uyumluluk özellikleri

Microsoft 365 İş Ekstra aboneliğiniz, uyumluluk ve mevzuat standartlarını korumanıza yardımcı olan özellikler içerir.

- **[Veri kaybı önleme ilkelerine](../compliance/data-loss-prevention-policies.md)** (DLP) genel bakış. 
    
    DLP'i, kredi kartı numaraları, sosyal güvenlik numaraları gibi hassas bilgileri, şirket dışında yanlışlıkla paylaşımını önlemek için otomatik olarak algılayan bir DLP kurabilirsiniz.
    
- **[Exchange Online Arşivleme](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Arşivleme lisansı, sürekli veri yedeklemeyle iletilerin kolayca arşivlenmesine olanak sağlar. Daha sonra keşif veya geri yükleme için gerekli olduğu durumlara karşı silinmiş öğeler de dahil olmak üzere kullanıcının tüm e-postalarını depolar. Buna ek olarak, mahkeme tutma, eBulma veya uyumluluk gereksinimlerini karşılamak üzere e-posta verilerini korumak için farklı bekletme ilkeleri kullanabilirsiniz.
    
- **[Duyarlılık etiketleri](../compliance/sensitivity-labels.md)**

   Microsoft 365 İş Ekstra, [Azure Information Protection Plan 1'in tüm özelliklerini içerir.](https://go.microsoft.com/fwlink/p/?linkid=871407) Bu planla, e-posta ve belgelerde "İ iletme" ve "Kopyalama" gibi denetimlerle hassas bilgilere erişimi denetlemenizi sağlayan Duyarlılık etiketleri oluşturabilirsiniz.  Ayrıca hassas bilgileri "Gizli" olarak sınıflandırabilir ve sınıflandırılmış bilgilerin işletme dışında ve iş içinde nasıl paylaşıla olacağını belirtebilirsiniz. Kurumsal sınıf şifreleme, e-posta ve belgelere kolayca uygulanarak, bilgilerin gizli tutabilirsiniz. Office uygulamaları için Azure Information Protection istemci eklentisini de yükleyebilirsiniz. Daha fazla bilgi için [Azure Information Protection birleşik etiketleme istemcisine bakın.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Duyarlılık etiketleri için etiketi **AzInfoProtection_UL.exe.**

Bu özellikleri Güvenlik Uyumluluk merkezi ve &amp; Intune yönetim merkezinde yönetsiniz. Zamanla basitleştirilmiş denetimler Microsoft 365 yönetim merkezine eklenecektir.
  
    
## <a name="faq"></a>SSS

 ### <a name="are-these-security-features-available-in-all-markets"></a>Bu güvenlik özellikleri tüm pazarlarda kullanılabilir mi?
  
Evet, bu özellikler Microsoft 365 İş Ekstra'nın satıldığı tüm pazarlarda kullanılabilir.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Güvenlik Uyumluluk merkezini nasıl &amp; bulamıyorum?
  
1. [Yönetici kimlik bilgilerinizi kullanarak Microsoft 365 İş Ekstra'da](https://portal.microsoft.com/) oturum açma. 
    
2. Sol gezintide Yönetim **merkezlerini bulun** ve genişletin. 
    
    ![Microsoft 365 yönetim merkezinin sol gezintisinde Yönetim merkezleri'ni seçin.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Güvenlik **uyumluluk &amp; merkezine gitmek** için Güvenlik &amp; Uyumluluğu'seçin.
