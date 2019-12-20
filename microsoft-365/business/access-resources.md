---
title: Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Windows 10 aygıtına katılan bir Azure Active Directory'den iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara nasıl erişebilirsiniz öğrenin.
ms.openlocfilehash: 89ac38f3da9cbdd3ff1a5eb33dc129d2e83521c7
ms.sourcegitcommit: 8c244b38c43dd00c4ef0102f8bed02ab36639a6b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39967173"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin

Azure Active Directory'nin birleştiği tüm Windows 10 aygıtları, Office 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişebilir ve Microsoft 365 Business tarafından korunabilir. Ayrıca, iş satırı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişime de izin verebilirsiniz. Erişime izin vermek için, şirket içi Active Directory'nizi Azure Etkin Dizini ile senkronize etmek için [Azure AD Connect'i](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) kullanın. 

Daha fazla bilgi için Azure [Active Directory'de aygıt yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction)'e bakın.
Adımlar da aşağıdaki bölümlerde özetlenmiştir.

> [!IMPORTANT]
> Bu yordam yalnızca OAuth ve NTLM için geçerlidir. Kerberos desteklenmiyor.
 
## <a name="run-azure-ad-connect"></a>Azure AD Connect çalıştırın

Kuruluşunuzun Azure AD'sinin birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.
  
1. Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.
    
2. Dizin eşitlemesi tamamlandıktan sonra, kuruluşunuzun Windows 10 aygıtlarının Azure AD'ye katıldığından emin olun. Bu adım her Windows 10 aygıtında ayrı ayrı yapılır. Ayrıntılar [için Microsoft 365 Business kullanıcıları için Windows aygıtları ayarlama'ya](set-up-windows-devices.md) bakın. 
    
3. Windows 10 aygıtları Azure AD'ye katıldıktan sonra, her kullanıcının aygıtlarını yeniden başlatması ve Microsoft 365 İş kimlik bilgileriyle oturum açması gerekir. Artık tüm aygıtlar şirket içi kaynaklara da erişebilir.
    
Azure AD'ye katılan aygıtlar için şirket içi kaynaklara erişmek için ek adım gerekmez. Bu işlev Windows 10'da yerleşiktir. 

WhFB kimlik bilgisi girişi ile PIN/Bio-metric gibi şifre yöntemi dışında AADJ cihazına giriş yapmayı planlıyorsanız ve şirket içi kaynaklara (paylaşımlar, yazıcılar) erişin. vb), lütfen izleyinhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Kuruluşunuz yukarıda açıklanan Azure AD birleştirilmiş aygıt yapılandırmasında kullanıma hazır değilse, [Karma Azure AD Joined aygıt yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünün.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Windows aygıtlarını Azure AD'ye katılırken dikkat edilmesi gerekenler

Azure-AD'nizin katıldığı Windows aygıtı daha önce etki alanına veya bir çalışma grubunda ysa, aşağıdaki sınırlamaları göz önünde bulundurun:
  
- Bir aygıt Azure AD katıldığında, varolan bir profile başvurmadan yeni bir kullanıcı oluşturur. Profiller el ile geçirilmelidir. Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgiler içerir. En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için bir üçüncü taraf aracı bulmaktır.

- Aygıt Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPO'larda Intune'da karşılaştırılabilir bir [Yapılandırma Hizmet Sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir. Mevcut GPO'lar için karşılaştırılabilir CSP'ler bulmak için [MMAT aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırın.

- Kullanıcılar Active Directory kimlik doğrulamasına bağlı olan uygulamaların kimliğini doğrulayamaz. Eski uygulamayı değerlendirin ve mümkünse modern Auth kullanan bir uygulamaya güncelleştirmeyi düşünün.

- Etkin Dizin yazıcısı bulma çalışmaz. Tüm kullanıcılar için doğrudan yazıcı yolları sağlayabilir veya [Karma Bulut Yazdırma'yı](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)kullanabilirsiniz.
