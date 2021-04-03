---
title: Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Android veya iOS cihazlarda uygulama yönetimi ilkesi oluşturma, düzenleme veya silmeyi ve iş dosyalarını korumayı öğrenin.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580304"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme

Bu makale Microsoft 365 İş Ekstra için geçerlidir.

## <a name="create-an-app-management-policy"></a>Uygulama yönetimi ilkesi oluşturma

1. Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin: 
    
2. Sol gezintide Cihaz **İlkeleri** \> **Ekle'yi** \> **seçin.**
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. İlke **türü altında,** oluşturmak **istediğiniz ilke** kümesine bağlı olarak Android için Uygulama Yönetimi'ne veya **iOS** için Uygulama Yönetimi'ne tıklayın. 
    
5. Cihazlar **kaybolur veya çalınırsa iş dosyalarını koru'ya** ve kullanıcıların mobil **cihazlarda Office dosyalarına nasıl erişeceklerini yönet'i genişletin.** Ayarları istediğiniz gibi yapılandırabilirsiniz. **Kullanıcıların mobil cihazlarda Office dosyalarına** nasıl erişeceklerini yönetme varsayılan olarak Kapalıdır, ancak bu ayarı açmanız **ve** varsayılan değerleri kabul etmenizi öneririz.  Daha fazla bilgi için Bkz. [Kullanılabilir ayarlar](#available-settings). 
    
    Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Varsayılan Tüm Kullanıcılar güvenlik grubunu kullanmak **istemiyorsanız** Değiştir'i **seçin,** bu ayarları alan güvenlik gruplarını \> **seçin.**
    
7. Son olarak, **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="edit-an-app-management-policy"></a>Uygulama yönetimi ilkesini düzenleme

1. **İlkeler kartında** İlkeyi **düzenle'yi seçin.**
    
2. **İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin. 
    
3. İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin. Bir değeri değiştirseniz, otomatik olarak ilkeye kaydedilir.
    
4. Bitirdikten sonra, İlkeyi düzenle **bölmesini** kapatın. 
    
## <a name="delete-an-app-management-policy"></a>Uygulama yönetimi ilkesini silme

1. **İlkeler sayfasında** bir ilke seçin ve ardından **Sil'i seçin.**
    
2. **İlkeyi sil bölmesinde,** seçtiğiniz **ilkeyi veya** ilkeleri silmek için Onayla'yı seçin. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Aşağıdaki tablolarda, cihazlardaki iş dosyalarını korumak için kullanılabilen ayarlar ve kullanıcıların mobil cihazlarından Office dosyalarına nasıl erişeni kontrol eden ayarlar hakkında ayrıntılı bilgiler ve sağlanmaktadır.
  
 Daha fazla bilgi için [bkz. Microsoft 365 İş Ekstra'daki](map-protection-features-to-intune-settings.md)koruma özellikleri ile Intune ayarları nasıl eşler. 
  
### <a name="settings-that-protect-work-files"></a>İş dosyalarını koruyan ayarlar

Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil  <br/> |Bir cihaz burada belirttiğiniz gün sayısı boyunca kullanılmazsa, cihazda depolanan tüm iş dosyaları otomatik olarak silinir.  <br/> |
|Tüm kullanıcıları iş dosyalarını OneDrive İş üzerine kaydetmeye zorla  <br/> |Bu ayar **Açıksa,** iş dosyaları için kullanılabilen tek kaydetme konumu OneDrive İş'tir.  <br/> |
|İş dosyalarını şifrele  <br/> |İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun. Cihaz kaybolsa veya çalınsa bile kimse şirket verilerinizi okumaz.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar

Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> |Bu ayar **On** kullanıcıların mobil cihazlarında Office uygulamalarını kullanamadan önce kullanıcı adı ve parolalarının yanı sıra başka bir kimlik doğrulama biçimi de sağlamaları gerekir.<br/> |
|Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla  <br/> |Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.  <br/> |
|Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste  <br/> |Bu ayar, bir kullanıcıdan yeniden oturum açması istenmeden önce ne kadar süre boşta bırakıla olacağını belirler.  <br/> |
|Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle  <br/> |Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  <br/> |
|Kullanıcıların Office uygulamalarına kişisel uygulamalara içerik kopyalamasına izin verme  <br/> |Bu duruma varsayılan olarak izin verilir, ancak bu ayar **Açık** olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel bir dosyaya aktarabilir. Ayar **Kapalı** durumdaysa, kullanıcı iş hesabındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.  <br/> |
