---
title: Microsoft 365 İş'den Microsoft 365 E3'e geçiş
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: İşletmenizi Microsoft 365 İş Ekstra'dan Microsoft 365 E3'e taşımayı öğrenin.
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164523"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Microsoft 365 İş Ekstra'dan Microsoft 365 E3'e geçiş

Microsoft 365 İş Ekstra, sınıfı en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek çalışanlarınızı en iyi şekilde çalışmalarına olanak sağlayan küçük işletmeniz için ihtiyacınız olan her şeye sahip. Bununla birlikte, bazı durumlarda Microsoft 365 İş Ekstra aboneliğinizi Microsoft 365 E3'e geçirmeniz gerekir. 

Örneğin, işletmeniz büyüdü ve 300'den fazla lisansa ihtiyacı var (bu arada tebrikler).

Ya da işletmenize kuruluş için Microsoft 365 Uygulamaları, Windows 10 Kurumsal E3 veya Kurumsal İstemci Erişimi Lisansları (CA'lar) gibi kurumsal özellikler gerekir.

Kolayca yükseltebilirsiniz: Yükseltmeyi Yönetim [merkezinden başlatabilirsiniz.](../commerce/subscriptions/upgrade-to-different-plan.md) Geçerli aboneliğinizin tüm verileri ve yapılandırması korunur. Geçişe hazırlanmak için yapacak hiçbir şey yoktur ve sonrasında yeni özelliklerden yararlanmak dışında hiçbir şey olmaz.

>[!Note]
>Ayrıca, en fazla 300 kişi için Microsoft 365 İş Ekstra aboneliği kullanabilir ve 300'den fazla koltuk için Microsoft 365 E3 aboneliği edinebilirsiniz. Ancak Office 365 için Microsoft Defender, Microsoft 365 E3'e dahil değildir. Tehdit korumasının devamını almak için, Office 365 için Defender lisansları eklemeniz gerekir; böylelikle Office 365 için Defender'nız kapsamındaki tüm kullanıcıların lisansı olur.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Microsoft 365 İş Ekstra ile Microsoft 365 Kurumsal arasındaki farklar

Bu tablo, Microsoft 365 İş Ekstra ile Microsoft 365 E3 arasındaki farkları gösterir.

| Özellik    | Microsoft 365 İş Ekstra desteği    | Microsoft 365 E3'te destek | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Office uygulamaları*    | [İş için Microsoft 365 Uygulamaları](#office-365-business)    | Microsoft 365 Kurumsal Uygulamaları | 
| **Bulut üretkenlik uygulamaları**        | | | 
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online arşivleme | 
| Teams    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız | 
| Yammer, SharePoint Online, Planner, Stream    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Tehdit Koruması**        | | | 
| Saldırı yüzeyini azaltma özellikleri    | [Bu listeye bakın](#threat-protection) | Microsoft Edge için donanım tabanlı yalıtmanın kurumsal yönetimi | 
| Office 365 için Defender Plan 1 | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | Dahil değildir, ancak | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Active Directory (Azure AD) hesapları için self servis parola sıfırlama, Azure AD çok faktörlü kimlik doğrulaması (MFA), Koşullu Erişim, şirket içi kimlikler için parola geri yazma|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Bulut Uygulaması Bulma, Azure AD Connect Durumu    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Office 365 uygulamaları Tek Sign-On (SSO): Kullanıcı başına 10 uygulama (Salesforce gibi Galeri SaaS uygulamaları)* | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: sınır yok (Azure AD Uygulama Ara Sunucusu aracılığıyla şirket içi uygulamalar ve Self-Service Tümleştirme şablonlarını kullanan galeri dışı uygulamalar)    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Cihaz ve uygulama yönetimi**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Sanal Masaüstü Erişimi (VDA)    |  |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Windows Sanal Masaüstü (WVD)    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Paylaşılan Bilgisayar Etkinleştirmesi (SCA)    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Microsoft Masaüstü İyileştirme Paketi    | |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Bilgi koruması**        | | | 
| Office 365 Veri Kaybını Önleme, Azure Information Protection Plan 1    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uç nokta DLP için Pencere Bilgileri Koruması    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **İstemci Erişim Lisansı (CAL hakları)**    | | |     
| Kurumsal CAL Paketi (Exchange, SharePoint, Skype, Windows, Microsoft Uç Nokta Yapılandırma Yöneticisi, Windows Hak Yönetimi)| |         ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Uyumluluk**        | | | 
| Sınırsız e-posta arşivleme    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uyumluluk Yöneticisi    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| eKbulma    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Yerinde tutma ve mahkeme tutma    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| İleti Kayıt Yönetimi (MRM) bekletme etiketleri ve bekletme ilkeleri    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
||||

\* SaaS uygulamalarına erişim atanmış olan kullanıcılar en çok 10 uygulama için SSO erişimine sahip olabilir. Yöneticiler SSO'ya yapılandırarak kullanıcı erişimini farklı SaaS uygulamalarına değiştirebilir, ancak SSO erişimine her kullanıcı için bir defada yalnızca 10 uygulama izin verilir. Tüm Office 365 uygulamaları tek bir uygulama olarak sayılır.

## <a name="migration"></a>Geçiş

Geçiş yapmak için microsoft 365 İş Ekstra aboneliğinizi ve lisanslarınızı lisansları ile uygun bir Microsoft 365 E3 aboneliğine taşımak için iş ortağınız ile birlikte çalışabilirsiniz.

Aşağıdaki bölümlerde, varsa, hangi değişiklikleri yapmak için ihtiyacınız olduğu ve geçiş sonrasında neler yaptığınız açıklanmaktadır.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 abonelik yapılandırması ve verileri

Şu bilgileri içeren, geçerli aboneliğiniz veya verilerinizde değişiklik yapmak zorunda değilsiniz:

- DNS etki alanı adları gibi abonelik yapılandırması.
- Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.
- Teams, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve bunların verileri.

Kullanıcılarınız artık Exchange Online posta kutularında ve OneDrive İş klasörlerinden sınırsız depolamanın keyfini çıkarabilirsiniz.

10'dan fazla uygulama için Bulut Uygulama Bulma, Azure AD Connect Health ve SSO kullanmaya başlayabilirsiniz.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Tehdit koruması

Windows 10 Business şu korumaları içerir:

- İşletim sisteminin başlatma işleminin bütünlüğü zorlaması
- Hassas işletim bileşenlerinin bütünlüğünü zorlama
- Gelişmiş güvenlik açığı ve sıfır gün açıktan yararlanma azaltmaları
- Microsoft Edge, Internet Explorer ve Chrome için saygınlık tabanlı ağ koruması
- Ana bilgisayar tabanlı güvenlik duvarı
- Fidye yazılımı riskleri
- Microsoft Edge için donanım tabanlı yalıtma
- Akıllı Güvenlik Grafiği ile desteklenen uygulama denetimi
- Cihaz denetimi (USB)
- Web tabanlı tehditlere karşı ağ koruması
- Ana bilgisayar izinsiz giriş engelleme kuralları

Windows 10 Enterprise E3, Microsoft Edge için donanım tabanlı yalıtma yönetimini de içerir.

>[!Note]
>Microsoft 365 E3'e geçirilen kullanıcıların her biri, devam eden tehdit koruması için Office 365 için Microsoft Defender lisansı gerektirir. Office 365 için Defender'ın tüm kullanıcılarının lisanslı olması için ek Office 365 için Defender lisansları satın aldığınızdan emin olun. 
>

### <a name="device-management-with-intune"></a>Intune ile cihaz yönetimi

Kayıtlı cihazları ve cihaz ve uygulama ayarlarını içeren, başlamadan önce geçerli Intune yapılandırmanız üzerinde herhangi bir değişiklik yapmak zorunda değilsiniz.

### <a name="windows-10"></a>Windows 10

Microsoft 365 İş Ekstra, Windows AutoPilot ile yük885 İş'i içeren Windows 10 Business'ı içerir. Microsoft 365 E3'e geçişte, her kullanıcı lisansı Windows 10 Enterprise E3'ü içerir ve bu lisansı Windows Autopilot ile de yükleyebilirsiniz.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>İş için Microsoft 365 Uygulamaları

Cihazlarınıza yüklenmiş olan İş için Microsoft 365 Uygulamaları istemciniz, otomatik olarak kuruluş için Microsoft 365 Uygulamaları'nın özelliklerini kullanmaya başlar. Geçiş sonrasında artık şunları kullanabilirsiniz:

 - Grup İlkesi desteği
 - Elektronik tablo karşılaştırma ve sorgulama
 - İş zekası

