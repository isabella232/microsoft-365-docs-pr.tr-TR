---
title: Microsoft 365 Business 'da Azure AD ile birleştirilmiş cihazından şirket içi kaynaklara erişme
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
description: Bir Azure Active Directory 'de Windows 10 aygıtından iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim almayı öğrenin.
ms.openlocfilehash: 2144268f5cbab67c39d5902622c61c0c35e6481c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295320"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Microsoft 365 Business Premium 'da Azure AD ile birleştirilmiş cihazından şirket içi kaynaklara erişme

Bu makale Microsoft 365 Business Premium için geçerlidir.

Azure Active Directory 'deki herhangi bir Windows 10 aygıtının, Microsoft 365 uygulamalarınız gibi tüm bulut tabanlı kaynaklara erişimi vardır ve Microsoft 365 Business Premium tarafından korunabilir. Ayrıca, iş kolu (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim izni verebilirsiniz. Erişime izin vermek için, şirket içi Active Directory 'yi Azure Active Directory ile eşitlemek üzere [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) 'i kullanın. 

Daha fazla bilgi edinmek için [Azure Active Directory 'de cihaz yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction)konusuna bakın.
Adımlar aşağıdaki bölümlerde de özetlenmiştir.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connect 'i çalıştırır

Kuruluşunuzun Azure AD birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.
  
1. Kullanıcıları, grupları ve kişilerinizi yerel Active Directory 'den Azure Active Directory 'ye eşitlemek için, [Office 365 için dizin eşitlemeyi ayarlama](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)başlığı altında açıklandığı gibi dizin eşitleme Sihirbazı 'Nı ve Azure AD Connect 'i çalıştırabilirsiniz.
    
2. Dizin eşitleme işlemi tamamlandıktan sonra, kuruluşunuzun Windows 10 cihazlarının Azure AD 'de bulunduğundan emin olun. Bu adım her Windows 10 cihazında tek tek yapılır. Ayrıntılar için [Microsoft 365 Business Premium kullanıcıları Için Windows cihazlarını ayarlama](set-up-windows-devices.md) bölümüne bakın. 
    
3. Windows 10 cihazları Azure AD 'e eklendiğinde, her kullanıcının cihazlarını yeniden başlatması ve Microsoft 365 Iş ekstra kimlik bilgileriyle oturum açması gerekir. Tüm aygıtların artık şirket içi kaynaklara erişimi vardır.
    
Azure AD birleştirilmiş cihazları için şirket içi kaynaklara erişim için ek adım gerekmez. Bu işlev Windows 10 ' da yerleşiktir. 

WHFB kimlik bilgisi oturumu aracılığıyla PIN/Bio-metrik gibi parola yöntemi dışında, AYARLANABILIR bir cihazda oturum açma planınız varsa ve şirket içi kaynaklara (paylaşımlar, yazıcılar... vb), lütfen takip edin https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Kuruluşunuz, yukarıda açıklanan Azure AD birleştirilmiş cihaz yapılandırmasında dağıtmaya hazır değilse, [karma Azure AD birleştirilmiş cihaz yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünebilirsiniz.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Windows cihazları Azure AD 'ye katıldığınızda dikkat edilecek noktalar

Azure-AD 'a katıldığınız Windows cihazı daha önce etki alanına veya bir çalışma grubunda yer alıyorsa aşağıdaki sınırlamaları dikkate alın:
  
- Bir cihaz Azure AD birleştirdiğinde, var olan bir profile başvurulmadan yeni bir kullanıcı oluşturur. Profiller el ile geçirilmesi gerekir. Kullanıcı profili, sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgileri içerir. En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için üçüncü taraf bir aracı bulmalıdır.

- Cihaz grup Ilkesi nesnelerini (GPO) kullanıyorsa, bazı GPO 'Larda karşılaştırılabilir bir [yapılandırma hizmeti sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir. Var olan GPO 'Lara benzer CSP 'Leri bulmak için [Mvade aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırabilirsiniz.

- Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulaması yapamaz. Eski uygulamayı değerlendirin ve mümkünse modern kimlik doğrulama kullanan bir uygulamaya güncelleştirmeyi düşünebilirsiniz.

- Active Directory yazıcı keşfi çalışmaz. Tüm kullanıcılar için doğrudan yazıcı yolları sağlayabilir veya [karma bulut yazdırma](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)kullanabilirsiniz.
