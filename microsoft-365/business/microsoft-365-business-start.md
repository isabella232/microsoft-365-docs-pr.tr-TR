---
title: Microsoft 365 İş ile çalışmaya başlama
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: İşletmeler Microsoft 365, nasıl kuracaklarını, kullanıcılarınızı cihaz ve bilgisayarları kurumsal cihazlarla korunacak şekilde nasıl hazırlayacaklarını Microsoft 365 öğrenin.
ms.openlocfilehash: cc54147e75a27fbb93255d6f706b4f9044c75858
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245134"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 İş ile çalışmaya başlama

## <a name="what-is-microsoft-365-for-business"></a>İşletmeler Microsoft 365 nedir?

Microsoft 365, her zaman güncel olan Outlook, Word, Excel ve diğer Office ürünleri gibi bir dizi kapsamlı iş üretkenliği ve işbirliği aracıdır. Tüm iOS, Android ve Windows 10 cihazlarınız üzerinde iş dosyalarınızı, yönetimi kolay kurumsal sınıf bir güvenlikle koruyabilirsiniz.

kurumsal e-ticarete hızlı bir genel bakış için Microsoft 365 izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 lisansı, 300'e kadar lisansa kadar anlamına geliyor. Daha fazla lisansa ihtiyacınız varsa daha fazla bilgi için [Microsoft 365 Kurumsal](../enterprise/index.yml) belgelerine göz atın. 
  
## <a name="get-microsoft-365-for-business"></a>İş için Microsoft 365'i elde Microsoft 365

- İş ortağınız varsa, onlar da iş Microsoft 365 edinecek: [Microsoft Microsoft 365 Merkezinden iş için iş için yardım al](get-microsoft-365-business.md).
    
- İş ortağınız yoksa ve iş Microsoft 365 almak Microsoft 365, buradan [satın alabilirsiniz.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>İşletmeler Microsoft 365 ayarlama

 **İşletmeler için Microsoft 365 Paketi'nin ayarlaması hakkında genel bakış**
  
Aşağıdaki diyagramda, yöneticilerin iş için iş için Microsoft 365 ayarlanmıştır. Ayrıca, iş için PCleri hazırlama Windows adımlar da Microsoft 365 açıklarıdır. AutoPilot ile birlikte yönetim merkezinde Microsoft 365 cihazlar [da Windows abilirsiniz.](add-autopilot-devices-and-profile.md) AutoPilot'i kullanarak, yeni cihazları ayarlandıktan ve önceden yapılandırarak, kullanıcı kurumsal kimlik bilgileri için kendi Microsoft 365 anda üretken kullanıma hazır olur.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

kurumsal kurulum ayarlarına genel bir bakış için Microsoft 365 bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: İş Microsoft 365 ayarlama (Yönetici)

Genel yönetici [Microsoft 365 bilgilerinizle](https://portal.office.com/adminportal/home) yönetim merkezinde oturum açma ve kurumsal yönetim bilgilerini ayarlamak için Microsoft 365 tamamlayın. 
  
1. [Cihazlardaki verileri iş için Microsoft 365 korumak için önkoşullar](pre-requisites-for-data-protection.md)
    
    Cihazlarınızı kurumsal kullanıma hazır olduğundan emin olmak için önce önkoşulları Microsoft 365 okuyun.
    
2. [Kurumsal kurulum sihirbazını kullanarak Microsoft 365 ayarlama](set-up.md)
    
    Yerel bir **Active Directory'den** kalıcı olarak buluta taşınıyorsanız, Microsoft 365 yönetim merkezine gidip kullanıcılarınızı el ile eklemek için kurulum sihirbazını kullanabilir veya Azure AD ile tek seferlik eşitleme Bağlan. Bunu yapmanın iki yolu vardır: 
    
    - Exchange 2010, Exchange 2013 veya Exchange 2016 sunucunuz varsa, Exchange posta kutularını Microsoft 365'e hızlıca geçirmek için En Düşük [Karma'Exchange kullanabilirsiniz.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) Düşük karma adımlarında, kullanıcıların Azure AD'ye bir defalık eşitlemesi ve şirket içi e-postadan buluta geçiş işlemi yer alır. E-posta geçişi tamamlandıktan sonra, bu yöntemi kullanırsanız dizin eşitleme otomatik olarak kapanır.
    
    - Kullanıcılarınızı buluta eşitlemek için dizin eşitleme sihirbazını kullanın. Bu işlemi tamamlamak [üzere Microsoft 365](../enterprise/set-up-directory-synchronization.md) ayarlama konusunda adımları izleyin. Kullanıcılarınızı buluta eşitledikten sonra, eşitleme için Dizin [eşitlemesini kapatmanız Microsoft 365.](../enterprise/turn-off-directory-synchronization.md)
    
    Ayrıca, bu yolla eklenen her kullanıcıya iş için lisans Microsoft 365 gerekir. Bunu kurulum sihirbazında [veya Kullanıcılara](set-up.md) lisans [ata'da da yapabiliriz.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobil cihazları hazırlama

Kurumsal kullanıcılar için [Microsoft 365](set-up-mobile-devices.md) için mobil cihazları ayarlama Office uygulamalarını cihazlara yükleme ve bu uygulamaların Microsoft 365 tarafından korunduklarına emin olun. 
  
### <a name="3-prepare-pcs"></a>3: Bilgisayarları hazırlama

Yöneticiler [AutoPilot'a](add-autopilot-devices-and-profile.md)Windows 10 kullanarak yeni BILGISAYAR Windows önceden seçebilirsiniz. Kullanıcılar, şu konudaki adımları Windows 10 var olan veya yeni cihazlarında ayarlamalar yapabilirsiniz: Kurumsal kullanıcılar için [Windows Microsoft 365 pc'leri ayarlama](set-up-windows-devices.md). Var olan cihazlar için, kullanıcılar **isteğe bağlı** [olarak dosyaları OneDrive İş.](move-files-to-onedrive.md) Ayrıca, üçüncü taraf araçlarını kullanarak, bir profille ilişkili dosyaları Windows dosyaları başka OneDrive.
  
Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için işletmeler için Microsoft 365'i kurabilirsiniz ve bu sırada yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz. Bu özelliği ayarlamak için [Etki alanına katılmış Windows 10 cihazlarını işletmeler](manage-windows-devices.md) için Microsoft 365 tarafından yönetilsin mi? alanında yer alan adımları izleyin. Bu yöntem tercih edilir ve bu durumdaki cihazlar Karma **Azure AD'ye katılmış cihazlar olarak adlandırılan cihazlar.** 
  
Bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'niz **varsa, Azure AD'ye** katılmış cihazlarınıza buradaki adımları takip edin: İş için [Microsoft 365'te Azure AD'ye](access-resources.md)katılmış bir cihazdan şirket içi kaynaklara erişme .
  
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- İşletme Microsoft 365 yöneticisi olarak, müşteri desteği ekibimize erişiminiz vardır: İş ürünleri için destan ile iletişime **[geçin - Yönetici Yardımı](../admin/contact-support-for-business-products.md)**
    
## <a name="related-content"></a>İlgili içerik

[Microsoft 365 belgeleri ve kaynakları için belgeler](./index.yml)
  
[İşletmeler Microsoft 365'i yönetme](manage.md)[Microsoft 365 İş'e geçiş](migrate-to-microsoft-365-business.md)

[Microsoft 365 eğitimi videoları için video](../business-video/index.yml)