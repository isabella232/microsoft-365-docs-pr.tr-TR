---
title: Şirket içinde Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara Microsoft 365 İş
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: İş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara bir Azure Active Directory bir Windows 10 öğrenin.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843332"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Şirket içinde Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara Microsoft 365 İş Ekstra

Bu makale diğer Microsoft 365 İş Ekstra.

Bir Windows 10 bağlı Azure Active Directory cihaz, Microsoft 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişim iznine sahip olur ve Microsoft 365 İş Ekstra. Ayrıca iş alanı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim izni de veebilirsiniz. Erişime izin vermek [için, Azure AD Bağlan'i](/azure/active-directory/connect/active-directory-aadconnect) kullanarak şirket içi Active Directory'nizi diğer Azure Active Directory.

Daha fazla bilgi edinmek için [bkz. Azure Active Directory'da cihaz yönetimine giriş.](/azure/active-directory/device-management-introduction)
Adımlar aşağıdaki bölümlerde da özetlenmiştir.

## <a name="run-azure-ad-connect"></a>Azure AD Bağlan'i çalıştırma

Azure AD'ye katılmış cihazlarının şirket içi kaynaklara erişmesi için aşağıdaki adımları tamamlayın.

1. Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'e eşitlemek için, Office 365 için dizin eşitlemesini ayarlama konusunda açıklandığı gibi Dizin eşitleme sihirbazını Bağlan Azure AD [Office 365.](../enterprise/set-up-directory-synchronization.md)

2. Dizin eşitlemesi tamamlandıktan sonra, tüm kuruluş cihazlarında Azure AD'Windows 10 bağlı olduğundan emin olun. Bu adım her cihazda ayrı Windows 10 yapılır. Ayrıntılar [için Windows cihazları Microsoft 365 İş Ekstra'ya](set-up-windows-devices.md) bakın.

3. Cihaz Windows 10 Azure AD'ye katıldıktan sonra, her kullanıcının cihazlarını yeniden başlatması ve kendi kullanıcı kimlik bilgileriyle Microsoft 365 İş Ekstra gerekir. Tüm cihazlar artık şirket içi kaynaklara da erişime sahip.

Azure AD'ye katılmış cihazlar için şirket içi kaynaklara erişmek için ek adımlar gerekmez. Bu işlevsellik yeni bir Windows 10.

PIN/Biyometrik WHFB kimlik bilgileri aracılığıyla oturum açma gibi parola yöntemi dışında bir AADJ cihazında oturum açma ve ardından şirket içi kaynaklara (paylaşımlar, yazıcılar, vb.) erişme planlarınız varsa, lütfen bu [makaleyi izleyin.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

Organizasyon, yukarıda açıklanan Azure AD'ye katılmış cihaz yapılandırmasını dağıtmaya hazır değilse, Azure AD'ye Katılan Karma cihaz yapılandırmasını [ayarlamayı göz önünde bulundurabilirsiniz.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Windows cihazları Azure AD'ye katılırken dikkate alınacak noktalar

Azure-AD Windows katıldığınız tüm cihaz daha önce etki alanına katılmış veya bir çalışma grubunda yer alan bir cihazsa, aşağıdaki sınırlamaları göz önünde önünde Windows:

- Bir Azure AD birleştirme cihazı katsıyorsa, var olan profile başvurmak gerekmeden yeni bir kullanıcı oluşturur. Profillerin el ile geçişi gerekir. Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgileri içerir. Mevcut dosyaları ve ayarları yeni profile eşlemek için bir üçüncü taraf aracı bulmak en iyi yaklaşımdır.

- Cihaz Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPOS'ların Intune'da benzer bir Yapılandırma Hizmeti Sağlayıcısı [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) yok olabilir. Var olan [GPOS'lar](https://www.microsoft.com/download/details.aspx?id=45520) için karşılaştırılabilir CSP'leri bulmak için MMAT aracını çalıştırın.

- Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulaması işlemi görenemmektedir. Eski uygulamayı değerlendirin ve mümkünse modern Kimlik Doğrulaması kullanan bir uygulamaya güncelleştirin.

- Active Directory yazıcı bulma işe yaramadı. Tüm kullanıcılar için doğrudan yazıcı yolları s sağlamanın veya Evrensel [Yazdırma'nın kullanımını sebilirsiniz.](/universal-print/)

### <a name="related-articles"></a>İlgili Makaleler

[Azure AD aboneliğinin önkoşulları Bağlan](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
