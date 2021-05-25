---
title: E3'Microsoft 365 İş E3'Office 365 geçirme
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
description: Office 365 E3 aboneliğiniz varsa ancak 300'den fazla çalışan yoksa, Microsoft 365 İş Ekstra.
ms.openlocfilehash: d139d07c946ff3efed3db3a73eb5e1a4ae66c190
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52623615"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>E3'Office 365 başka bir e-postaya Microsoft 365 İş Ekstra

Microsoft 365 İş Ekstra, sınıf için en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek küçük işletmeniz için gereken her şeye sahip olur. Şu anda bir Office 365 E3 aboneliğiniz varsa ancak 300'den fazla çalışan yoksa, ek güvenlik özellikleri için Microsoft 365 İş Ekstra'e geçmeyi göz önünde bulundurabilirsiniz.

Geçiş yapmak kolaydır: Önce lisansları değiştirersiniz ve geçerli aboneliğinizin tüm verileriyle kullanıcı bilgileri korunur. Geçiş sonrasında, Özellikler'e eklenen özellikleri Microsoft 365 İş Ekstra.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>E3 ile Office 365 arasındaki farklar Microsoft 365 İş Ekstra

Bu tabloda, E3'Microsoft 365 İş Ekstra iki Office 365 gösterir.

| Özellik    | Destek Microsoft 365 İş Ekstra    | Office 365 E3'te destek |
|:-------|:-----|:-----|
| **Şirket içi**        | | |
| Office uygulamaları<sup>1</sup>    | İş için Microsoft 365 Uygulamaları    | Microsoft 365 Kurumsal Uygulamaları |
| **Bulut üretkenlik uygulamaları**        | | |
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız depolama Exchange Online Arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız depolama Exchange Online Arşivleme |
| Teams    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız | 
| Yammer, SharePoint Online, Planner, Stream    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) | 
| StaffHub    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) |
| **Tehdit Koruması**        | | |
| Office 365 için Defender Plan 1 | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | Dahil değildir, ancak |
| **Kimlik yönetimi**        | | |
| Karma kimlik bilgileri (Azure AD) Azure Active Directory, Azure AD multi-factor authentication (MFA), Koşullu Erişim için self servis parola sıfırlama, şirket içi kimlikler için parola geri yazma|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    |  |
| **Cihaz ve uygulama yönetimi**        | | |
| Microsoft Intune AutoPilot Windows a|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    |  |
| Paylaşılan bilgisayar etkinleştirmesi|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png)| 
| Win 7/8.1 Windows 10 Pro lisanslarından yükseltme Pro hakları|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    ||
| **Bilgi koruması**        | | |
|Office 365 Veri Kaybını Önleme|    ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)|![Office 365 E3'e dahil](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker zorlaması|![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)||
|Azure Information Protection Plan 1, Duyarlılık etiketleri|![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)||
|**İstemci Erişimi Lisansı (CAL hakları)**|||
|Enterprise CAL Paketi (Exchange, SharePoint, Skype)||![Office 365 E3'e dahil](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 İş Ekstra uygulamalarının en iyi sürümü Office Grup İlkesi, uygulama telemetrisi, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya İş Zekası aracılığıyla toplu etkinleştirmeyi içermemektedir.

## <a name="migration"></a>Geçiş

Aboneliğinizi geçirmek için, [yalnızca birkaç kişiyi](../commerce/subscriptions/change-plans-manually.md) taşımak istediğiniz yönergeler için bkz. El ile Microsoft 365 İş Ekstra. Ayrıca, E3 [aboneliğinizi ve](../commerce/subscriptions/upgrade-to-different-plan.md)lisanslarınızı yeni bir aboneliğe taşımak için herkesi otomatik olarak yükseltebilirsiniz veya bir Microsoft 365 İş Ekstra çalışabilirsiniz.
Aşağıdaki bölümlerde, varsa yapmak için ihtiyacınız olan değişiklikler ve geçiş sonrasında neler yapabilirsiniz açıklanmaktadır.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 abonelik yapılandırması ve verileri
Şu gibi değişikliklerden önce geçerli aboneliğiniz veya verilerinizde değişiklik yapmak zorunda değilsiniz:

- Dns kayıtları ve etki alanı adları gibi abonelik yapılandırması.
- Çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ile kimlik doğrulama ayarları.
- Üretkenlik hizmeti yapılandırmaları ve Teams, Exchange Online kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve not defterleri gibi verileri OneNote.
- Office uygulamalar otomatik olarak ölçeklendirilir. Office 365 lisanslama, kullanıcının lisans atamasını her 72 saatte bir kontrol edin ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.

### <a name="windows-10"></a>Windows 10

Windows Creator güncelleştirmesi'Windows Pro bunları Windows Pro [Creators Update sürümüne yükseltin.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Kullanıcı cihazlarını ve dosyalarını korumak için ilkeler ayarlama

> [!NOTE]
> Farklı MDM Office 365 cihazları ayarladısanız, bu cihazlar Yönetim Merkezi'nin **Cihazlar** Microsoft 365 listelenir. Ayar her ilke [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.

Microsoft 365 İş Ekstra'a lisans atadikten sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.

Microsoft 365 İş Ekstra'a tüm kuruluş yükseltmelerini yaptıysanız, Giriş sayfasında kurulum sihirbazını görebilirsiniz ve dosyaları ve mobil cihazları korumak için kurulum sihirbazının adımlarında [Microsoft 365 İş Ekstra'i](set-up.md) ayarlama adımlarını izleyin.

Şu adımları Cihazlar sayfasında da tamamabilirsiniz:
  
1. Yönetim merkezinde, sol gezintide Cihaz **İlkeleri'ne** \> **gidin.**

2. Cihaz ilkeleri **sayfasında Ekle'yi** **seçin.**

3. İlke **ekle bölmesinde** ilkeye bir ad verin ve sonra açılan açılan seçim **listesinden** İlke türü seçin.

     Android ve iPhone cihazlarında dosyaların korunması için uygulama ilkelerinin yanı sıra Windows 10 ve şirkete ait farklı cihazlarda cihaz yapılandırma Windows 10 kurabilirsiniz. Ayrıntılar için aşağıdaki bağlantılara bakın:

  - [Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme](app-protection-settings-for-android-and-ios.md)

  - [Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme](protection-settings-for-windows-10-devices.md)

  - [Bilgisayarlarda cihaz koruma Windows 10 ayarlama](protection-settings-for-windows-10-pcs.md)
  
4. İlkeleri ayar defa siz ve çalışanlarınız cihazları kurabilirsiniz:

  - Mobil [cihazlara Windows için Microsoft 365 İş Ekstra için](set-up-windows-devices.md) cihaz ayarlama Windows bakın. 

  - Android telefonlar ve iPhone [Microsoft 365 İş Ekstra için](set-up-mobile-devices.md) mobil cihazları mobil cihazlara ayarlama. 
  
### <a name="mailbox-size"></a>Posta Kutusu Boyutu

Microsoft 365 İş Ekstra Plan 1'i kullandığı için 50 GB Exchange Online sınırlaması vardır. Microsoft 365 İş Ekstra'a geçirken, kullanıcılardan herhangi biri 50 GB'lık posta kutusu depolama alanını aşıyorsa, bu kullanıcıya Exchange Online Plan 2 atamanız ve her ikisini de atamak uygun bir uygulama olduğu için Exchange Online Plan 1'i kaldırmanız önerilir.

### <a name="threat-protection"></a>Tehdit koruması

Microsoft 365 İş Ekstra'a Office 365 için Defender'ınız Office 365. Genel [bir bakış için Office 365](../security/office-365-security/defender-for-office-365.md) için Microsoft Defender'a bakın. Ayarlamak için bkz. Bağlantı [Kasa](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)ayarlama [,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)Kasa Ekleri ayarlama ve Güvenlik için Defender'da Kimlik avı [koruması'Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Duyarlılık etiketleri

Duyarlılık etiketlerini kullanmaya başlamak için bkz. [Duyarlılık etiketlerine genel bakış](../compliance/sensitivity-labels.md) ve duyarlılık etiketleri videosu oluşturma ve [yönetme.](../business-video/create-sensitivity-labels.md)

## <a name="related-content"></a>İlgili içerik

[Planları el ile değiştirme](../commerce/subscriptions/change-plans-manually.md) (makale)\
[Cihazları Windows (video)\ Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) yükseltme
[Android veya iOS cihazlarına yönelik uygulama koruma ayarlarını ayarlama](app-protection-settings-for-android-and-ios.md) (makale)\
[Cihazlar için uygulama koruma ayarlarını Windows 10 düzenleme](protection-settings-for-windows-10-devices.md) (makale)\
[]

