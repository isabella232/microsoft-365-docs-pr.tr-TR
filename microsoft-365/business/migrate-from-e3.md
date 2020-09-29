---
title: Office 365 E3 'den Microsoft 365 Business 'a geçme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: İşinizi Office 365 E3 'den Microsoft 365 Business Premium 'a taşımayı öğrenin.
ms.openlocfilehash: f3f3894a2a5cb69f9f91825d89db4f4b857fac5c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295300"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Office 365 E3 'den Microsoft 365 Business Premium 'a geçme 

Microsoft 365 Iş ekstra, basit cihaz yönetimi ve güvenliğiyle en iyi sınıf bulut tabanlı verimlilik uygulamalarını birleştiren küçük işletmeniz için gereken her şeyi içerir. Şu anda bir Office 365 E3 aboneliğiniz varsa, ancak 300 ' den fazla çalışanı yoksa, ek güvenlik özellikleri için Microsoft 365 Iş Premium 'a geçmeyi düşünebilirsiniz.

Geçiş kolay: Ilk olarak lisansları değiştirdiğinizde geçerli aboneliğinizde tüm verileriniz ve Kullanıcı bilgileriniz korunur. Geçişten sonra, Microsoft 365 Business Premium 'A eklenen özellikleri ayarlamanız gerekir.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3 ve Microsoft 365 Iş ekstra arasındaki farklar

Bu tabloda, Microsoft 365 Business Premium ve Office 365 E3 arasındaki farklılıklar gösterilmektedir.

| Özellik    | Microsoft 365 Business Premium 'da destek    | Office 365 E3 | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Office uygulamaları<sup>1</sup>    | İş için Microsoft 365 uygulamaları    | Kurumlar için Microsoft 365 Uygulamaları | 
| **Bulut üretkenlik uygulamaları**        | | | 
| Exchange Online ve Outlook    | posta kutusu başına 50 GB depolama alanı ve sınırsız Exchange Online arşivleme    | posta kutusu başına 100 GB depolama alanı ve sınırsız Exchange Online arşivleme | 
| Teams    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Süresiz | 
| Yammer, SharePoint Online, Planner, akış    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| StaffHub    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | | 
| **Tehdit koruması**        | | | 
| Office 365 Gelişmiş tehdit koruması (ATP) plan 1 | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | Dahil değildir, ancak eklenebilir | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Active Directory (Azure AD) hesapları, Azure Multi-Factor Authentication (MFA) için self servis parola sıfırlama, koşullu erişim, şirket içi kimlikler için parola geri yazma|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    |  | 
| **Cihaz ve uygulama yönetimi**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    |  |
| Paylaşılan bilgisayar etkinleştirmesi|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| Win 7/8.1 Pro lisanlarından Windows 10 Pro 'ya yükseltme hakları|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    || 
| **Bilgi koruması**        | | |
|Office 365 veri kaybı önleme|    ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|Azure bilgi koruma planı 1, BitLocker zorlaması|![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)||
|Azure bilgi koruma planı 1, duyarlılık etiketleri|![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)||
|**İstemci erişim lisansı (CAL hakları)**|||
|Kurumsal CAL Paketi (Exchange, SharePoint, Skype)||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<sup>1</sup> Office uygulamalarının Microsoft 365 Business Premium sürümü Grup ilkesi, uygulama telemetri, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya iş zekası aracılığıyla toplu etkinleştirme içermez.

## <a name="migration"></a>Geçişte

Aboneliğinizi geçirmek için, yalnızca birkaç kişiyi Microsoft 365 Business Premium 'a taşımak isterseniz yönergeleri [El Ile değiştirme](../commerce/subscriptions/change-plans-manually.md) konusuna bakın. Ayrıca, E3 aboneliğinizi ve lisanslarınızı bir Microsoft 365 Iş Ekstra aboneliğine taşımak için [herkesi otomatik olarak yükseltebilir](../commerce/subscriptions/upgrade-to-different-plan.md)veya bir iş ortağıyla çalışabilirsiniz.
Aşağıdaki bölümlerde, eğer varsa ve geçiş sonrasında yapabileceğiniz değişiklikler açıklanmaktadır.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 abonelik yapılandırması ve verileri
Geçirmeden önce geçerli aboneliğinizde veya verilerinizde değişiklik yapmanız gerekmez, aşağıdakileri içerir:

- DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.
- Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.
- Üretkenlik hizmeti yapılandırmaları ve takımlar, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive Iş klasörleri ve OneNote Not defterleri gibi verileri.
- Office uygulamaları otomatik olarak ölçeklenir. Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte denetler ve Office uygulamalarını Kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.

### <a name="windows-10"></a>Windows 10

Windows 'da Windows Pro Creator güncelleştirmesi yoksa, [bunları Windows Pro Creators Update 'e yükseltebilirsiniz](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Kullanıcı aygıtlarını ve dosyalarını koruyacak ilkeler ayarlama

> [!NOTE]
> Office 365 MDM ilkeleri ve aygıtları ayarlıyorsanız, bu cihazlar Microsoft 365 yönetim merkezindeki **cihazlar** sayfasında listelenir. Ayarladığınız tüm ilkeler [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.

Microsoft 365 Business Premium 'a lisans atadıktan sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.

Kuruluşunuzdaki herkesi Microsoft 365 Business Premium 'a yükselttiyseniz, giriş sayfasında Kurulum Sihirbazı 'nı görürsünüz ve dosyaları ve mobil cihazları koruyan [Kurulum sihirbazındaki Microsoft 365 Business Premium](set-up.md) kurulumunu izleyebilir.

Bu adımları aygıtlar sayfasında da tamamlayabilirsiniz:
  
1. Yönetim merkezinde, sol gezintide, **cihazlar** \> **ilkeleri**'ne gidin.
    
2. **Cihaz ilkeleri** sayfasında **Ekle**'yi seçin.
    
3. **Ilke Ekle** bölmesinde ilkeye bir ad verin ve açılan listeden bir **ilke türü** seçin. 
    
     Windows 10 ' da Android ve iPhone cihazlarında dosyaları korumak için uygulama ilkelerini ayarlayabilir ve şirkete ait Windows 10 cihazlarında aygıt yapılandırma ilkelerini ayarlayabilirsiniz. Ayrıntılar için aşağıdaki bağlantılara bakın:
    
  - [Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme](app-protection-settings-for-android-and-ios.md)
    
  - [Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme](protection-settings-for-windows-10-devices.md)
    
  - [Windows 10 bilgisayarlarında cihaz koruma ayarlarını ayarlama](protection-settings-for-windows-10-pcs.md)
  
4. İlkeleri ayarladıktan sonra, siz ve çalışanlarınız cihazları ayarlayabilirsiniz:
    
  - Windows aygıtlarının adımları için [Microsoft 365 Business Premium kullanıcıları Için Windows cihazlarını ayarlama](set-up-windows-devices.md) bölümüne bakın. 
    
  - Android telefonlar ve IPhone adımları için [Microsoft 365 Business Premium kullanıcıları için mobil cihazları ayarlayın](set-up-mobile-devices.md) bölümüne bakın. 
  
### <a name="mailbox-size"></a>Posta kutusu boyutu

Microsoft 365 Business Premium, Exchange Online Plan 1 kullandığı için 50 GB depolama sınırlamasına sahiptir. Microsoft 365 Business Premium 'a geçiş yaparken, kullanıcılarınız 50 GB 'lik posta kutusu deposunu aşıyorsa, bu kullanıcıyı bir Exchange Online Plan 2 ' ye atamanız ve her ikisini de atamak uygun olmadığı için Exchange Online Plan 1 ' i kaldırmanız önerilir.


### <a name="threat-protection"></a>Tehdit koruması

Microsoft 365 Business Premium 'a geçtikten sonra, Office 365 ATP 'niz vardır. Genel bakış için [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) 'ye bakın. Ayarlamak için, [ATP güvenli bağlantılarını ayarlayın](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [ATP güvenli EKLERINI ayarlayın](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ve [ATP önleme önleyici bir şekilde ayarlayın](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Duyarlılık etiketleri

Duyarlılık etiketlerini kullanmaya başlamak için, [duyarlılık etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ve [duyarlılık etiketleri oluşturma ve yönetme](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)
