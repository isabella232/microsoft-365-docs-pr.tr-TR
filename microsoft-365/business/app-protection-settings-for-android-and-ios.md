---
title: Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Oluşturmak, düzenlemek veya bir uygulama yönetimi ilkesini silin ve Android veya IOS cihazlarda çalışma dosyaları korumak öğrenin.
ms.openlocfilehash: e81ff8a4bd71dbbbf7ccc31249d450e03f4bd241
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277471"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme

## <a name="create-an-app-management-policy"></a>Uygulama yönetimi ilkesi oluşturma

1. [Microsoft 365 iş Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=837890) genel yönetim kimlik bilgileriyle oturum açın. 
    
2. Yönetim Merkezi'nde **cihaz** seçmenizi \> **ilkeleri** \> **İlkesi Ekle**.
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında, oluşturmak istediğiniz ilke grubuna bağlı olarak **Android için Uygulama Yönetimi**'ni veya **iOS için Uygulama Yönetimi**'ni seçin. 
    
5. Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. Daha fazla bilgi için bkz: [kullanılabilir ayarları](#available-settings) . 
    
    Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
7. Son olarak **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="edit-an-app-management-policy"></a>Uygulama yönetimi ilkesini düzenleme

1. **İlkeleri** kartında **ilkesini Düzenle**' yi seçin.
    
2. **İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin. 
    
3. İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin. Değiştirdiğiniz değerler otomatik olarak ilkeye kaydedilir. 
    
4. İşiniz bittiğinde **İlkeyi düzenle** bölmesini kapatın. 
    
## <a name="delete-an-app-management-policy"></a>Uygulama yönetimi ilkesini silme

1. **İlkeler** kartında **İlkeyi sil**'i seçin.
    
2. On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Aşağıdaki tablolarda, cihazdaki iş dosyalarını koruma ve kullanıcıların Office dosyalarına mobil cihazlarından erişimini denetleyen ayarlar hakkında ayrıntılı bilgi verilmiştir.
  
 Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md) 
  
### <a name="settings-that-protect-work-files"></a>İş dosyalarını koruyan ayarlar

Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil  <br/> |Bir cihaz, burada belirttiğiniz gün sayısı boyunca kullanılmazsa, cihazda depolanan tüm iş dosyaları otomatik olarak silinir.  <br/> |
|Tüm kullanıcıları iş dosyalarını OneDrive İş üzerine kaydetmeye zorla  <br/> |Bu ayar **Açık** olduğunda, iş dosyaları yalnızca OneDrive İş konumuna kaydedilebilir.  <br/> |
|İş dosyalarını şifrele  <br/> |İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun. Cihaz kaybolsa veya çalınsa bile hiç kimse şirket verilerinizi okuyamaz.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar

Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> |Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.  <br/> |
|Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla  <br/> |Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.  <br/> |
|Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste  <br/> |Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.  <br/> |
|Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle  <br/> |Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  <br/> |
|Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver  <br/> |Bu duruma varsayılan olarak izin verilir, ancak bu ayar **Açık** olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel bir dosyaya aktarabilir. Ayar **Kapalı** durumdaysa, kullanıcı iş hesabındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.  <br/> |
   

  

