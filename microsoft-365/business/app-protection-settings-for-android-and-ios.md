---
title: Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983670"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme

## <a name="create-an-app-management-policy"></a>Uygulama yönetimi ilkesi oluşturma

1. Genel yönetici kimlik bilgileriyle [Microsoft 365 Business](https://portal.office.com)'da oturum açın. 
    
2. Yönetim merkezinde, **Cihaz ilkeleri** kartında **İlke ekle**'yi seçin.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında, oluşturmak istediğiniz ilke grubuna bağlı olarak **Android için Uygulama Yönetimi**'ni veya **iOS için Uygulama Yönetimi**'ni seçin. 
    
5. **Aygıtları kaybolur veya çalınırsa, çalışma dosyaları Koru** ve **kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek** genişletin \> nasıl istediğiniz ayarları yapılandırın. ** **Kullanıcıların Office dosyalarını mobil aygıtlarda nasıl eriştiğini yönetmek** varsayılan olarak kapalıdır** ancak **bunu açın** ve varsayılan değerleri kabul önerilir. Daha fazla bilgi için bkz: [kullanılabilir ayarları](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) . 
    
    Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Sonra karar **Bu ayarları elde kim?** Varsayılan **Tüm kullanıcıların** güvenlik grubu kullanmak istemiyorsanız, **Değiştir**' i seçin, bu ayarları alırsınız güvenlik grupları seçin \> **seçin**.
    
7. Son olarak **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="edit-an-app-management-policy"></a>Uygulama yönetimi ilkesini düzenleme

1. **İlkeleri** kartında **ilkesini Düzenle**' yi seçin.
    
2. **İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin. 
    
3. İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin. Değiştirdiğiniz değerler otomatik olarak ilkeye kaydedilir. 
    
4. İşiniz bittiğinde **İlkeyi düzenle** bölmesini kapatın. 
    
## <a name="delete-an-app-management-policy"></a>Uygulama yönetimi ilkesini silme

1. **İlkeler** kartında **İlkeyi sil**'i seçin.
    
2. **İlke Sil** bölmesinde, silmek istediğiniz ilkeleri seçin \> **seçin**ve ardından **Onayla** ilke veya seçtiğiniz ilkelerini silmek için. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Aşağıdaki tablolarda, cihazdaki iş dosyalarını koruma ve kullanıcıların Office dosyalarına mobil cihazlarından erişimini denetleyen ayarlar hakkında ayrıntılı bilgi verilmiştir.
  
 Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md) 
  
### <a name="settings-that-protect-work-files"></a>İş dosyalarını koruyan ayarlar

Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil:  <br/> |Bir cihaz, burada belirttiğiniz gün sayısı boyunca kullanılmazsa, cihazda depolanan tüm iş dosyaları otomatik olarak silinir.  <br/> |
|Tüm kullanıcıları, iş dosyalarını OneDrive İş üzerine kaydetmeye zorlama  <br/> |Bu ayar **Açık** olduğunda, iş dosyaları yalnızca OneDrive İş konumuna kaydedilebilir.  <br/> |
|İş dosyalarını şifreleme  <br/> |İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun. Cihaz kaybolsa veya çalınsa bile hiç kimse şirket verilerinizi okuyamaz.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar

Kullanıcıların Office iş dosyalarına erişimini yönetmek şu ayarlar kullanılabilir:
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> |Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.  <br/> |
|Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla  <br/> |Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.  <br/> |
|Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste  <br/> |Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.  <br/> |
|Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelleme  <br/> |Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  <br/> |
|Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver  <br/> |Bu varsayılan olarak izin veriyoruz, ancak **ayar açıksa,** kullanıcı bilgileri iş dosyasında bir kişisel dosyaya kopyalamak. Bu ayar **devre**dışıysa, kullanıcı bir kişisel app veya kişisel hesap bilgileri iş hesabından kopyalama mümkün olmayacaktır.<br/> |
   

  

