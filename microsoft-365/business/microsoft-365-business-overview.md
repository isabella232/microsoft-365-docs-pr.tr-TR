---
title: Microsoft 365 İş ile çalışmaya başlama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 9/20/2018
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Microsoft 365 iş öğrenin.
ms.openlocfilehash: ee15ffa98de032d7936d950124cdf772335949bd
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983290"
---
# <a name="get-started-with-microsoft-365-business"></a>Microsoft 365 İş ile çalışmaya başlama

## <a name="what-is-microsoft-365-business"></a>Microsoft 365 İş nedir?

Microsoft 365 İş, sürekli güncelleştirilen Outlook, Word, Excel ve diğer Office ürünlerini içeren bir grup kapsamlı iş üretkenliği ve işbirliği aracıdır. Tüm iOS, Android ve Windows 10 cihazlarınızdaki iş dosyalarınızı, yönetimi kolay kurumsal düzeyde bir güvenlikle koruyabilirsiniz.
  
Microsoft 365 İş 300 lisansa kadar yöneliktir, daha fazla lisansa ihtiyacınız varsa daha fazla bilgi için [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) belgelerine göz atın. 
  
## <a name="get-microsoft-365-business"></a>Microsoft 365 İş'i alma

- İş ortağınız varsa, onlar da Microsoft 365 İş ürününü alır: [Microsoft 365 İş'i Microsoft İş Ortağı Merkezi'nden alma](get-microsoft-365-business.md).
    
- İş ortağınız yoksa ve Microsoft 365 İş'i edinmek istiyorsanız, [buradan satın alabilirsiniz](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Microsoft 365 İş'i ayarlama

 **Microsoft 365 Business Suite ayarlanan genel bakış**
  
Aşağıdaki diyagramda Microsoft 365 iş yöneticileri nasıl ayarlanacağını açıklar. Ayrıca 365 işletmeler için Microsoft Windows PC'ler hazırlamak için gereken adımları açıklar. Yeni aygıtlar için Microsoft 365 iş Yönetim Merkezi'nde [Windows AutoPilot](add-autopilot-devices-and-profile.md)ile de ekleyebilirsiniz. AutoPilot ayarlamak ve yeni aygıtlar kendi Microsoft 365 iş kimlik bilgileriyle kullanıcı imzalar hemen sonra bunları üretken kullanılmaya hazır alma önceden yapılandırmak için kullanabilirsiniz.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 iş (Admin) ayarlamanız

Genel yönetici kimlik bilgilerinizle [Microsoft 365 İş yönetim merkezinde](https://portal.office.com/adminportal/home) oturum açın ve Microsoft 365 İş'ı ayarlamak için aşağıdaki adımları tamamlayın. 
  
1. [Cihazlardaki verileri Microsoft 365 İş ile korumanın önkoşulları](pre-requisites-for-data-protection.md)
    
    Önkoşulları okuyun ve cihazınızın Microsoft 365 İş için hazır olduğundan emin olun.
    
2. [Microsoft 365 İş'i kurulum sihirbazını kullanarak ayarlama](set-up.md)
    
    **Bulut için bir yerel Active Directory'den kalıcı olarak taşıma**iseniz, ya da kullanıcıların el ile Microsoft 365 iş Yönetim Merkezi'nde Kurulum Sihirbazı'nı kullanarak ekleyebilirsiniz veya Azure AD Connect ile bir kerelik eşitleme yapabilirsiniz. Bunu yapmanın iki yolu vardır: 
    
  - Ayrıca bir Exchange 2010, Exchange 2013 veya 2016 Exchange sunucusu varsa, [Hızlı bir şekilde Office 365 Exchange posta kutularına geçirmek için en az karma](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)olabilir. En az karma adımları Azure Reklam kullanıcılara tek seferlik bir eşitleme dahil yanı sıra yerinde geçiş bulut için e-posta. E-posta geçişi tamamlandıktan sonra dizin eşitleme otomatik olarak bu yöntemi kullanırken kapalı.
    
  - Kullanıcılarınızı buluta eşitlemek için Office 365 dizin eşitleme sihirbazını kullanın. Bu işlemi tamamlamak üzere [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) bölümündeki adımları izleyin. Kullanıcılarınızı buluta eşitledikten sonra [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Bu şekilde bir lisans Microsoft 365 iş için eklenen her kullanıcıya vermek gerekecektir. [Kurulum Sihirbazı](set-up.md)' nı veya [iş için Office 365'te kullanıcılara lisans atama](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)bunu yapabilirsiniz.
    
### <a name="2-prepare-mobile-devices"></a>2: mobil cihazlar hazırla

[Mobil aygıtlar Microsoft 365 iş kullanıcıları için ayarlama](set-up-mobile-devices.md) aygıtları ve Microsoft 365 işletme tarafından korunan emin olarak Office uygulamaları yüklemek için adımları izleyin. 
  
### <a name="3-prepare-pcs"></a>3: bilgisayarları hazırlama

Yöneticiler yeni aygıtların Windows 10 PC'ler ayarlarını [Windows AutoPilot](add-autopilot-devices-and-profile.md)kullanarak önceden seçebilirsiniz. Kullanıcılar, varolan veya yeni Windows 10 aygıtları bu konudaki adımları izleyerek ayarlayabilirsiniz: [Microsoft 365 iş kullanıcıları için Windows PC'ler ayarlayın](set-up-windows-devices.md). Varolan aygıtlar için **isteğe bağlı olarak**[İş OneDrive için dosyaları taşıyın](move-files-to-onedrive.md)kullanıcıları da yapabilirsiniz. Bunlar da OneDrive için Windows profili ile ilişkili dosyaları taşımak için üçüncü taraf araçları kullanabilirsiniz.
  
Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz. Bunu ayarlamak için [Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış Windows 10 aygıtları etkinleştirme](manage-windows-devices.md) adımlarını izleyin. Tercih edilen yöntem budur ve bu durumda aygıtları **karma Azure AD alanına bağlı aygıtlar**denir. 
  
Yerel korumak bazı içeren Active Directory yerinde kaynaklar (örneğin, dosya paylaşımları ve yazıcılar), bu kaynakların **Azure AD alanına bağlı aygıtlara** erişiminizi burada adımları izleyerek verebilirsiniz: [erişim şirket içi kaynaklardan bir 365 işletmede Azure AD alanına bağlı aygıt](access-resources.md).
  
Windows 10 PC'ler ayarladıktan sonra aygıtlara [otomatik olarak Office yükleme](auto-install-or-uninstall-office.md) yapabilirsiniz. 
  
## <a name="contact-support"></a>Desteğe başvurun

 **Desteğe başvurmanız gerekiyorsa:**
  
- İş ortağınızla iletişime geçin.
    
- Microsoft 365 iş yönetici, müşteri destek ekibimiz, ** [iş ürünleri - yönetici Yardım için desteğe başvurun](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) erişebilirsiniz**
    

