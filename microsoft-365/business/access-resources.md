---
title: Microsoft 365 İş'te Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara erişme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Azure Active Directory'ye katılmış bir Windows 10 cihazından iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişmeyi öğrenin.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445358"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Microsoft 365 İş Ekstra'da Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara erişme

Bu makale Microsoft 365 İş Ekstra için geçerlidir.

Azure Active Directory'ye katılmış tüm Windows 10 cihazlarında, Microsoft 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişimi vardır ve Microsoft 365 İş Ekstra tarafından korunabilirsiniz. Ayrıca iş hattı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişime izin veabilirsiniz. Erişime izin vermek [için, Şirket içi](/azure/active-directory/connect/active-directory-aadconnect) Active Directory'nizi Azure Active Directory ile eşitlemek için Azure AD Connect'i kullanın. 

Daha fazla bilgi edinmek için [Bkz. Azure Active Directory'de cihaz yönetimine giriş.](/azure/active-directory/device-management-introduction)
Adımlar aşağıdaki bölümlerde de özetlenmiştir.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connect'i çalıştırma

Kuruma katılan Azure AD cihazlarının şirket içi kaynaklara erişmesi için aşağıdaki adımları tamamlayın.
  
1. Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'ye eşitlemek için, [Office 365](../enterprise/set-up-directory-synchronization.md)için dizin eşitlemesini ayarlama konusunda açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.
    
2. Dizin eşitlemesi tamamlandıktan sonra, kuruluşun Windows 10 cihazlarının Azure AD'ye katıldığından emin olun. Bu adım, her Windows 10 cihazında ayrı ayrı yapılır. Ayrıntılar [için Bkz. Microsoft 365 İş Ekstra kullanıcıları](set-up-windows-devices.md) için Windows cihazlarını ayarlama. 
    
3. Windows 10 cihazları Azure AD'ye katıldıktan sonra, her kullanıcının cihazlarını yeniden başlatması ve Microsoft 365 İş Ekstra kimlik bilgileriyle oturum açması gerekir. Artık tüm cihazlara şirket içi kaynaklara da erişebilirsiniz.
    
Azure AD'ye katılmış cihazlar için şirket içi kaynaklara erişmek için ek adım gerekmez. Bu işlev Windows 10'da yerleşik olarak yer alan bir işlevdir. 

WHFB kimlik bilgileriyle oturum açma yoluyla PIN/Biyometrik gibi parola yöntemi dışında AADJ cihazında oturum açma ve ardından şirket içi kaynaklara (paylaşımlar,yazıcılar) erişme planlarınız varsa. vb. gibi) lütfen https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Organizasyonunız yukarıda açıklanan Azure AD'ye katılmış cihaz yapılandırmasında dağıtmaya hazır değilse, Karma Azure AD Katıldı cihaz [yapılandırmasını ayarlamayı göz önünde bulundurabilirsiniz.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Windows cihazlarıyla Azure AD'ye katılırken dikkat edilmesi gereken noktalar

Azure-AD'ye katıldığınız Windows cihazı daha önce etki alanına katılmış veya bir çalışma grubunda yer alan bir cihazsa, aşağıdaki sınırlamaları göz önünde önünde önünde düşünün:
  
- Azure AD'nin bir cihaz birleştirmesi, var olan bir profile başvurmadan yeni bir kullanıcı oluşturur. Profillerin el ile geçirilir. Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlangıç menüsü ayarları gibi bilgileri içerir. Mevcut dosyaları ve ayarları yeni profile eşlemek için üçüncü taraf bir araç bulmak en iyi yaklaşımdır.

- Cihaz Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPOS'ların Intune'da karşılaştırılabilir bir Yapılandırma Hizmeti Sağlayıcısı [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olabilir. Mevcut [GPO'lar](https://www.microsoft.com/download/details.aspx?id=45520) için benzer CSP'leri bulmak için MMAT aracını çalıştırın.

- Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulamasına sahip olamayabilecektir. Eski uygulamayı değerlendirin ve mümkünse modern Kimlik Doğrulaması kullanan bir uygulamaya güncelleştirmeyi göz önünde bulundurabilirsiniz.

- Active Directory yazıcı bulma çalışmaz. Tüm kullanıcılar için doğrudan yazıcı yolları s sağlama veya [Evrensel Yazdırma'ı kullanabilirsiniz.](/universal-print/)

### <a name="related-articles"></a>İlgili Makaleler

[Azure AD Connect için önkoşullar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
