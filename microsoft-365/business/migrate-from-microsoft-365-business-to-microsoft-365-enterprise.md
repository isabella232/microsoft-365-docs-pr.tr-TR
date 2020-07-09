---
title: Microsoft 365 Business'tan Microsoft 365 E3'e geçiş
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
description: İşletmenizi Microsoft 365 Business Premium'dan Microsoft 365 E3'e nasıl taşıyacın öğrenin.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081921"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Microsoft 365 Business Premium'dan Microsoft 365 E3'e geçiş

Microsoft 365 Business Premium, çalışanlarınızın en iyi işlerini yapmalarını sağlayan basit cihaz yönetimi ve güvenlikle sınıfının en iyisi bulut tabanlı üretkenlik uygulamalarını birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahiptir. Ancak bazı durumlarda, Microsoft 365 Business Premium aboneliğinizi Microsoft 365 E3'e geçirmeniz gerekebilir. 

Örneğin, işletmeniz büyüdü ve 300'den fazla lisansa ihtiyacı var (tebrikler, bu arada).

Veya işletmenizin kurumsal için Microsoft 365 Uygulamaları, Windows 10 Kurumsal E3 veya Kurumsal İstemci Erişim Lisansları (CALs) gibi kurumsal özelliklere ihtiyacı vardır.

Yükseltme kolaydır: [Yükseltmeyi Yönetici merkezinden](../commerce/subscriptions/upgrade-to-different-plan.md)başlatabilirsiniz. Geçerli aboneliğinizdeki tüm verileriniz ve yapılandırmanız korunur. Geçişe hazırlanmak için yapacak bir şeyiniz yok ve yeni özelliklerden yararlanmak dışında daha sonra yapacak bir şey yok.

>[!Note]
>Ayrıca 300'e kadar koltuk için Microsoft 365 Business Premium aboneliği kullanabilir ve 300'den fazla koltuk için Microsoft 365 E3 aboneliği alabilirsiniz. Ancak, Office 365 ATP Microsoft 365 E3 dahil değildir. Sürekli tehdit koruması için, Office 365 ATP polisleriniz kapsamındaki tüm kullanıcıların lisanslı olması için ek Office 365 ATP lisansları eklemeniz gerekir.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Microsoft 365 Business Premium ve Microsoft 365 Enterprise arasındaki farklar

Bu tablo, Microsoft 365 Business Premium ve Microsoft 365 E3 arasındaki farkları gösterir.

| Özellik    | Microsoft 365 Business Premium desteği    | Microsoft 365 E3 desteği | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Windows 10    | Windows 10 İş  |     Windows 10 Kurumsal E3| 
| Ofis uygulamaları*    | [Microsoft 365 İş uygulamaları](#office-365-business)    | Kurumsal uygulamalar için Microsoft 365 | 
| **Bulut üretkenliği uygulamaları**        | | | 
| Exchange Online ve Outlook    | Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online arşivleme    | Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online arşivleme | 
| Takım    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Sınırsız | 
| Yammer, SharePoint Online, Planlayıcı, Akış    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Outlook Müşteri Yöneticisi, MileIQ    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | | 
| **Tehdit Koruması**        | | | 
| Saldırı yüzey azaltma yetenekleri    | [Bu listeye bakın](#threat-protection) | Microsoft Edge için donanım tabanlı yalıtımın kurumsal yönetimi | 
| Office 365 Gelişmiş Tehdit Koruması (ATP) Planı 1 | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | Dahil değil, ancak eklenebilir | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Etkin Dizin (Azure AD) hesapları, Azure çok faktörlü kimlik doğrulama (MFA), Koşullu Erişim, şirket içi kimlikler için parola yazma için self servis parola sıfırlama|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Bulut Uygulaması Bulma, Azure AD Connect Health    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Office 365 uygulamaları Tek Oturum Açma (SSO): Kullanıcı başına 10 uygulama (Salesforce gibi Galeri SaaS uygulamaları)* | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: limitsiz (Azure AD Uygulama Proxy'si aracılığıyla şirket içi uygulamalar ve Self Servis Uygulama Tümleştirme şablonlarını kullanan galeri dışı uygulamalar)    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Cihaz ve uygulama yönetimi**        | | | 
| Microsoft Intune, Windows Otomatik Pilot|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Sanal Masaüstü Erişimi (VDA)    |  |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Windows Sanal Masaüstü (WVD)    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Paylaşılan Bilgisayar Etkinleştirme (SCA)    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Microsoft Masaüstü Optimizasyon Paketi    | |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Bilgi koruması**        | | | 
| Office 365 Veri Kaybıönleme, Azure Bilgi Koruma Planı 1    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uç nokta DLP için Pencere Bilgi Koruması    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **İstemci Erişim Lisansı (CAL hakları)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Hakları Yönetimi)| |         ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Uyumlu -luk**        | | | 
| Sınırsız e-posta arşivleme    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uyumluluk Puanı/Uyumluluk Yöneticisi    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Ediscovery    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Yerinde bekleme ve dava tutma    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Mesajlaşma Kayıtları Yönetimi (MRM) bekletme etiketleri ve bekletme ilkeleri    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
||||

\*SaaS uygulamalarına erişim izni alan kullanıcılar, SSO'nun en fazla 10 uygulamaya erişebiliyor. Yöneticiler SSO'yı yapılandırabilir ve kullanıcı erişimini farklı SaaS uygulamalarına değiştirebilir, ancak SSO erişimine aynı anda kullanıcı başına yalnızca 10 uygulama için izin verilir. Tüm Office 365 uygulamaları tek bir uygulama olarak sayılır.

## <a name="migration"></a>Geçiş

Geçiş yapmak için, Microsoft 365 Business Premium aboneliğinizi ve lisanslarınızı lisansları olan uygun bir Microsoft 365 E3 aboneliğine taşımak için iş ortağınızla birlikte çalışın.

Aşağıdaki bölümlerde, varsa hangi değişiklikleri yapmanız gerektiği ve geçişten sonra neler yapabileceğiniz açıklanabilir.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 abonelik yapılandırması ve verileri

Geçiş yapmadan önce geçerli aboneliğinizde veya verilerinizde herhangi bir değişiklik yapmanız gerekmez:

- DNS etki alanı adları gibi abonelik yapılandırması.
- Çok faktörlü kimlik doğrulama veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ve kimlik doğrulama ayarları.
- Ekipler, Exchange Online posta kutuları, SharePoint Online siteleri, İş için OneDrive klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve verileri.

Kullanıcılarınız artık Exchange Online posta kutularında ve İş için OneDrive klasörlerinde sınırsız depolama alanının keyfini çıkarabilir.

10'dan fazla uygulama için Cloud App Discovery, Azure AD Connect Health ve SSO'yı kullanmaya başlayabilirsiniz.

>[!Note]
>Microsoft 365 E3'e geçirilen kullanıcılar artık Outlook Müşteri Yöneticisi ve MileIQ kullanamaz.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Tehdit koruması

Windows 10 İş bu korumaları içerir:

- İşletim sistemi önyükleme işleminin bütünlük uygulaması
- Hassas işletim bileşenlerinin bütünlük zorlama
- Gelişmiş güvenlik açığı ve sıfır gün istismarı azaltımları
- Microsoft Edge, Internet Explorer ve Chrome için itibar tabanlı ağ koruması
- Ana bilgisayar tabanlı güvenlik duvarı
- Ransomware azaltma
- Microsoft Edge için donanım tabanlı yalıtım
- Akıllı Güvenlik Grafiği ile desteklenen uygulama denetimi
- Cihaz kontrolü (USB)
- Web tabanlı tehditler için ağ koruması
- Ev sahibi izinsiz giriş önleme kuralları

Windows 10 Enterprise E3, Microsoft Edge için donanım tabanlı yalıtımın kurumsal yönetimini de içerir.

>[!Note]
>Microsoft 365 E3'e geçirilen kullanıcıların her biri sürekli tehdit koruması için bir Office 365 ATP lisansı gerektirir. Office 365 ATP polisleriniz kapsamındaki tüm kullanıcıların lisanslı olması için ek Office 365 ATP lisansları satın aldığından emin olun. 
>

### <a name="device-management-with-intune"></a>Intune ile cihaz yönetimi

Geçiş yapmadan önce kayıtlı aygıtlar, aygıtlar ve uygulama ayarlarını içeren geçerli Intune yapılandırmanızda herhangi bir değişiklik yapmanız gerekmez.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium, Windows AutoPilot ile yükleyebileceğiniz Windows 10 Business'ı içerir. Microsoft 365 E3'e geçiş yaptığınızda, her kullanıcı lisansı, Windows Autopilot ile de yükleyebileceğiniz Windows 10 Enterprise E3 içerir.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 İş uygulamaları

Cihazlarınızda yüklü olan Microsoft 365 Apps iş istemcisi için Uygulamalarınız, kurumsal olarak Microsoft 365 Apps özelliklerini otomatik olarak kullanmaya başlar. Geçişten sonra artık şunları kullanabilirsiniz:

 - Grup İlkesi ile birim etkinleştirme
 - Uygulama telemetrisi
 - Denetimleri güncelleştirme
 - Elektronik tablo karşılaştırın ve sorgulayın
 - İş zekası

