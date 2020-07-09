---
title: Office 365 E3'ten Microsoft 365 Business'a geçiş
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
description: İşinizi Office 365 E3'ten Microsoft 365 Business Premium'a nasıl taşıyabildiğiniöğrenin.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081924"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Office 365 E3'ten Microsoft 365 Business Premium'a geçiş 

Microsoft 365 Business Premium, sınıfının en iyisi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahiptir. Şu anda bir Office 365 E3 aboneliğiniz varsa, ancak 300'den fazla çalışanın yoksa, ek güvenlik özellikleri için Microsoft 365 Business Premium'a geçmeyi düşünün.

Geçiş kolaydır: Önce lisansları değiştirirsiniz ve geçerli aboneliğinizdeki tüm verileriniz ve kullanıcı bilgileriniz korunur. Geçişten sonra Microsoft 365 Business Premium'a eklenen özellikleri ayarlamanız gerekir.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3 ile Microsoft 365 Business Premium arasındaki farklar

Bu tablo, Microsoft 365 Business Premium ve Office 365 E3 arasındaki farkları gösterir.

| Özellik    | Microsoft 365 Business Premium desteği    | Office 365 E3'te destek | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Office uygulamaları<sup>1</sup>    | Microsoft 365 İş uygulamaları    | Kurumsal uygulamalar için Microsoft 365 | 
| **Bulut üretkenliği uygulamaları**        | | | 
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online Arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online Arşivleme | 
| Takım    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız | 
| Yammer, SharePoint Online, Planlayıcı, Akış    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| PersonelHub    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| Outlook Müşteri Yöneticisi, MileIQ    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | | 
| **Tehdit Koruması**        | | | 
| Office 365 Gelişmiş Tehdit Koruması (ATP) Planı 1 | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | Dahil değil, ancak eklenebilir | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Etkin Dizin (Azure AD) hesapları, Azure çok faktörlü kimlik doğrulama (MFA), Koşullu Erişim, şirket içi kimlikler için parola yazma için self servis parola sıfırlama|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    |  | 
| **Cihaz ve uygulama yönetimi**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    |  |
| Paylaşılan bilgisayar etkinleştirme|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| Win 7/8.1 Pro lisanslarından Windows 10 Pro'nun yükseltme hakları|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    || 
| **Bilgi koruması**        | | |
|Office 365 Veri Kaybı Önleme|    ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|Azure Bilgi Koruma Planı 1, Bitlocker uygulaması|![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)||
|Azure Bilgi Koruma Planı 1, Duyarlılık etiketleri|![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)||
|**İstemci Erişim Lisansı (CAL hakları)**|||
|Kurumsal CAL Paketi (Exchange, SharePoint, Skype)||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<sup>1</sup> Office uygulamalarının Microsoft 365 Business Premium sürümü, Grup İlkesi, uygulama telemetrisi, denetimleri güncelleştirme, elektronik tablo karşılaştırma ve sorgulama veya iş Zekası yoluyla toplu etkinleştirme içermez.

## <a name="migration"></a>Geçiş

Aboneliğinizi geçirmek için, birkaç kişiyi Microsoft 365 Business Premium'a taşımak istiyorsanız, talimatları [el ile değiştir planlarına](../commerce/subscriptions/change-plans-manually.md) bakın. E3 aboneliğinizi ve lisanslarınızı Microsoft 365 Business Premium aboneliğine taşımak için [herkesi otomatik olarak yükseltebilir](../commerce/subscriptions/upgrade-to-different-plan.md)veya bir iş ortağıyla birlikte çalışabilirsiniz.
Aşağıdaki bölümlerde, varsa yapmanız gereken değişiklikleri ve geçişten sonra neler yapabileceğiniz açıklanabilir.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 abonelik yapılandırması ve verileri
Geçiş yapmadan önce geçerli aboneliğinizde veya verilerinizde herhangi bir değişiklik yapmanız gerekmez:

- DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.
- Çok faktörlü kimlik doğrulama veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ve kimlik doğrulama ayarları.
- Ekipler, Exchange Online posta kutuları, SharePoint Online siteleri, İş için OneDrive klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve verileri.
- Office uygulamaları otomatik olarak ölçeklendirilir. Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte bir denetler ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.

### <a name="windows-10"></a>Windows 10

Windows'unuz Windows Pro Creator güncelleştirmesi kullanmıyorsa, [bunları Windows Pro Creators Update'e yükseltin.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Kullanıcı aygıtlarını ve dosyalarını korumak için ilkeler ayarlama

> [!NOTE]
> Office 365 MDM ilkeleri ve aygıtları ayarlarsanız, bu aygıtlar Microsoft 365 yönetici merkezindeki **Cihazlar** sayfasında listelenir. Ayarladığınız tüm [ilkeler, Intune portalındaki](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde gösterecektir.

Microsoft 365 Business Premium'a lisans lar atadıktan sonra, kullanıcıların aygıtlarını ve dosyalarını korumaya başlayabilirsiniz.

Kuruluşunuzdaki herkesi Microsoft 365 Business Premium'a yükselttiyseniz, Ana Sayfada kurulum sihirbazını görürsünüz ve dosyaları ve mobil aygıtları korumak için [kurulum sihirbazı adımlarında Microsoft 365 Business Premium'u](set-up.md) ayarlayabilirsiniz.

Ayrıca Cihazlar sayfasında aşağıdaki adımları tamamlayabilirsiniz:
  
1. Yönetici merkezinde, sol navigasyonda Aygıt **Devices** \> **İlkeleri'ne**gidin.
    
2. Aygıt **ilkeleri** sayfasında **Ekle'yi**seçin.
    
3. **İlke Ekle** bölmesinde ilke bir ad verin ve ardından açılan dan bir **İlke türü** seçin. 
    
     Android ve iPhone aygıtlarının yanı sıra Windows 10'daki dosyaları korumak için uygulama ilkeleri ayarlayabilir ve şirkete ait Windows 10 aygıtları için aygıt yapılandırma ilkeleri ayarlayabilirsiniz. Ayrıntılar için aşağıdaki bağlantılara bakın:
    
  - [Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme](app-protection-settings-for-android-and-ios.md)
    
  - [Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme](protection-settings-for-windows-10-devices.md)
    
  - [Windows 10 bilgisayarların aygıt koruma ayarlarını ayarlama](protection-settings-for-windows-10-pcs.md)
  
4. İlkeleri ayarladıktan sonra, siz ve çalışanlarınız aygıtlar ayarlayabilirsiniz:
    
  - Bkz. Windows aygıtları için adımlar [için Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlayın.](set-up-windows-devices.md) 
    
  - Bkz. Android telefonlar ve iPhone'lar için adımlar için [Microsoft 365 Business Premium kullanıcıları için mobil cihazlar ayarlama.](set-up-mobile-devices.md) 

### <a name="threat-protection"></a>Tehdit koruması

Microsoft 365 Business Premium'a geçtikten sonra Office 365 ATP'niz var. Genel bakış için [Office 365 ATP'ye](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) bakın. Kurmak için, [ATP güvenli bağlantılar kurmak,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [ATP güvenli ekleri kurmak](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ve [ATP anti-phishing kurmak](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)bakın.

### <a name="sensitivity-labels"></a>Duyarlılık etiketleri

Duyarlılık etiketleri kullanmaya başlamak için duyarlılık [etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) bölümüne bakın ve duyarlılık etiketleri videosu [oluşturun ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)
