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
description: İşletmenizi yeni bir web Microsoft 365 İş Ekstra taşımayı Microsoft 365 E3.
ms.openlocfilehash: d3030518f7f4467c7b2e16897dc7b100764d9d5a36c50169b58f1adcd7bef209
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837643"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Geçiş Microsoft 365 İş Ekstra Microsoft 365 E3

Microsoft 365 İş Ekstra, sınıf için en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek çalışanlarınızı en iyi şekilde çalışmalarını sağlayacak şekilde küçük işletmeniz için gereken her şeye sahip olur. Bununla birlikte bazı durumlarda, Microsoft 365 İş Ekstra aboneliğinizi başka bir Microsoft 365 E3.

Örneğin, işletmeniz büyür ve 300'den fazla lisansa ihtiyacı vardır (bu arada tebrikler).

Ya da işletmenize İstemci Erişimi Lisansları (CA'lar) Kurumlar için Microsoft 365 Uygulamaları, Windows 10 Enterprise E3 veya Enterprise gibi kurumsal özellikler de gerekir.

Yükseltme kolaydır: Yükseltmeyi Yönetim [merkezinden başlatabilirsiniz.](../commerce/subscriptions/upgrade-to-different-plan.md) Geçerli aboneliğinizin tüm verileri ve yapılandırması korunur. Geçişe hazırlanmak için size bir şey yoktur ve sonrasında yeni özelliklerden yararlanmak dışında herhangi bir şey yapmaya gerek yoktur.

> [!NOTE]
> Ayrıca en çok 300 Microsoft 365 İş Ekstra için Microsoft 365 E3 aboneliği kullanabilir ve 300'den fazla Microsoft 365 E3 aboneliğine sahip olursınız. Bununla birlikte, Office 365 için Microsoft Defender bu ürün Microsoft 365 E3. Tehdit korumasına devam etmek için Office 365 için ek Defender lisansları eklemeniz gerekir. Böylelikle, Office 365 için Defender İlkeniz kapsamındaki tüm kullanıcılar lisanslara sahip olur.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>İki Microsoft 365 İş Ekstra arasındaki farklar Microsoft 365 Kurumsal

Bu tabloda, iki tablo Microsoft 365 İş Ekstra arasındaki farklar Microsoft 365 E3.

| Özellik    | Destek Microsoft 365 İş Ekstra    | Destek Microsoft 365 E3 |
|:-------|:-----|:-----|
| **Şirket içi**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office uygulamaları*    | [İş için Microsoft 365 Uygulamaları](#office-365-business)    | Microsoft 365 Kurumsal Uygulamaları |
| **Bulut üretkenlik uygulamaları**        | | |
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online arşivleme |
| Teams    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız |
| Yammer, SharePoint Online, Planner, Stream    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| **Tehdit Koruması**        | | |
| Saldırı yüzeyini azaltma özellikleri    | [Bu listeye bakın](#threat-protection) | Enterprise için donanım tabanlı yalıtımnın yönetimini Microsoft Edge |
| Office 365 için Defender Plan 1 | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | Dahil değildir, ancak |
| **Kimlik yönetimi**        | | |
| Karma kimlik bilgileri (Azure AD) Azure Active Directory, Azure AD multi-factor authentication (MFA), Koşullu Erişim için self servis parola sıfırlama, şirket içi kimlikler için parola geri yazma|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Bulut Uygulaması Keşif, Azure AD Bağlan Durumu    |     | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Office 365 Uygulamalar Tek Sign-On (SSO): Kullanıcı başına 10 uygulama (Salesforce gibi Galeri SaaS uygulamaları)* | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Premium 1 SSO kullanabilirsiniz: sınır yoktur (Azure AD Uygulama Ara Sunucusu üzerinden şirket içi uygulamalar ve Self-Service Tümleştirme şablonları kullanılarak galeri dışı uygulamalar)    |     | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| **Cihaz ve uygulama yönetimi**        | | |
| Microsoft Intune AutoPilot Windows'i çalıştırın|     ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
|Sanal Masaüstü Erişimi (VDA)    |  |     ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
|Windows Sanal Masaüstü (WVD)    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png) |     ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
|Paylaşılan Bilgisayar Etkinleştirmesi (SCA)    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png) |     ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Microsoft Masaüstü İyileştirme Paketi    | |     ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| **Bilgi koruması**        | | |
| Office 365 Veri Kaybını Önleme, Azure Information Protection Plan 1    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Uç nokta DLP için Window Information Protection    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| **İstemci Erişimi Lisansı (CAL hakları)**    | | |
| Enterprise CAL Paketi (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Yönetimi)| |         ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| **Uyumluluk**        | | |
| Sınırsız e-posta arşivleme    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Uyumluluk Yöneticisi    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| eKbulma    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| Yerinde tutma ve mahkeme tutma    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
| İleti Kayıtları Yönetimi (MRM) bekletme etiketleri ve bekletme ilkeleri    | ![Bu yeni Microsoft 365 İş Ekstra](../media/check-mark.png)    | ![Bu yeni Microsoft 365 E3](../media/check-mark.png) |
||||

\* SaaS uygulamalarına erişim atanmış olan kullanıcılar SSO'nun en çok 10 uygulamasına erişimi olabilir. Yöneticiler SSO'yi yapılandırarak kullanıcı erişimini farklı SaaS uygulamalarına değiştirebilir, ancak SSO erişimine bir defada kullanıcı başına yalnızca 10 uygulama izin verilir. Tüm Office 365 uygulamaları tek bir uygulama olarak sayılır.

## <a name="migration"></a>Geçiş

Geçiş yapmak için iş ortağınız ile birlikte çalışarak Microsoft 365 İş Ekstra lisansları olan uygun bir Microsoft 365 E3 aboneliğine geçin.

Aşağıdaki bölümlerde, geçiş sonrasında hangi değişiklikleri yapmak için ihtiyacınız olduğu ve varsa neler yapabilirsiniz açıklanmaktadır.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 yapılandırmasını ve verilerini yapılandırma

Şu gibi değişikliklerden önce geçerli aboneliğiniz veya verilerinizde değişiklik yapmak zorunda değilsiniz:

- DNS etki alanı adları gibi abonelik yapılandırması.
- Çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ile kimlik doğrulama ayarları.
- Üretkenlik hizmeti yapılandırmaları ve Teams, Exchange Online kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve not defterleri gibi verileri OneNote.

Kullanıcılarınız artık posta kutularına ve posta kutularına sınırsız Exchange Online keyfini OneDrive İş keyfini çıkarabilirsiniz.

10'dan fazla uygulamada Bulut Uygulama Bulma, Azure AD Bağlan Health ve SSO kullanmaya başlayabilirsiniz.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Tehdit koruması

Windows 10 Business şu korumaları içerir:

- İşletim sisteminin önyükleme işleminin bütünlüğü zorlaması
- Hassas işletim bileşenlerinin bütünlükle zorlaması
- Gelişmiş güvenlik açığı ve sıfır gün açıkları açıkları azaltma
- İnternet Explorer ve Chrome'da Microsoft Edge tabanlı ağ koruması
- Ana bilgisayar tabanlı güvenlik duvarı
- Fidye yazılımı azaltma
- Sistem için donanım tabanlı Microsoft Edge
- Akıllı Güvenlik Tarafından desteklenen uygulama Graph
- Cihaz denetimi (USB)
- Web tabanlı tehditlere karşı ağ koruması
- Host intrusion prevention rules

Windows 10 Enterprise E3, teknik destek için donanım tabanlı yalıtım kurumsal yönetimini Microsoft Edge.

> [!NOTE]
> Microsoft 365 E3'a Microsoft 365 E3 devam eden tehdit koruması için Office 365 için Microsoft Defender gerekir. Güvenlik İlkeleri için Defender Office 365 kapsamındaki tüm kullanıcıların lisanslı olması için ek Office 365 Defender satın aldığınızdan emin olun.

### <a name="device-management-with-intune"></a>Intune ile cihaz yönetimi

Kayıtlı cihazları ve cihaz ve uygulama ayarlarını da içeren, başlamadan önce geçerli Intune yapılandırmanız üzerinde değişiklik yapmak zorunda değilsiniz.

### <a name="windows-10"></a>Windows 10

Microsoft 365 İş Ekstra, Windows 10 Business AutoPilot ile yüklerini Windows içerir. Microsoft 365 E3'e geçiş Microsoft 365 E3, her kullanıcı lisansı Windows 10 Enterprise E3 içerir; bu E3'ü AutoPilot Windows da yükleyebilirsiniz.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>İş için Microsoft 365 Uygulamaları

Cihazlarınıza İş için Microsoft 365 Uygulamaları bilgisayarınıza yüklenmiş olan kullanıcı istemciniz, sistem özelliklerinin otomatik olarak Kurumlar için Microsoft 365 Uygulamaları. Geçiş sonrasında şunları kullanabilirsiniz:

- Grup İlkesi desteği
- Elektronik tablo karşılaştırma ve sorgulama
- İş Zekası
