---
title: Microsoft 365 Business Premium güvenlik ve uyumluluk özellikleri
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
description: PC, telefon ve tabletlerde verilerinizi korumaya yardımcı olmak için Microsoft 365 Business Premium ile sağlanan güvenlik özellikleri hakkında bilgi edinin.
ms.openlocfilehash: 587d80c27f867a387c901d23f4ec05f3c5905bf6
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48843498"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium güvenlik ve uyumluluk özellikleri

Microsoft 365 Iş ekstra, PC, telefon ve tabletlerde verilerinizi korumaya yardımcı olmak için basitleştirilmiş güvenlik özellikleri sunar.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 Yönetim Merkezi güvenlik özellikleri

Yönetim merkezinde Microsoft 365 Iş ekstra güvenlik özelliklerinin çoğunu, bu özellikleri açmanız veya kapatmanızı sağlayan basitleştirilmiş bir yol veren bir çoğunu yönetebilirsiniz. Yönetim merkezinde aşağıdakileri yapabilirsiniz:
  
- [Android veya iOS cihazları için uygulama yönetimi ayarlarını](app-protection-settings-for-android-and-ios.md) yapın. 
    
    Bu ayarlar, bir süre sonra etkin olmayan aygıttaki dosyaları silme, iş dosyalarını şifreleme
    
- [Windows 10 cihazlarında uygulama koruma ayarlarını](protection-settings-for-windows-10-devices.md) yapın. 
    
    Bu ayarlar, şirkete ait veya kişisel olarak sahip olunan cihazlarda şirket verilerine uygulanabilir.
    
- [Windows 10 cihazlarında cihaz koruma ayarlarını](protection-settings-for-windows-10-pcs.md) yapın. 
    
    Bir cihazın kaybolması veya çalınması durumunda verilerin korunmasına yardımcı olmak için [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) şifrelemesini etkinleştirebilir ve [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) 'ı fidye aşamalarına karşı gelişmiş koruma sağlar. 
    
- [Cihazlardan şirket verilerini kaldırma](remove-company-data.md)
    
    Bir cihaz kaybolmuşsa, çalınırsa veya bir çalışanın şirketinizi terk ettiğinde şirket verilerini uzaktan silebilirsiniz.
    
- [Windows 10 cihazlarını fabrika ayarlarına sıfırlayın](reset-devices-to-factory-settings.md) . 
    
    Cihaz koruma ayarları uygulanmış olan tüm Windows 10 cihazlarını sıfırlayabilirsiniz.
    
## <a name="additional-security-features"></a>Ek güvenlik özellikleri 

Microsoft 365 Business Premium 'daki gelişmiş özellikler, işletmenizi sanal tehditlere karşı korumaya yardımcı olmak ve hassas bilgileri korumak için kullanılabilir.
  
- **[Office için Microsoft Defender 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Office 365 için Microsoft Defender, iş veya müşteri bilgilerini tehlikeye atabilir Özellikler şunlardır:
    
  - Tehlikeli iletileri algılayıp atmak için gelişmiş ek taraması ve AI destekli çözümleme.
    
  - E-postadaki bağlantıların, kimlik avı düzeninin bir parçası olup olmadıklarını değerlendirmek için otomatik olarak gözden geçirmeleri. Bu, güvenli olmayan Web sitelerine erişiminizi güvende tutar.

- **[Azure portalında Intune 'un tüm özellikleri](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Azure portalında Intune yönetim merkezine erişmek için, Microsoft 365 Yönetim Merkezi aracılığıyla kullanılamayan MacOS cihazları, iPhone ve Android aygıtlarının yönetimi gibi ek güvenlik özelliklerini ayarlayabilirsiniz.
- **Azure AD Premium P1 planıyla aynı [koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)**


    Koşullu erişim, kuruluşunuzun oturum açma riskiyle korunmasını, beklenmeyen bir ağ veya yerel ayardan erişim girişimlerini, riskli cihaz türlerinden erişim girişimlerini vb. engellemeye yardımcı olabilir. İlk kimlik doğrulama tamamlandıktan sonra koşullu erişim ilkeleri zorlanır ve denenen erişimin onaylanması, reddedilmesi veya daha fazla kanıt (ikinci bir tanımlama biçimi gibi) gerekip gerekmediğini belirlemek için ilk kimlik doğrulama olayından sinyaller kullanır.

    Sağlanan koşullu erişim özellikleri şunlardır:

    - Kullanıcı adı, Grup ve role dayalı erişim
    - [Uygulamaya dayalı](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) erişim 
    - [Konuma göre erişim](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  yalnızca güvenilen IP aralıklarından veya belirli ülkelerden erişime izin verme 
    - Access için MFA gerektir
    - [Eski kimlik doğrulama](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) kullanan uygulamalara erişimi engelleyin
    - [Uygulama TP](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access) 'si
    - Örneğin, üçüncü taraf sağlayıcılarla MFA gibi özel kimlik doğrulama.
   
    Diğer özellikler:
    - Karma Azure AD için [self servis parola sıfırlama](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization)
    
## <a name="compliance-features"></a>Uyumluluk özellikleri

Microsoft 365 Business Premium aboneliğiniz, uyumluluk ve mevzuat standartlarını korumanıza yardımcı olan özellikler içerir.

- **[Veri kaybına](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** karşı koruma ilkelerine (DLP) genel bakış. 
    
    Şirketinizin dışından yanlışlıkla paylaşılmasını önleyecek şekilde, kredi kartı numaraları, sosyal güvenlik numaraları gibi hassas bilgileri otomatik olarak algılamak için DLP ayarlayabilirsiniz.
    
- **[Exchange Online Arşivleme](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online arşivleme lisansı iletileri sürekli veri yedekleme ile kolayca arşivlenebilir. Daha sonra bulma veya geri yükleme için gerekli olmaları durumunda, tüm kullanıcı e-postalarını silinen öğeler de içinde depolar. Ayrıca, bir dava bekletme ilkesini korumak için e-posta verilerini korumak, eBulma veya uyumluluk gereksinimlerini karşılamak üzere farklı bekletme ilkeleri kullanabilirsiniz.
    
- **[Duyarlılık etiketleri](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Iş ekstra, [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407)' in tüm özelliklerini içerir. Bu planla, e-posta ve belgelerdeki hassas bilgilere erişimi denetlemenize olanak tanıyan **duyarlılık etiketleri** oluşturabilirsiniz; "iletme" ve "kopyalama yapma" gibi denetimler. Ayrıca hassas bilgileri "gizli" olarak sınıflayabilir ve sınıflandırılmış bilgilerin iş dışından nasıl paylaşılacağını belirtebilirsiniz. Kurumsal düzeyde şifreleme, bilgilerinizi özel tutmak için e-posta ve belgelere uygulamak kolaydır. Office uygulamaları için Azure Information Protection istemci eklentisini de yükleyebilirsiniz. Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Duyarlılık etiketleri için **AzInfoProtection_UL.exe** yükleyin.

Bu özellikleri Güvenlik &amp; Uyumluluk Merkezi 'nde ve Intune yönetim merkezinde yönetebilirsiniz. Zaman içinde, Basitleştirilmiş denetimler Microsoft 365 yönetim merkezine eklenir.
  
    
## <a name="faq"></a>SSS

 ### <a name="are-these-security-features-available-in-all-markets"></a>Bu güvenlik özellikleri tüm pazarlarda kullanılabilir mi?
  
Evet, bu özellikler Microsoft 365 Iş ekstra 'nın satıldığı tüm pazarlarda kullanılabilir.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Güvenlik &amp; Uyumluluk merkezini nasıl bulabilirim?
  
1. Yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Business Premium 'Da oturum açın](https://portal.microsoft.com/) . 
    
2. Sol gezintide **Yönetim Merkezleri** 'ni bulun ve genişletin. 
    
    ![Microsoft 365 Yönetim merkezinde sol gezintide yönetim merkezleri 'ni seçin.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Güvenlik Uyumluluk Merkezi 'ne gitmek için **Güvenlik &amp; uyumluluğu** 'nı seçin &amp; .
