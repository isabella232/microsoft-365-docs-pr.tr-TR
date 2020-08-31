---
title: İş için Microsoft 365 kullanmaya başlama
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
description: İş için Microsoft 365 hakkında bilgi edinin, bu uygulamayı nasıl ayarlayabilirim ve kullanıcıların cihazlarından ve PC 'larından işletmeler için Microsoft 365 tarafından korunduğundan emin olun.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306499"
---
# <a name="get-started-with-microsoft-365-for-business"></a>İş için Microsoft 365 kullanmaya başlama

## <a name="what-is-microsoft-365-for-business"></a>İş için Microsoft 365 nedir?

İş için Microsoft 365, her zaman güncel olan Outlook, Word, Excel ve diğer Office ürünleri gibi kapsamlı bir iş verimliliği ve işbirliği araçları kümesidir. İş dosyalarınızı tüm iOS, Android ve Windows 10 cihazlarınızda, yönetimi kolay olan kurumsal güvenlik güvenliğiyle koruyabilir.

Microsoft 365 iş 'e hızlı bir genel bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 işletmeler için 300 lisans sağlanmıştır. Daha fazla lisansa ihtiyacınız varsa daha fazla bilgi için [Microsoft 365 Kurumsal](https://go.microsoft.com/fwlink/p/?linkid=860986) belgelerine göz atın. 
  
## <a name="get-microsoft-365-for-business"></a>İş için Microsoft 365

- İş ortağınız varsa 365, Microsoft iş [Ortağı Merkezi 'nden iş için microsoft 365](get-microsoft-365-business.md).
    
- İş ortağınız yoksa ve Microsoft 365 iş 'i edinmek istiyorsanız, [buradan satın](https://www.microsoft.com/microsoft-365/business)alabilirsiniz.
    
## <a name="set-up-microsoft-365-for-business"></a>Microsoft 365 iş 'i ayarlama

 **İş için Microsoft 365 kurulumu**
  
Aşağıdaki diyagramda, yöneticilerin Microsoft 365 iş için nasıl ayarlandığı açıklanmaktadır. Ayrıca, Microsoft 365 iş için Windows bilgisayarlarını hazırlama adımlarını da açıklar. Microsoft 365 Yönetim Merkezi 'nde [Windows Autopilot](add-autopilot-devices-and-profile.md)ile yeni aygıtlar da ekleyebilirsiniz. Bir Kullanıcı Microsoft 365 iş kimlik bilgileriyle oturum açtığında, üretken olmaları için yeni cihazları ayarlamak ve önceden yapılandırmak üzere AutoPilot 'ı kullanabilirsiniz.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

İş için Microsoft 365 'e genel bir bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Microsoft 365 iş 'i ayarlama (yönetici)

Genel yönetici kimlik bilgilerinizle [microsoft 365 Yönetim Merkezi](https://portal.office.com/adminportal/home) 'nde oturum açın ve Microsoft 365 iş için ayarlamak üzere aşağıdaki adımları tamamlayın. 
  
1. [Microsoft 365 iş 'te cihazlarda verileri koruma önkoşulları](pre-requisites-for-data-protection.md)
    
    Cihazınızın Microsoft 365 iş için hazır olduğundan emin olmak için öncelikle önkoşulları okuyun.
    
2. [Microsoft 365 iş 'i ayarlamak için kurulum sihirbazını kullanma](set-up.md)
    
    **Bir yerel Active Directory 'den buluta kalıcı olarak taşınmıyorsanız**, Microsoft 365 Yönetim Merkezi 'ne gidebilir ve Kurulum Sihirbazı 'nı kullanarak, kullanıcılarınızı el ile ekleyebilir veya Azure AD Connect ile bir kerelik eşitleme yapabilirsiniz. Bunu yapmanın iki yolu vardır: 
    
    - Ayrıca Exchange 2010, Exchange 2013 veya Exchange 2016 sunucunuz varsa, [Exchange posta kutularını hızla 365 Microsoft 'a geçirmek Için en az karma kullanabilirsiniz](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). En az karma adımlarda, kullanıcılardan Azure AD 'ye bir kerelik eşitleme ve şirket içi 'tan buluta e-posta geçişi dahildir. E-posta geçişi tamamlandıktan sonra, bu yöntemi kullandığınızda dizin eşitlemesi otomatik olarak kapatılır.
    
    - Kullanıcılarınızı bulut ile eşitlemek için Dizin eşitleme Sihirbazı 'nı kullanın. Bu süreci tamamlamak için [Microsoft 365 için dizin eşitlemesini ayarlama](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) bölümündeki adımları izleyin. Kullanıcılarınızı bulut ile eşitledikten sonra, [Microsoft 365 için dizin eşitlemesini](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization)kapatmanız gerekir.
    
    Bu şekilde, bir Microsoft 365 kullanıcısına bu şekilde eklenen her kullanıcıya da izin vermeniz gerekir. Bu işlemi [Kurulum sihirbazında](set-up.md) yapabilir veya [kullanıcılara lisans atayabilirsiniz](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: mobil cihazları hazırlama

[Microsoft 365 iş kullanıcıları için mobil cihazları ayarlama](set-up-mobile-devices.md) konusundaki adımları izleyerek Office uygulamalarını cihazlara yükleyebilir ve Microsoft 365 iş için korunduğundan emin olun. 
  
### <a name="3-prepare-pcs"></a>3: bilgisayarları hazırlama

Yöneticiler, [Windows Autopilot](add-autopilot-devices-and-profile.md)kullanarak yeni Windows 10 PC 'lerin ayarlarını önceden seçebilir. Kullanıcılar, bu konudaki adımları izleyerek mevcut veya yeni Windows 10 cihazlarını ayarlayabilir: [iş Için Microsoft 365 Windows bilgisayarlarını ayarlama](set-up-windows-devices.md). Var olan cihazlarda, kullanıcılar **isteğe bağlı olarak** [dosyaları OneDrive iş 'e taşıyabilir](move-files-to-onedrive.md). Windows profiliyle ilişkili dosyaları OneDrive 'a taşımak için üçüncü taraf araçları da kullanabilirler.
  
Kuruluşunuzda Windows Server Active Directory 'yi şirket içinde kullanıyorsanız, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürmek için Microsoft 365 iş için iş 'i ayarlayabilirsiniz. [Etki alanı odaklı Windows 10 cihazlarının iş Için Microsoft 365 tarafından yönetilmesini etkinleştirme](manage-windows-devices.md) konusundaki adımları izleyin. Bu yöntem tercih edilir ve bu durumdaki cihazlar **karma Azure AD birleştirilmiş cihazları**olarak adlandırılır. 
  
Bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory 'yi korumanız durumunda, buradaki adımları izleyerek **Azure AD-birleştirilmiş cihazlarınıza** bu kaynaklar için erişim sağlayabilirsiniz: [Şirket Içi 365 kaynaklara erişim](access-resources.md)sağlayın.
  
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- İş için Microsoft 365, müşteri desteği ekibimize erişiminiz vardır: ** [iş ürünleri Için desteğe başvurun-Yönetici Yardımı](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Ayrıca bkz.

[İş belgeleri ve kaynaklar için Microsoft 365](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[İş için 365 microsoft](manage.md)[365 iş 'i](migrate-to-microsoft-365-business.md) yönetme

[Microsoft 365 iş eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
