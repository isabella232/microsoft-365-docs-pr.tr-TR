---
title: Microsoft 365 İş Ekstra'daki koruma özellikleri Intune ayarlarıyla nasıl eşler
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
ms.date: 8/13/2018
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Microsoft 365 İş Ekstra'daki koruma özelliklerinin Intune ayarlarıyla nasıl eş olduğunu öğrenin. Abonelik size Intune ayarlarını değiştirme lisansı sağlar.
ms.openlocfilehash: 9a6dcf014e009389e49860fa96486c264c22f501
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580124"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Microsoft 365 İş Ekstra'daki koruma özellikleri Intune ayarlarıyla nasıl eşler

## <a name="android-and-ios-application-protection-settings"></a>Android ve iOS uygulama koruma ayarları

Aşağıdaki tabloda, Android ve iOS uygulama ilkesi ayarlarının Intune ayarlarıyla nasıl eşlendiği ayrıntılarıyla gösterilir.
  
Intune ayarını bulmak için, Microsoft 365 İş Ekstra yönetici kimlik bilgilerinizle oturum açmalı, Yönetim merkezlerine ve **ardından Intune'a gidin.**
  
 > [!IMPORTANT]
 > 
 > Microsoft 365 İş Ekstra aboneliği size tüm Intune ayarlarını değiştirme lisansı verir. Başlamak [için Intune'a Giriş'e bakın.](/intune/introduction-intune)
  
İstediğiniz İlke adını &mdash; seçin( örneğin, Android için Uygulama ilkesi) ve &mdash; ardından İlke **ayarları'ı seçin.**
  
**Cihaz kaybolursa veya çalınırsa iş dosyalarını koru** alanında
  
|**Android veya iOS uygulama ilkesi ayarı**|**Intune ayarları**|
|:-----|:-----|
|Şu süre sonunda iş dosyalarını etkin olmayan cihazdan sil  <br/> |Uygulama verileri temizlenmeden önce geçen çevrimdışı süre (gün cinsinden)  <br/> |
|Kullanıcıları, iş dosyalarını OneDrive İş'e kaydetmeye zorla  <br/> Yalnızca OneDrive İş'e izin verildiğini unutmayın  <br/> |Şirket verilerinin kaydedileceği depolama hizmetlerini seçin  <br/> |
|||
   
**Kullanıcının mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** alanında
  
|**Android veya iOS uygulama ilkesi ayarı**|**Intune ayarları**|
|:-----|:-----|
|Şu süre sonunda iş dosyalarını etkin olmayan cihazdan sil  <br/> |Uygulama verileri temizlenmeden önce geçen çevrimdışı süre (gün cinsinden)  <br/> |
|Kullanıcıları, iş dosyalarını OneDrive İş'e kaydetmeye zorla  <br/> Yalnızca OneDrive İş'e izin verildiğini unutmayın  <br/> |Şirket verilerinin kaydedileceği depolama hizmetlerini seçin  <br/> |
|İş dosyalarını şifrele  <br/> |Uygulama verilerini şifrele  <br/> |
|**Kullanıcının mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** alanında <br/> ||
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> | Erişim için PIN iste  <br/>  Ayrıca şu ayarları da yapar:  <br/> **Basit PIN'e İzin Ver** için **Evet** <br/> **PIN Uzunluğu** için 4  <br/> **PIN yerine parmak izine izin ver** için **Evet** <br/> **Cihaz PIN'i yönetildiğinde uygulama PIN'ini devre dışı bırakma** için **Hayır** <br/> |
|Oturum açma başarısız olduğunda PIN'i sıfırla (PIN gerekli değilse bu devre dışı bırakılır)  <br/> |PIN sıfırlamadan önceki deneme sayısı  <br/> |
|Office uygulamaları boşta kaldıktan sonra kullanıcıların yeniden oturum açmasını gerektir (PIN gerekmiyorsa bu devre dışı bırakılır)  <br/> | Şu sürenin ardından erişim gereksinimlerini yeniden denetle (dakika cinsinden)  <br/>  Ayrıca şu ayarları da yapar:  <br/> **Zaman aşımı** dakika sayısına ayarlanır  <br/>  Bu, Microsoft 365 İş içinde ayarladığınız dakika sayısıyla aynıdır.  <br/> **Çevrimdışı tanınan süre** değeri varsayılan olarak 720 dakikaya ayarlanır  <br/> |
|İşletim sistemi kısıtlamaları kaldırılmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle  <br/> |Yönetilen uygulamaların işletim sistemi kısıtlamaları kaldırılmış veya kök erişim izni verilmiş cihazlarda çalışmasını engelle  <br/> |
|Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver  <br/> | Diğer uygulamalarla kesme, kopyalama ve yapıştırmayı kısıtla  <br/>  Microsoft 365 İş Ekstra seçeneği Açık olarak ayarlanmışsa, bu üç seçenek Intune'daki **Tüm Uygulamalar olarak** da ayarlanır:  <br/> **Uygulamanın diğer uygulamalara veri aktarmasına izin ver** <br/> **Uygulamanın diğer uygulamalardan veri almasına izin ver** <br/> **Diğer uygulamalarla kesme, kopyalama ve yapıştırmayı kısıtla** <br/>  Microsoft 365 İş seçeneği **Açık** olarak ayarlandıysa, tüm Intune seçenekleri şöyle ayarlanır:  <br/> **Uygulamanın diğer uygulamalara veri aktarmasına izin ver** seçeneği **İlke ile yönetilen uygulamalar** olarak ayarlanır <br/> **Uygulamanın diğer uygulamalardan veri almasına izin ver** seçeneği **Tüm Uygulamalar** olarak ayarlanır <br/> **Diğer uygulamalarla kesme, kopyalama ve yapıştırmayı kısıtla** seçeneği **İçine Yapıştırmayla İlke ile Yönetilen Uygulamalar** olarak ayarlanır <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10 uygulama koruma ayarları

Aşağıdaki tabloda, Windows 10 uygulama ilkesi ayarlarının Intune ayarlarıyla nasıl eşlendiği ayrıntılarıyla gösterilir.
  
Intune ayarını bulmak için Microsoft 365 İş Ekstra yönetici kimlik bilgilerinizle oturum açın ve [Azure portalına gidin.](https://portal.azure.com) Diğer **hizmetler'i** seçin ve Filtre'ye Intune **yazın.** **Intune Uygulama Koruma Uygulama** \> **İlkesi'ne seçin.**
  
 > [!IMPORTANT]
 >
 >Microsoft 365 İş Ekstra aboneliği, size yalnızca Microsoft 365 İş Ekstra'da bulunan ayarlarla eşananlı Intune ayarlarını değiştirme lisansı verir. 
  
Kullanılabilir ayarları keşfetmek için, istediğiniz ilke adını seçin ve ardından sol gezinti bölmesinde  **Genel,** Ödevler, **İzin** verilen uygulamalar, Muaf uygulamalar, Gerekli ayarlar veya Gelişmiş ayarlar'ı seçin.   
  
|**Windows 10 uygulama ilkesi ayarı**|**Intune ayarları**|
|:-----|:-----|
|İş dosyalarını şifrele  <br/> |**Gelişmiş ayarlar** \> **Veri koruma**: **Kayıt kaldırılırken şifreleme anahtarlarını iptal et** ve **Cihaz MDM'ye kaydedildiğinde korumalı verilere erişimi iptal et** seçeneklerinin ikisi de **Açık** olarak ayarlanır.  <br/> |
|Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engeller.  <br/> |**Gerekli ayarlar** \> **Windows Bilgi Koruması modu**.  Microsoft 365 İş Ekstra haritalarında açık: **Geçersiz** Kılmaları **Gizle,** Microsoft 365 İş Ekstra haritalarında Kapalı: **Kapalı.**  <br/> |
|Office belgeleri erişimi denetimi  <br/> | Bu ayar Microsoft  365 İş Ekstra'da Açık olarak ayarlanmışsa  <br/> **Gelişmiş ayarlar** \> **Erişim**, **Windows'ta oturum açma yöntemi olarak İş İçin Windows Hello kullan** seçeneği **Açık** olarak ayarlanır ve aşağıdaki ek ayarlar da yapılır:  <br/> **PIN için gerekli en az karakter sayısını ayarla** seçeneği **4** olarak ayarlanır.  <br/> **İş İçin Windows Hello PIN'inde büyük harf kullanımını yapılandır** seçeneği **PIN için büyük harf kullanımına izin verme** olarak ayarlanır.  <br/> **İş İçin Windows Hello PIN'inde küçük harf kullanımını yapılandır** seçeneği **PIN için küçük harf kullanımına izin verme** olarak ayarlanır.  <br/> **İş İçin Windows Hello PIN'inde özel karakter kullanımını yapılandır** seçeneği **PIN'de özel karakter kullanımına izin verme** olarak ayarlanır.  <br/> **Sistemin kullanıcının 0 olarak** değişmesini gerektirmeden önce PIN'in kullanılma süresi (gün olarak) **belirtin.**  <br/> **Tekrar kullanılamayan bir kullanıcı hesabı ile ilişkili eski PIN'lerin sayısını belirtin** seçeneği **0** olarak ayarlanır.  <br/> **Cihaz silinmeden önce izin verilen kimlik doğrulama hatası sayısı** seçeneği Microsoft 365 İş'tekiyle aynı değere ayarlanır (varsayılan olarak 5).  <br/> **Cihazın PIN'inin veya parolasının kilitlenmesine neden olan izin verilen en uzun boşta kalma süresi (dakika cinsinden)** seçeneği Microsoft 365 İş'tekiyle aynı değere ayarlanır.  <br/> |
|Korumalı verilerde kurtarmayı etkinleştir  <br/> |**Gelişmiş ayarlar** \> **Veri koruma**: **Kurumsal verileri koruma simgesini göster** ve **WIP için Azure RMS kullan** seçenekleri **Açık** olarak ayarlanır.  <br/> |
|Ek şirket bulut konumlarını koru  <br/> |**Gelişmiş ayarlar** \> **Korunan etki alanları** ve **Bulut kaynakları**, etki alanlarını ve SharePoint sitelerini gösterir.  <br/> |
|Bu uygulamaların kullandığı dosyalar korunur  <br/> |Korunan uygulamalar, **İzin verilen uygulamalar**'da listelenir.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Windows 10 cihaz koruma ayarları

Aşağıdaki tabloda, Windows 10 cihaz yapılandırma ayarlarının Intune ayarlarıyla nasıl eşlendiği ayrıntılarıyla gösterilir.
  
Intune ayarını bulmak için Microsoft 365 İş Ekstra yönetici kimlik bilgilerinizle oturum açın ve [Azure portalına](https://portal.azure.com)gidin, Daha fazla hizmet seçin ve Intune'a **Filtre'ye** yazın, **Intune** Cihaz yapılandırma Profilleri'ni \>  \> seçin. Ardından, **Windows 10 Için Cihaz İlkesi Özellikleri** \> **Ayarları'ı** \> **seçin.**
  
|**Windows 10 cihazı ilkesi ayarı**|**Intune ayarları**|
|:-----|:-----|
|Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol  <br/> |Gerçek Zamanlı İzlemeye İzin Ver = Açık  <br/> Bulut Korumasına İzin Ver = Açık  <br/> Kullanıcılardan Örnek Göndermelerini İste = Güvenli örnekleri otomatik olarak gönder (Varsayılan PII dışını otomatik gönder)  <br/> |
|Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol  <br/> |**Edge Tarayıcı Ayarları**'nda **SmartScreen** seçeneği **Gerekli** olarak ayarlanır.  <br/> |
|Cihaz şu kadar süreyle boşta kaldığında ekranı kapat (dakika)  <br/> |Ekran kilitlenmeden önce geçmesi gereken, işlem yapılmayan dakika sayısı  <br/> |
|Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver  <br/> |Özel URI ilkesi  <br/> |
|Kullanıcıların Cortana'ya erişmesine izin ver  <br/> |**Genel** \> **Cortana,** Microsoft  365 İş Ekstra'da kapalı olarak **ayar olduğunda** Intune'da engellenir.  <br/> |
|Kullanıcıların Microsoft'tan Windows ipucu ve reklam almasına izin ver  <br/> |**Microsoft** 365 İş Ekstra'da kapalı olarak **ayarlanırsa** Windows öne çıkanlar, hepsi engellenir.  <br/> |
|Windows 10 cihazları otomatik olarak güncelleştir  <br/> | Bu ayar **Microsoft Intune** Hizmeti güncelleştirmeleri - Windows 10 Güncelleştirme Halkaları'nın \> içindedir, **Windows 10** cihazları için Güncelleştirme ilkesi'ne ve ardından Özellikler Ayarları'nın **seçin.** \>   <br/>  Microsoft 365 İş Ekstra ayarı Açık olarak **ayar olduğunda,** aşağıdaki tüm ayarlar ayarlanır:  <br/> **Hizmet dalı** **CB** olarak ayarlanır (Microsoft 365 İş Ekstra'da bu kapalıyken CBB).  <br/> **Microsoft ürün güncelleştirmeleri** seçeneği **İzin ver** olarak ayarlanır.  <br/> **Windows sürücüleri** seçeneği **İzin ver** olarak ayarlanır.  <br/> **Otomatik güncelleştirme davranışı** seçeneği **Bakım zamanında otomatik yükle** olarak ayarlanır ve:  <br/> **Etkin saatlerin başlangıcı** için **06:00** ayarlanır.  <br/> **Etkin saatlerin sonu** için **22:00** ayarlanır.  <br/> **Kalite güncelleştirmesi erteleme süresi (gün)** için **0** ayarlanır.  <br/> **Özellik güncelleştirmesi erteleme süresi (gün)** için **0** ayarlanır.  <br/> **Teslimi iyileştirme indirme modu** için **Aynı NAT arkasında eşleme ile karışık HTTP** ayarlanır.  <br/> |
|||
