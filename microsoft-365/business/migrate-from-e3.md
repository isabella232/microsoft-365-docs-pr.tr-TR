---
title: Office 365 E3'den Microsoft 365 İş'e geçiş
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
description: İşletmenizi Office 365 E3'te Microsoft 365 İş Ekstra'ya taşımayı öğrenin.
ms.openlocfilehash: cb70260201686cae02428c715ac98ffe2f88787f
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198107"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Office 365 E3'den Microsoft 365 İş Ekstra'ya

Microsoft 365 İş Ekstra, sınıfı en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahip. Şu anda bir Office 365 E3 aboneliğiniz varsa ancak 300'den fazla çalışan yoksa, ek güvenlik özellikleri için Microsoft 365 İş Ekstra'ya geçmeyi göz önünde bulundurabilirsiniz.

Geçiş kolaydır: İlk olarak lisansları değiştirebilirsiniz ve geçerli aboneliğinizin tüm verileri ve kullanıcı bilgileri korunur. Geçiş sonrasında, Microsoft 365 İş Ekstra'ya eklenen özellikleri ayarlamalısiniz.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Office 365 E3 ile Microsoft 365 İş Ekstra arasındaki farklar

Bu tablo, Microsoft 365 İş Ekstra ile Office 365 E3 arasındaki farkları gösterir.

| Özellik    | Microsoft 365 İş Ekstra desteği    | Office 365 E3'te destek | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Office uygulamaları<sup>1</sup>    | İş için Microsoft 365 Uygulamaları    | Microsoft 365 Kurumsal Uygulamaları | 
| **Bulut üretkenlik uygulamaları**        | | | 
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online Arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online Arşivleme | 
| Teams    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız | 
| Yammer, SharePoint Online, Planner, Stream    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| StaffHub    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| Outlook Customer Manager    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | | 
| **Tehdit Koruması**        | | | 
| Office 365 için Defender Plan 1 | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | Dahil değildir, ancak | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Active Directory (Azure AD) hesapları için self servis parola sıfırlama, Azure AD çok faktörlü kimlik doğrulaması (MFA), Koşullu Erişim, şirket içi kimlikler için parola geri yazma|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    |  | 
| **Cihaz ve uygulama yönetimi**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    |  |
| Paylaşılan bilgisayar etkinleştirmesi|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| Win 7/8.1 Pro lisanslarından Windows 10 Pro'ya yükseltme hakları|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    || 
| **Bilgi koruması**        | | |
|Office 365 Veri Kaybını Önleme|    ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker zorlaması|![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)||
|Azure Information Protection Plan 1, Duyarlılık etiketleri|![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)||
|**İstemci Erişim Lisansı (CAL hakları)**|||
|Kurumsal CAL Paketi (Exchange, SharePoint, Skype)||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<sup>1</sup> Office uygulamalarının Microsoft 365 İş Ekstra sürümü Grup İlkesi, uygulama telemetrisi, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya İş Zekası aracılığıyla toplu etkinleştirmeyi içermemektedir.

## <a name="migration"></a>Geçiş

Aboneliğinizi geçirmek için, yalnızca birkaç kişiyi Microsoft 365 İş Ekstra'ya taşımak istediğiniz yönergeleri el ile değiştirme yönergelerine bakın. [](../commerce/subscriptions/change-plans-manually.md) Ayrıca, E3 [aboneliğinizi](../commerce/subscriptions/upgrade-to-different-plan.md)ve lisanslarınızı Microsoft 365 İş Ekstra aboneliğine taşımak için herkesi otomatik olarak yükseltebilirsiniz veya bir iş ortağıyla çalışabilirsiniz.
Aşağıdaki bölümlerde, varsa, yapmak için gereken değişiklikler ve geçiş sonrasında neler yapabilirsiniz açıklanmaktadır.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 abonelik yapılandırması ve verileri
Geçerli aboneliğiniz veya verilerinizde, şu değişikliklerden önce değişiklik yapmak zorunda değildir:

- DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.
- Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.
- Teams, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve bunların verileri.
- Office uygulamaları otomatik olarak ölçeklendirilir. Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte bir kontrol edin ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.

### <a name="windows-10"></a>Windows 10

Windows'uz henüz Windows Pro Creator güncelleştirmesi üzerinde değilse, bunları [Windows Pro Creators Update'e yükseltin.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Kullanıcı cihazlarını ve dosyalarını korumak için ilkeler ayarlama

> [!NOTE]
> Office 365 MDM ilkelerini ve cihazlarını kursanız, bu  cihazlar Microsoft 365 yönetim merkezinin Cihazlar sayfasında listelenir. Ayar her ilke [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.

Lisansları Microsoft 365 İş Ekstra'ya atadikten sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.

Kuruluşta yer alan herkesi Microsoft 365 İş Ekstra'ya yükselttiyebilirsiniz. Kurulum sihirbazını Giriş sayfasında görebilirsiniz ve dosyaları ve mobil cihazları korumak için kurulum sihirbazı adımlarında [Microsoft 365 İş Ekstra'nın](set-up.md) kurulumu adımlarını takip edebilirsiniz.

Bu adımları Cihazlar sayfasında da tamamabilirsiniz:
  
1. Yönetim merkezinde, sol gezintide Cihazlar **İlkeleri'ne** \> **gidin.**
    
2. Cihaz ilkeleri **sayfasında Ekle'yi** **seçin.**
    
3. İlke **ekle bölmesinde** ilkeye bir ad verin ve ardından açılan **listelerden bir** İlke türü seçin. 
    
     Android ve iPhone cihazlarının yanı sıra Windows 10'da da dosyaları korumak için uygulama ilkeleri ayarlarken, şirkete ait Windows 10 cihazları için cihaz yapılandırma ilkelerini de kurabilirsiniz. Ayrıntılar için aşağıdaki bağlantılara bakın:
    
  - [Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme](app-protection-settings-for-android-and-ios.md)
    
  - [Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme](protection-settings-for-windows-10-devices.md)
    
  - [Windows 10 bilgisayarlar için cihaz koruma ayarlarını ayarlama](protection-settings-for-windows-10-pcs.md)
  
4. İlkeleri ayar defa siz ve çalışanlarınız cihazları kurabilirsiniz:
    
  - Windows [cihazları için adımlar için Bkz. Microsoft 365 İş Ekstra](set-up-windows-devices.md) kullanıcıları için Windows cihazlarını ayarlama. 
    
  - Android telefonlar ve iPhone'lar için adımlar için [Bkz. Microsoft 365](set-up-mobile-devices.md) İş Ekstra kullanıcıları için mobil cihazları ayarlama. 
  
### <a name="mailbox-size"></a>Posta Kutusu Boyutu

Exchange Online Plan 1'i kullandığı için Microsoft 365 İş Ekstra'nın 50 GB depolama sınırı vardır. Microsoft 365 İş Ekstra'ya geçen kullanıcılardan herhangi biri 50 GB'lık posta kutusu depolama alanını aşarsa, bu kullanıcıya Exchange Online Plan 2 atamanız ve Exchange Online Plan 1'i kaldırmanız önerilir çünkü her ikisini de atamak uygun değildir.


### <a name="threat-protection"></a>Tehdit koruması

Microsoft 365 İş Ekstra'ya katıldıktan sonra Office 365 için Defender'a sahipsiniz. Genel [bakış için Office 365 için Microsoft Defender'a](../security/office-365-security/defender-for-office-365.md) bakın. Ayarlamak için Güvenli [Bağlantılar'ı](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [ayarlama,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)Güvenli Ekleri ayarlama ve [Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)için Defender'da Kimlik avı önlemeyi ayarlama.

### <a name="sensitivity-labels"></a>Duyarlılık etiketleri

Duyarlılık etiketlerini kullanmaya başlamak için, duyarlılık etiketlerine [genel bakış](../compliance/sensitivity-labels.md) videosunu izleyin ve duyarlılık etiketleri videosu oluşturun [ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)
