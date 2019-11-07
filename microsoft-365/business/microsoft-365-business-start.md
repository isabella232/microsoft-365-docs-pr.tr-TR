---
title: Microsoft 365 İş ile çalışmaya başlama
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Microsoft 365 Business'ı ayarlamayı öğrenin.
ms.openlocfilehash: 4c744d6a900dba3c11ee51e75602a430268e15bb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38029114"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 İş ile çalışmaya başlama

## <a name="what-is-microsoft-365-business"></a>Microsoft 365 İş nedir?

Microsoft 365 İş, sürekli güncelleştirilen Outlook, Word, Excel ve diğer Office ürünlerini içeren bir grup kapsamlı iş üretkenliği ve işbirliği aracıdır. Tüm iOS, Android ve Windows 10 cihazlarınızdaki iş dosyalarınızı, yönetimi kolay kurumsal düzeyde bir güvenlikle koruyabilirsiniz.
  
Microsoft 365 İş 300 lisansa kadar yöneliktir, daha fazla lisansa ihtiyacınız varsa daha fazla bilgi için [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) belgelerine göz atın. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 İş'i edinme

- İş ortağınız varsa, onlar da Microsoft 365 İş ürününü alır: [Microsoft 365 İş'i Microsoft İş Ortağı Merkezi'nden alma](get-microsoft-365-business.md).
    
- İş ortağınız yoksa ve Microsoft 365 İş'i edinmek istiyorsanız, [buradan satın alabilirsiniz](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 İş'i ayarlama

 **Microsoft 365 Business Suite kurulumuna genel bakış**
  
Aşağıdaki diyagramda, yöneticilerin Microsoft 365 Business'ı nasıl kurdukları açıklanmaktadır. Ayrıca Windows bilgisayarları Microsoft 365 İş için hazırlama adımları da açıklanır. Ayrıca, [Windows AutoPilot](add-autopilot-devices-and-profile.md) ile Microsoft 365 İş yönetim merkezinde yeni cihazlar da ekleyebilirsiniz. AutoPilot'ı kullanarak yeni cihazları ayarlayıp önceden yapılandırabilir, böylece kullanıcı kendi Microsoft 365 İş kimlik bilgileriyle oturum açtığı anda cihazın üretimde kullanıma hazır olmasını sağlayabilirsiniz.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 Business (Yönetici) ayarlama

Genel yönetici kimlik bilgilerinizle [Microsoft 365 İş yönetim merkezinde](https://portal.office.com/adminportal/home) oturum açın ve Microsoft 365 İş'ı ayarlamak için aşağıdaki adımları tamamlayın. 
  
1. [Cihazlardaki verileri Microsoft 365 İş ile korumanın önkoşulları](pre-requisites-for-data-protection.md)
    
    Önkoşulları okuyun ve cihazınızın Microsoft 365 İş için hazır olduğundan emin olun.
    
2. [Microsoft 365 İş'i kurulum sihirbazını kullanarak ayarlama](set-up.md)
    
    **Yerel bir Active Directory'den buluta kalıcı olarak taşınıyorsanız,** kurulum sihirbazını kullanarak kullanıcılarınızı Microsoft 365 İş yöneticisi merkezine el ile ekleyebilir veya Azure AD Connect ile tek seferlik eşitleme yapabilirsiniz. Bunu yapmanın iki yolu vardır: 
    
  - Exchange 2010, Exchange 2013 veya Exchange 2016 sunucunuz da varsa, [Exchange posta kutularını Office 365'e hızla geçirmek için Minimal Karma'yı kullanabilirsiniz.](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef) Düşük karma adımlarında, kullanıcıların Azure AD ile tek seferlik eşitlenmesinin yanı sıra şirket içi e-postaları buluta geçirme işlemleri bulunur. Bu yöntem kullanıldığında, e-posta geçişi tamamlandıktan sonra dizin eşitleme otomatik olarak kapatılır.
    
  - Kullanıcılarınızı buluta eşitlemek için Office 365 dizin eşitleme sihirbazını kullanın. Bu işlemi tamamlamak üzere [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) bölümündeki adımları izleyin. Kullanıcılarınızı buluta eşitledikten sonra [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Ayrıca, bu yolla eklenen her kullanıcıya bir Microsoft 365 İş lisansı vermeniz gerekir. Bunu [kurulum sihirbazında](set-up.md)veya iş [için Office 365'teki kullanıcılara lisans atama'da](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)yapabilirsiniz.
    
### <a name="2-prepare-mobile-devices"></a>2: Mobil cihazları hazırlama

Office uygulamalarını aygıtlara yüklemeleri ve Microsoft 365 Business tarafından korunduklarını sağlamaları[için Microsoft 365 Business kullanıcılarıiçin mobil aygıtlar ayarlama](set-up-mobile-devices.md) adımlarını izleyin. 
  
### <a name="3-prepare-pcs"></a>3: Hazırlayın CD'ler

Yöneticiler, [Windows AutoPilot'u](add-autopilot-devices-and-profile.md)kullanarak yeni cihazlar için windows 10 bilgisayarları ayarlarını önceden seçebilirler. Kullanıcılar bu konudaki adımları izleyerek mevcut veya yeni Windows 10 aygıtlarını ayarlayabilir: [Microsoft 365 Business kullanıcıları için Windows bilgisayarları ayarlayın.](set-up-windows-devices.md) Mevcut aygıtlar için kullanıcılar dosyaları **Isteğe bağlı olarak**[İş Için OneDrive'a taşıyabilirler.](move-files-to-onedrive.md) Windows profiliyle ilişkili dosyaları OneDrive'a taşımak için üçüncü taraf araçlarını da kullanabilirler.
  
Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz. Bunu ayarlamak için [Microsoft 365 Business tarafından yönetilecek etki alanına birleştirilmiş Windows 10 aygıtlarını etkinleştir](manage-windows-devices.md) metodu adımlarını izleyin. Bu tercih edilen yöntemdir ve bu durumdaki aygıtlar **Karma Azure AD birleştirilmiş aygıtlar**olarak adlandırılır. 
  
Bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Etkin Dizin'i korursanız, **Azure AD'ye katılan aygıtlarınıza** bu kaynaklara buradaki adımları izleyerek erişim sağlayabilirsiniz: [Şirket içi kaynaklara bir Microsoft 365 Business'ta Azure AD'ye bağlı aygıt.](access-resources.md)
  
Windows 10 bilgisayarlarına yükledikten sonra Office'i aygıtlara [otomatik olarak yükleyebilirsiniz.](auto-install-or-uninstall-office.md) 
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- Microsoft 365 Business yöneticisi olarak, müşteri destek ekibimize, ** [iş ürünleri için başvuru desteğine](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) erişebilirsiniz - Yönetici Yardımı**
    
## <a name="related-topics"></a>İlgili Konular
[Microsoft 365 İş belgeleri ve kaynakları](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 İş yönetimi](manage.md)[Microsoft 365 İş'e geçiş](migrate-to-microsoft-365-business.md)
  

