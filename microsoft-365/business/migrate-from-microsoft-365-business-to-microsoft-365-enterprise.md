---
title: Microsoft 365 Business 'dan Microsoft 365 E3 uygulamasına geçme
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
description: İşletmenizi Microsoft 365 Business Premium 'dan Microsoft 365 E3 'e taşımayı öğrenin.
ms.openlocfilehash: 874da0d35759c8af4c3ee2ca4a1bdfa90a91627c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842210"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Microsoft 365 Business Premium 'dan Microsoft 365 E3

Microsoft 365 Business Premium, çalışanlarınızın en iyi işlerini yapmalarına olanak tanıyan, en iyi bulut tabanlı bulut uygulamalarını basit cihaz yönetimi ve güvenliğiyle birleştiren, küçük işletme için gereken her şeyi içerir. Ancak bazı durumlarda Microsoft 365 Business Premium aboneliğinizi Microsoft 365 E3 'e düzenlemeniz gerekebilir. 

Örneğin, işletmeniz 300 lisanlarından daha fazlasını (Tebrikler, tebrikler) en çok büyümüştür ve gereksinim duyar.

Veya işiniz, kurumsal Microsoft 365 uygulamaları, Windows 10 Enterprise E3 veya kurumsal Istemci erişim lisansları (CAL) gibi Kurumsal özelliklere ihtiyaç duyar.

Yükseltme işlemi kolaydır: yükseltmeye [Yönetim merkezinden](../commerce/subscriptions/upgrade-to-different-plan.md)başlayabilirsiniz. Geçerli aboneliğinizde tüm verileriniz ve yapılandırmanız korunur. Yeni özelliklerden yararlanmak dışında, Geçişe hazırlanmak için hiçbir şey olmuyor ve bundan sonra hiçbir şey olmuyor.

>[!Note]
>300 oturun kadar Microsoft 365 Iş ekstra aboneliği de kullanabilir ve 300 bir E3 aboneliği için bir Microsoft 365 aboneliği edinebilirsiniz. Ancak, Office 365 için Microsoft Defender, Microsoft 365 E3. Devam eden tehdit koruması için, Office 365 ilkeleriyle ilgili tüm kullanıcıların lisanslı olması için Office 365 lisansları için ek Defender 'ı eklemeniz gerekir.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Microsoft 365 Business Premium ve Microsoft 365 Enterprise arasındaki farklar

Bu tabloda, Microsoft 365 Business Premium ve Microsoft 365 E3 arasındaki farklılıklar gösterilmektedir.

| Özellik    | Microsoft 365 Business Premium 'da destek    | Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Şirket içi**        | | | 
| Windows 10    | Windows 10 Iş  |     Windows 10 Kurumsal E3| 
| Office uygulamaları *    | [İş için Microsoft 365 uygulamaları](#office-365-business)    | Microsoft 365 Kurumsal Uygulamaları | 
| **Bulut üretkenlik uygulamaları**        | | | 
| Exchange Online ve Outlook    | posta kutusu başına 50 GB depolama alanı ve sınırsız Exchange Online arşivleme    | posta kutusu başına 100 GB depolama alanı ve sınırsız Exchange Online arşivleme | 
| Teams    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| OneDrive İş    | Kullanıcı başına 1 TB depolama sınırı    | Süresiz | 
| Yammer, SharePoint Online, Planner, akış    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | | 
| **Tehdit koruması**        | | | 
| Attack Surface azaltma özellikleri    | [Bu listeye bakın](#threat-protection) | Microsoft Edge için donanım tabanlı yalıtımın Kurumsal Yönetimi | 
| Office 365 plan 1 için Defender | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | Dahil değildir, ancak eklenebilir | 
| **Kimlik yönetimi**        | | | 
| Karma Azure Active Directory (Azure AD) hesapları, Azure Multi-Factor Authentication (MFA) için self servis parola sıfırlama, koşullu erişim, şirket içi kimlikler için parola geri yazma|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Bulut uygulama keşfi, Azure AD Connect durumu    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Office 365 uygulamaları tek Sign-On (SSO): Kullanıcı başına 10 uygulama (örneğin, Salesforce gibi Galeri SaaS uygulamaları) * | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: sınırsız (Azure AD uygulaması proxy 'Si ile şirket içi uygulamalar, Self-Service uygulama tümleştirme şablonları kullanılarak Galeri dışı uygulamalar)    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Cihaz ve uygulama yönetimi**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Sanal masaüstü erişimi (VDA)    |  |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Windows sanal masaüstü (WVD)    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|Paylaşılan bilgisayar etkinleştirmesi (SCA)    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Microsoft Masaüstü Iyileştirme paketi    | |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Bilgi koruması**        | | | 
| Office 365 veri kaybı önleme, Azure bilgi koruma planı 1    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uç nokta DLP için pencere bilgileri koruması    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **İstemci erişim lisansı (CAL hakları)**    | | |     
| Kurumsal CAL Paketi (Exchange, SharePoint, Skype, Windows, Microsoft uç nokta Yapılandırma Yöneticisi, Windows hak yönetimi)| |         ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| **Uyum**        | | | 
| Sınırsız e-posta arşivleme    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Uyumluluk Yöneticisi    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Eş    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Yerinde saklama ve dava tutma    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| Mesajlaşma kaydı yönetimi (MRM) bekletme etiketleri ve bekletme ilkeleri    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
||||

\* SaaS uygulamalarına erişim atanmış kullanıcılar, en fazla 10 uygulamaya SSO erişimi alabilirler. Yöneticiler SSO 'yu yapılandırabilir ve farklı SaaS uygulamalarına Kullanıcı erişimini değiştirebilir, ancak SSO erişimine aynı anda Kullanıcı başına 10 uygulama için izin verilir. Tüm Office 365 uygulamaları tek bir uygulama olarak sayılır.

## <a name="migration"></a>Geçişte

Taşımak için, iş ortağınızla birlikte çalışarak Microsoft 365 Business Premium aboneliğinizi ve lisanslarınızı lisanlarıyla uygun bir Microsoft 365 E3 aboneliğine taşıyın.

Aşağıdaki bölümlerde, eğer varsa ve geçiş sonrasında yapabileceğiniz değişiklikler açıklanmaktadır.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 aboneliği yapılandırması ve verileri

Geçirmeden önce geçerli aboneliğinizde veya verilerinizde herhangi bir değişiklik yapmanız gerekmez, aşağıdakileri içerir:

- DNS etki alanı adları gibi abonelik yapılandırması.
- Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.
- Üretkenlik hizmeti yapılandırmaları ve takımlar, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive Iş klasörleri ve OneNote Not defterleri gibi verileri.

Kullanıcılarınız artık Exchange Online posta kutuları ve OneDrive Iş klasörlerindeki sınırsız depolama alanını kullanabilir.

10 ' dan fazla uygulama için bulut uygulaması keşfi, Azure AD Connect sağlık ve SSO kullanmaya başlayabilirsiniz.

>[!Note]
>Microsoft 365 E3 'e geçirilen kullanıcılar artık Outlook Customer Manager ve MileIQ 'i kullanamaz.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Tehdit koruması

Windows 10 Business bu korumaları içerir:

- İşletim sistemi önyükleme işleminin bütünlüğü zorlaması
- Hassas işletim bileşenlerinin bütünlüğünü zorlamayı
- Gelişmiş Güvenlik Açığı ve sıfır günlük yararlanma azaltıcı etkenleri
- Microsoft Edge, Internet Explorer ve Chrome için, saygınlık tabanlı ağ koruması
- Ana bilgisayar tabanlı güvenlik duvarı
- Fidye yazılımı azaltıcı etkenleri
- Microsoft Edge için donanım tabanlı yalıtım
- Akıllı güvenlik grafiği tarafından desteklenen uygulama denetimi
- Aygıt denetimi (USB)
- Web tabanlı tehditler için ağ koruması
- Barındırma önleme kuralları

Windows 10 Enterprise E3, Microsoft Edge için donanım tabanlı yalıtımın kurumsal yönetimini de içerir.

>[!Note]
>Microsoft 365 E3 'e geçirilen kullanıcıların, sürekli tehdit koruması için Office 365 için bir Microsoft Defender lisansı gerekir. Office 365 ilkeleriyle ilgili tüm kullanıcıların lisanslı olması için Office 365 lisansları için ek Defender 'ı satın aldığınızdan emin olun. 
>

### <a name="device-management-with-intune"></a>Intune ile cihaz yönetimi

Geçiş yapmadan önce, kayıtlı cihazları ve cihaz ve uygulama ayarlarını içeren geçirmeden önce geçerli Intune yapılandırmanızda değişiklik yapmanız gerekmez.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Iş ekstra, Windows AutoPilot ile yükleyebileceğiniz Windows 10 Iş 'i içerir. Microsoft 365 E3 'e geçiş yaptığınızda, her kullanıcı lisansı Windows Autopilot ile de yükleyebileceğiniz Windows 10 Kurumsal E3 içerir.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>İş için Microsoft 365 uygulamaları

Cihazlarınızda yüklü iş için Microsoft 365 uygulamalarınız, kuruluşunuzdaki Microsoft 365 Apps özelliklerini otomatik olarak kullanmaya başlayacaktır. Geçiş sonrasında şunları kullanabilirsiniz:

 - Grup Ilkesi aracılığıyla toplu etkinleştirme
 - Uygulama telemetri
 - Güncelleştirme denetimleri
 - Elektronik tablo karşılaştırma ve sorgulama
 - İş zekası

