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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Microsoft 365 Business'ı ayarlamayı öğrenin.
ms.openlocfilehash: 32bb30208083c4f62dd449290a7c9f5d8c725631
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831423"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 İş ile çalışmaya başlama

## <a name="what-is-microsoft-365-business"></a>Microsoft 365 İş nedir?

Microsoft 365 Business, Outlook, Word, Excel ve diğer Office ürünleri gibi her zaman güncel olan kapsamlı bir iş üretkenliği ve işbirliği araçları kümesidir. İş dosyalarınızı tüm iOS, Android ve Windows 10 aygıtlarınızda, yönetilmesi kolay kurumsal sınıf güvenlikle koruyabilirsiniz.

Microsoft 365 Business'a hızlı bir genel bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business, 300'e kadar lisans içindir. Daha fazla lisansa ihtiyacınız varsa, daha fazla bilgi için [Microsoft 365 Kurumsal](https://go.microsoft.com/fwlink/p/?linkid=860986) belgelerine bakın. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 İş'i edinme

- Bir iş ortağınız varsa, Microsoft 365 Business: [Microsoft 365 Business'ı Microsoft İş Ortağı Merkezi'nden alın.](get-microsoft-365-business.md)
    
- İş ortağınız yoksa ve Microsoft 365 İş'i edinmek istiyorsanız, [buradan satın alabilirsiniz](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 İş'i ayarlama

 **Microsoft 365 Business Suite kurulumuna genel bakış**
  
Aşağıdaki diyagramda, yöneticilerin Microsoft 365 Business'ı nasıl kurdukları açıklanmaktadır. Ayrıca Windows bilgisayarları Microsoft 365 İş için hazırlama adımları da açıklanır. Ayrıca [Windows AutoPilot](add-autopilot-devices-and-profile.md)ile Microsoft 365 İş admin merkezine yeni cihazlar ekleyebilirsiniz. Yeni aygıtları, kullanıcı Microsoft 365 Business kimlik bilgilerini girer almaz verimli kullanıma hazır olacak şekilde ayarlamak ve önceden yapılandırmak için Otomatik Pilot'u kullanabilirsiniz.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Microsoft 365 İş kurulumuna genel bir bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Bu videoyu yararlı bulduysanız, [küçük işletmeler ve Microsoft 365'e yeni katılanlar için tam eğitim serisine](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)göz atın.

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 Business (Yönetici) ayarlama

Global yönetici kimlik bilgilerinizle [Microsoft 365 Business yönetici merkezinde](https://portal.office.com/adminportal/home) oturum açın ve Microsoft 365 Business'ı kurmak için aşağıdaki adımları tamamlayın. 
  
1. [Microsoft 365 Business ile cihazlardaki verileri korumak için ön koşullar](pre-requisites-for-data-protection.md)
    
    Aygıtlarınızın Microsoft 365 Business için hazır olduğundan emin olmak için önce ön koşulları okuyun.
    
2. [Microsoft 365 Business'ı kurmak için kurulum sihirbazını kullanın](set-up.md)
    
    Yerel bir **Active Directory'den buluta kalıcı olarak hareket**ediyorsanız, Microsoft 365 İş yöneticisi merkezine gidebilir ve kullanıcılarınızı el ile eklemek için kurulum sihirbazını kullanabilir veya Azure AD Connect ile tek seferlik eşitleme yapabilirsiniz. Bunu yapmanın iki yolu vardır: 
    
    - Exchange 2010, Exchange 2013 veya Exchange 2016 sunucunuz da varsa, [Exchange posta kutularını Office 365'e hızla geçirmek için Minimal Karma'yı kullanabilirsiniz.](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef) En az karma adımlar, kullanıcıların Azure AD ile tek seferlik eşitlemeyi ve şirket içi buluta e-posta geçişini içerir. E-posta geçişi tamamlandıktan sonra, bu yöntemi kullandığınızda dizin eşitlemesi otomatik olarak kapatılır.
    
    - Kullanıcılarınızı bulutla eşitlemek için Office 365 dizin eşitleme sihirbazını kullanın. Bu işlemi tamamlamak üzere [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) bölümündeki adımları izleyin. Kullanıcılarınızı bulutla eşitledikten sonra [Office 365 için dizin eşitlemesi kapatmanız](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d)gerekir.
    
    Bu şekilde eklenen her kullanıcıya Microsoft 365 Business'a bir lisans da vermeniz gerekir. Bunu [kurulum sihirbazında](set-up.md) yapabilir veya [iş için Office 365'teki kullanıcılara lisans atayabilirsiniz.](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobil cihazları hazırlama

Office uygulamalarını aygıtlara yüklemeleri ve Microsoft 365 Business tarafından korunduklarına emin olmaları [için Microsoft 365 Business kullanıcıları için mobil aygıtlar ayarlama](set-up-mobile-devices.md) adımlarını izleyin. 
  
### <a name="3-prepare-pcs"></a>3: Hazırlayın CD'ler

Yöneticiler, [Windows AutoPilot'u](add-autopilot-devices-and-profile.md)kullanarak yeni Windows 10 bilgisayarları için ayarları önceden seçebilirler. Kullanıcılar bu konudaki adımları izleyerek mevcut veya yeni Windows 10 aygıtlarını ayarlayabilir: [Microsoft 365 Business kullanıcıları için Windows bilgisayarları ayarlayın.](set-up-windows-devices.md) Varolan aygıtlar için kullanıcılar **dosyaları isteğe bağlı olarak** [OneDrive for Business'a taşıyabilir.](move-files-to-onedrive.md) Windows profiliyle ilişkili dosyaları OneDrive'a taşımak için üçüncü taraf araçlarını da kullanabilirler.
  
Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz. Bunu ayarlamak için [Microsoft 365 Business tarafından yönetilecek etki alanına birleştirilmiş Windows 10 aygıtlarını etkinleştir](manage-windows-devices.md) metodu adımlarını izleyin. Bu yöntem tercih edilir ve bu durumdaki aygıtlar **Karma Azure AD birleştirilmiş aygıtlar**olarak adlandırılır. 
  
Bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Etkin Dizin'i korursanız, **Azure AD'ye katılan aygıtlarınıza** buradaki adımları izleyerek bu kaynaklara erişim sağlayabilirsiniz: [Microsoft 365 Business'taki Azure AD'ye bağlı bir aygıttan şirket içi kaynaklara erişin.](access-resources.md)
  
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- Microsoft 365 Business yöneticisi olarak, müşteri destek ekibimize erişebilirsiniz: ** [İş ürünleri için destekle iletişim e-cevap - Yönetici Yardımı](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>See also

[Microsoft 365 İş belgeleri ve kaynakları](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 İş yönetimi](manage.md)[Microsoft 365 İş'e geçiş](migrate-to-microsoft-365-business.md)

[Microsoft 365 İş eğitim videoları](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
