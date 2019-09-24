---
title: Microsoft 365 İş güvenliği ve uyumluluk özellikleri
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Microsoft 365 Business ile birlikte gelen güvenlik özellikleri hakkında bilgi edinin.
ms.openlocfilehash: 6b8fc215b95913e1beef3a3715119b947a7af406
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121168"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 İş güvenliği ve uyumluluk özellikleri

Microsoft 365 Business, bilgisayar, telefon ve tabletlerdeki verilerinizin korunmasına yardımcı olmak için basitleştirilmiş güvenlik özellikleri sunar.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 İş yönetici merkezi güvenlik özellikleri

[![Yönetici merkezinin değiştiğini bildirmek için etiket ve aka.ms/aboutM365preview daha fazla ayrıntı bulabilirsiniz.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Bu özellikleri açmak veya kapatmak için basitleştirilmiş bir yol sağlayan microsoft 365 İş güvenliği özelliklerinin çoğunu yönetici merkezinde yönetebilirsiniz. Yönetici merkezinde aşağıdakileri yapabilirsiniz:
  
  
- [Android veya iOS aygıtları için uygulama yönetimi ayarlarını ayarlayın.](app-protection-settings-for-android-and-ios.md) 
    
    Bu ayarlar arasında, belirli bir süre sonra etkin olmayan bir aygıttan dosyaları silme, iş dosyalarını şifreleme, kullanıcıların PIN ayarlamalarını gerektirmevb.
    
- [Windows 10 aygıtları için uygulama koruma ayarlarını ayarlayın.](protection-settings-for-windows-10-devices.md) 
    
    Bu ayarlar, hem şirkete ait hem de kişisel olarak sahip olunan aygıtlarda şirket verilerine uygulanabilir.
    
- [Windows 10 aygıtları için aygıt koruma ayarlarını ayarlayın.](protection-settings-for-windows-10-pcs.md) 
    
    Bir aygıtın kaybolması veya çalınması durumunda verilerin korunmasına yardımcı olmak için [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) şifrelemesini etkinleştirebilir ve [Windows Exploit Guard'ın](https://go.microsoft.com/fwlink/p/?linkid=871404) fidye yazılımlarına karşı gelişmiş koruma sağlamasını sağlayabilirsiniz. 
    
- [Cihazlardan şirket verilerini kaldırma](remove-company-data.md)
    
    Bir aygıt kaybolursa, çalınırsa veya bir çalışan şirketinizden ayrılırsa şirket verilerini uzaktan silebilirsiniz.
    
- [Windows 10 aygıtlarını fabrika ayarlarına sıfırlayın.](reset-devices-to-factory-settings.md) 
    
    Aygıt koruma ayarları uygulanan windows 10 aygıtlarını sıfırlayabilirsiniz.
    
## <a name="additional-security-features"></a>Ek güvenlik özellikleri 

Microsoft 365 Business'taki gelişmiş özellikler, işletmenizi siber tehditlere karşı korumanıza ve hassas bilgileri korumanıza yardımcı olmak için kullanılabilir.
  
- **[Office 365 Gelişmiş Tehdit Koruması](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Gelişmiş Tehdit Koruması (ATP), çalışan veya müşteri bilgilerini tehlikeye atmak üzere tasarlanmış gelişmiş kimlik avı ve fidye yazılımı saldırılarına karşı işletmenizi korumaya yardımcı olur. Özellikler şunlardır:
    
  - Tehlikeli iletileri algılamak ve atmak için gelişmiş ek tarama ve AI destekli analiz.
    
  - Kimlik avı düzeninin parçası olup olmadıklarını değerlendirmek için e-postadaki bağlantıların otomatik denetimleri. Bu, güvenli olmayan web sitelerine erişmenizi sağlar.

- **[Azure portalında Intune'un tüm özellikleri](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Azure portalındaki Intune yönetici merkezine erişmek, MacOS aygıtlarının yönetimi, iPhone ve Android aygıtlarının yanı sıra Microsoft tarafından kullanılamayan Windows için gelişmiş aygıt yönetimi gibi ek güvenlik özellikleri ayarlamanıza olanak tanır 365 İş yönetici merkezi.
- **Azure AD P1 planıyla Aynı [Koşullu Erişim](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview)**

    Koşullu Erişim, kuruluşunuzun oturum açma riskine karşı korunmasına, beklenmeyen bir ağdan veya yerel olarak erişim girişimlerine, erişim girişimlerinin riskli aygıt türleri oluşturmasına ve benzeri nedenlerle korunmasına yardımcı olabilir. Koşullu Erişim ilkeleri ilk kimlik doğrulama tamamlandıktan sonra uygulanır ve girişimde bulunulması onaylanması, reddedilmesi veya f daha fazla kanıt (ikinci kimlik biçimi gibi) olup olmadığını belirlemek için ilk kimlik doğrulama olayından gelen sinyalleri kullanır Gerekli.

    Koşullu erişim özellikleri şunlardır:

    - Kullanıcı adına, gruba ve role göre erişim
    - [Bir uygulamaya dayalı](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) erişim 
    - [Konuma göre erişim](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  yalnızca güvenilir IP aralıklarından veya belirli ülkelerden erişime izin 
    - Erişim için MFA gerektirir
    - [Eski kimlik doğrulaması](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) kullanan uygulamalara erişimi engelleme
    - Uygulamalar tp kullanımı [Intune uygulama koruması](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access) gerektirir
    - Örneğin DUO, üçüncü taraf sağlayıcılarla MFA gibi özel kimlik doğrulaması.
   
    Diğer özellikler:
    - Karma Azure AD için [self servis parola sıfırlama](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization)
    
## <a name="compliance-features"></a>Uyumluluk özellikleri

Microsoft 365 Business aboneliğiniz, uyumluluk ve düzenleme standartlarını korumanıza yardımcı olan özellikler içerir.

- **[Veri kaybını önleme politikalarına genel bakış](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Kredi kartı numaraları, sosyal güvenlik numaraları, vb. gibi hassas bilgileri şirketiniz dışında yanlışlıkla paylaşmalarını önlemek için otomatik olarak algılamak için DLP'yi ayarlayabilirsiniz.
    
- **[Exchange Online Arşivleme](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Arşivleme lisansı, iletilerin sürekli veri yedekleme ile kolayca arşivlemesini sağlar. Daha sonra keşif veya geri yükleme için ihtiyaç duyulması durumunda, silinen öğeler de dahil olmak üzere kullanıcının tüm e-postalarını saklar. Ayrıca, e-posta verilerini dava tutma, eDiscovery veya uyumluluk gereksinimlerini karşılamak için korumak için farklı saklama ilkeleri kullanabilirsiniz.
    
- **[Azure Bilgi Koruması](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Bilgi koruması, e-posta ve belgelerdeki hassas bilgilere erişimi "İdem etmeyin" ve "Kopyalamayın" gibi denetimlerle kontrol etmemenize yardımcı olur. Ayrıca hassas bilgileri "Gizli" olarak sınıflandırabilir ve gizli bilgilerin işletmenin dışında ve içinde nasıl paylaşılabileceğini belirtebilirsiniz. Bilgilerinizi gizli tutmak için e-posta ve belgelere kurumsal sınıf şifreleme uygulamak kolaydır. Microsoft 365 Business, [Azure Bilgi Koruma Planı 1'in](https://go.microsoft.com/fwlink/p/?linkid=871407)tüm özelliklerini içerir. Office uygulamaları için Azure Bilgi Koruması istemci eklentisini de yükleyebilirsiniz. Daha fazla bilgi için [Azure Bilgi Koruması istemci yöneticisi kılavuzuna](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide)bakın.

Bu özellikleri Güvenlik &amp; Uyumluluğu merkezinde ve Intune yönetici merkezinde yönetebilirsiniz. Zamanla basitleştirilmiş denetimler Microsoft 365 Business yönetici merkezine eklenir.
  
    
## <a name="faq"></a>SSS

 ### <a name="are-these-security-features-available-in-all-markets"></a>Bu güvenlik özellikleri tüm pazarlarda kullanılabilir mi?
  
Evet, bu özellikler Microsoft 365 Business'ın satıldığı tüm pazarlarda kullanılabilir.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Güvenlik &amp; Uyumluluk merkezini nasıl bulabilirim?
  
1. Yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Business'ta oturum açın.](https://portal.microsoft.com/) 
    
2. Sol navigasyonda, **Yönetici merkezlerini** bulun ve genişletin. 
    
    ![Microsoft 365 yönetici merkezindeki sol gezinmede Yönetici merkezlerini seçin.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Güvenlik uyumluluk merkezine gitmek &amp; için **Güvenlik &amp; Uyumluluğu'ni** seçin.