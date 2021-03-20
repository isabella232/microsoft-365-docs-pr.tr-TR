---
title: Microsoft 365 İş ile çalışmaya başlama
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Microsoft 365 İş hakkında, ayarlama ve kullanıcılarınızı ve bilgisayarlarını Microsoft 365 İş tarafından korunacak şekilde hazırlama hakkında bilgi edinebilirsiniz.
ms.openlocfilehash: 9430dc7aa637be3fdb833150b83e96caacc82170
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912972"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Microsoft 365 İş ile çalışmaya başlama

## <a name="what-is-microsoft-365-for-business"></a>Microsoft 365 İş nedir?

İş için Microsoft 365, outlook, Word, Excel ve diğer Office ürünleri gibi her zaman güncel olan kapsamlı bir iş üretkenliği ve işbirliği araçları kümesidir. Yönetimi basit kurumsal sınıf güvenlikle tüm iOS, Android ve Windows 10 cihazlarınız için iş dosyalarınızı koruyabilirsiniz.

Microsoft 365 İş'e hızlı bir genel bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
İşletmeler için Microsoft 365, 300'e kadar lisans anlamına geliyor. Daha fazla lisansa ihtiyacınız varsa daha fazla bilgi için [Microsoft 365 Kurumsal](../enterprise/index.yml) belgelerine göz atın. 
  
## <a name="get-microsoft-365-for-business"></a>Microsoft 365 İş'i al

- bir iş ortağınız varsa, onlar Microsoft 365 İş'i edinecek: Microsoft İş Ortağı Merkezi'nden [Microsoft 365 İş'i edinin.](get-microsoft-365-business.md)
    
- İş ortağınız yoksa ve Microsoft 365 İş'i almak için buradan [satın alabilirsiniz.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>Microsoft 365 İş'i ayarlama

 **Microsoft 365 İş Paketi'nin ayarlanmış sürümüne genel bakış**
  
Aşağıdaki diyagramda yöneticilerin Microsoft 365 İş'i nasıl ayarlayaları açık bir şekilde açık almaktadır. Ayrıca, Windows bilgisayarlarını Microsoft 365 İş'e hazırlama adımları da açık almaktadır. Ayrıca, Microsoft 365 yönetim merkezinde Windows AutoPilot ile yeni [cihazlar da ebilirsiniz.](add-autopilot-devices-and-profile.md) AutoPilot'u kullanarak, kullanıcı microsoft 365 iş kimlik bilgileriyle oturum alar açmaz üretken kullanıma hazır olması için yeni cihazları ayarlar ve önceden yapılandırabilirsiniz.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Microsoft 365 İş kurulumuna genel bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Microsoft 365 İş'i ayarlama (Yönetici)

Genel yönetici [kimlik bilgilerinizle Microsoft 365](https://portal.office.com/adminportal/home) yönetim merkezinde oturum açma ve Microsoft 365 İş'i ayarlama adımlarını tamamlayın. 
  
1. [Microsoft 365 İş ile cihazlardaki verileri korumak için önkoşullar](pre-requisites-for-data-protection.md)
    
    Cihazlarınızı Microsoft 365 İş için hazır olduğundan emin olmak için önce önkoşulları okuyun.
    
2. [Microsoft 365 İş'i ayarlamak için kurulum sihirbazını kullanma](set-up.md)
    
    Yerel bir **Active Directory'den** buluta kalıcı olarak taşınıyorsanız, Microsoft 365 yönetim merkezine gidip kurulum sihirbazını kullanarak kullanıcılarınızı el ile ekleyebilir veya Azure AD Connect ile tek kullanımlık eşitleme yapabilirsiniz. Bunu yapmanın iki yolu vardır: 
    
    - Exchange 2010, Exchange 2013 veya Exchange 2016 sunucunuz varsa, Exchange posta kutularını [Microsoft 365'e](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate)hızla geçirmek için En Düşük Karma'nın kullanabilirsiniz. En düşük karma adım, kullanıcıların Azure AD'ye tek kullanımlık eşitlemesi ve şirket içi e-posta geçişini içerir. E-posta geçişi tamamlandıktan sonra, bu yöntemi kullanırsanız dizin eşitlemesi otomatik olarak kapalı olur.
    
    - Kullanıcılarınızı buluta eşitlemek için dizin eşitleme sihirbazını kullanın. Bu işlemi tamamlamak [için Microsoft 365 için dizin eşitlemesini](../enterprise/set-up-directory-synchronization.md) ayarlama makalesinde yer alan adımları izleyin. Kullanıcılarınızı buluta eşitledikten sonra, Microsoft 365 için dizin [eşitlemesini kapatmanız gerekir.](../enterprise/turn-off-directory-synchronization.md)
    
    Ayrıca, bu yolla eklenen her kullanıcıya microsoft 365 İş lisansı da ver gerekir. Bunu kurulum sihirbazında [veya kullanıcılara](set-up.md) lisans [atabilirsiniz.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobil cihazları hazırlama

İşletmeler için [Microsoft 365](set-up-mobile-devices.md) kullanıcılarının cihazlara Office uygulamalarını yüklemesi ve bunların Microsoft 365 İş tarafından korun olduğundan emin olmak için mobil cihazları ayarlama makalesinde yer alan adımları izleyin. 
  
### <a name="3-prepare-pcs"></a>3: Bilgisayarları hazırlama

Yöneticiler, [Windows AutoPilot'u](add-autopilot-devices-and-profile.md)kullanarak yeni Windows 10 bilgisayarları için ayarları önceden seçebilirsiniz. Kullanıcılar, bu konudaki adımları kullanarak mevcut veya yeni Windows 10 cihazlarını oluşturabilir: Microsoft 365 İş kullanıcıları için [Windows pc'leri ayarlama.](set-up-windows-devices.md) Var olan cihazlar için, kullanıcılar **isteğe bağlı** [olarak dosyaları OneDrive İş'e taşımaya devam eder.](move-files-to-onedrive.md) Ayrıca, Windows profiliyle ilişkili dosyaları OneDrive'a taşımak için üçüncü taraf araçlarını da kullanabilirler.
  
Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 İş'i kurabilirsiniz ve öte yandan da yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi koruyabilirsiniz. Bu ayarı yapmak [için etki alanına katılmış Windows 10 cihazlarını Microsoft 365](manage-windows-devices.md) İş tarafından yönetilsin. Bu yöntem tercih edilir ve bu durumdaki cihazlar Karma **Azure AD'ye** katılmış cihazlar olarak adlandırılan cihazlar. 
  
Bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'niz varsa, **Azure AD'ye** katılmış cihazlarınıza şu adımları takip edin: Microsoft [365](access-resources.md)İş'te Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara erişme.
  
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- İşletmeler için Microsoft 365 yöneticisi olarak, müşteri desteği ekibimize erişiminiz vardır: İş ürünleri için de destek ekibiyle iletişime geçin **[- Yönetici Yardımı](../admin/contact-support-for-business-products.md)**
    
## <a name="see-also"></a>Ayrıca bkz.

[İşletmeler için Microsoft 365 belgeleri ve kaynakları](./index.yml)
  
[Microsoft 365 İş'i yönetme](manage.md)[İş için Microsoft 365'e geçiş](migrate-to-microsoft-365-business.md)

[İş için Microsoft 365 eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)