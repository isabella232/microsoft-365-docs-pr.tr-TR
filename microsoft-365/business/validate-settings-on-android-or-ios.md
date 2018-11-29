---
title: Android veya IOS cihazlarda uygulama koruması ayarlarını doğrula
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 300f59e81a93cc3dfc03fd1d98891be1ac4f7795
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983680"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Android veya IOS cihazlarda uygulama koruması ayarlarını doğrula

Android veya IOS cihazlarda uygulama koruması ayarlarını doğrulamak için sekmeleri'ndaki yönergeleri izleyin.
  
## <a name="androidtab"></a>[Android](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Uygulama koruma ayarlarının kullanıcı cihazlarında çalışıp çalışmadığını denetleme

Uygulamaları korumak amacıyla [Android cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin. 
  
Öncelikle, ilkenin doğrulama yapacağınız uygulama için geçerli olduğundan emin olun.
  
1. Microsoft 365 Business [yönetim merkezinde](https://portal.office.com) **İlkeler** \> **İlkeyi Düzenle**'ye gidin.
    
2. Kurulum sırasında oluşturduğunuz ayarlarda **Android için uygulama ilkesi**'ni veya oluşturduğunuz başka bir ilkeyi seçin ve bunun uygulandığını (örneğin, Outlook'ta) doğrulayın. 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>Office uygulamalarına erişim için PIN veya parmak izi isteme doğrulaması

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Kullanıcının Android cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.
    
2. Sizden de PIN girmeniz veya parmak izini kullanmanız istenir.
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Birkaç başarısız girişimden sonra PIN'i sıfırla** seçeneğinin herhangi bir sayıya (varsayılan olarak 5'tir) ayarlandığından emin olun. 
  
1. Kullanıcının Android cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.
    
2. İlke tarafından belirtilen sayıda yanlış PIN girin. **PIN Girişimi Sınırına Ulaşıldı** uyarısını veren bir istem görürsünüz ve sonrasında PIN'i sıfırlayabilirsiniz. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. **PIN'i Sıfırla**'ya basın. Kullanıcının Microsoft 365 İş kimlik bilgileri ile oturum açmanız ve sonrasında yeni bir PIN ayarlamanız istenir.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorlama doğrulaması

**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Eki olan bir e-posta açın ve ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    Ekranın en altında **Cihaza kaydedilemiyor** ifadesini görürsünüz. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > Şu anda Android için OneDrive İş'e kaydetme etkinleştirilmemiştir; dolayısıyla, yalnızca yerel olarak kaydetmenin engellendiğini görebilirsiniz. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Office uygulamaları şu kadar süre boşta kalırsa kullanıcıların yeniden oturum açmasını isteme doğrulaması

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamaları şu kadar süre boşta kalırsa kullanıcıların yeniden oturum açmasını iste** seçeneğinin herhangi bir dakika sayısına (varsayılan olarak 30 dakikadır) ayarlandığından emin olun. 
  
1. Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Şimdi Outlook gelen kutusunu görüyor olmalısınız. Android cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın ve boşta beklemesini sağlayın. Cihaz büyük olasılıkla kararacaktır.
    
3. Android cihazından Outlook'a yeniden erişin.
    
4. Outlook'a yeniden erişebilmeniz için önce PIN kodunuzu girmeniz istenir.
    
### <a name="validate-protect-work-files-with-encryption"></a>Şifreli çalışma dosyalarını koruma doğrulaması

**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Şifreli çalışma dosyalarını koru** seçeneğinin **Açık**, **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Kapalı** olarak ayarlandığından emin olun.
  
1. Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Birkaç resim dosyası eki olan bir e-postayı açın.
    
3. Kaydetmek için ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Outlook'un cihazınızdaki fotoğraflara, medyaya ve dosyalara erişmesine izin vermeniz istenebilir. **İzin Ver**'e dokunun.
    
5. Ekranın en altında, **Cihaza Kaydet**'i seçin ve ardından **Galeri** uygulamasını açın. 
    
6. Listede şifrelenmiş bir fotoğraf (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) görüyor olmalısınız. Resimler listesinde, ortasında beyaz bir dairenin içinde beyaz bir ünlem işareti bulunan gri bir kare olarak gösteriliyor olabilir.
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[IOS](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Uygulama koruma ayarlarının kullanıcı cihazlarında çalışıp çalışmadığını denetleme

Uygulamaları korumak amacıyla [iOS cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin. 
  
Öncelikle, ilkenin doğrulama yapacağınız uygulama için geçerli olduğundan emin olun.
  
1. Microsoft 365 Business [yönetim merkezinde](https://portal.office.com) **İlkeler** \> **İlkeyi düzenle**'ye gidin.
    
2. Kurulum sırasında oluşturduğunuz ayarlarda **iOS için uygulama ilkesi**'ni veya oluşturduğunuz başka bir ilkeyi seçin ve bunun uygulandığını (örneğin, Outlook'ta) doğrulayın. 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>Office uygulamalarına erişmek için PIN istemeyi doğrulama

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçip **Kullanıcıların mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** bölümünü genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Kullanıcının iOS cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.
    
2. Sizden de bir PIN girmeniz veya parmak izi kullanmanız istenir.
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçip **Kullanıcıların mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** bölümünü genişletin ve **Birkaç başarısız girişimden sonra PIN'i sıfırla** seçeneğinin herhangi bir sayı (varsayılan olarak 5'tir) olarak ayarlandığından emin olun. 
  
1. Kullanıcının iOS cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.
    
2. İlke tarafından belirtilen sayıda yanlış PIN girin. **PIN Deneme Sınırına Ulaşıldı** uyarısını bildiren bir istem görürsünüz ve bundan sonra PIN'i sıfırlayabilirsiniz. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. **Tamam**'a basın. Kullanıcının Microsoft 365 İş kimlik bilgileri ile oturum açmanız ve ardından yeni bir PIN belirlemeniz istenir.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorlama doğrulaması

**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Ek içeren bir e-postayı açın ve eki açıp ekranın altındaki **Kaydet**'i seçin. 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. OneDrive İş için yalnızca bir seçenek görüyor olmanız gerekir. Görmüyorsanız **Hesap Ekle**'ye dokunup **Depolama Hesabı Ekle** ekranından **OneDrive İş**'i seçin. İstendiği zaman son kullanıcının Microsoft 365 İş bilgilerini sağlayarak oturum açın. 
    
    **Kaydet**'e tıklayıp **OneDrive İş**'i seçin.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcının tekrardan oturum açmasını istemeyi doğrulama

**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçip **Kullanıcıların mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** bölümünü genişletin ve **Office uygulamaları şu kadar süre boyunca boşta kalırsa kullanıcıların tekrardan oturum açmasını iste:** seçeneği için dakika cinsinden bir süre (varsayılan olarak 30 dakikadır) belirlendiğinden emin olun. 
  
1. Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Şimdi Outlook gelen kutusunu görüyor olmanız gerekir. iOS cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın. Cihaz büyük olasılıkla kararır.
    
3. iOS cihazından Outlook'a tekrar erişin.
    
4. Outlook'a yeniden erişebilmeniz için PIN kodunuzu girmeniz istenir.
    
### <a name="validate-protect-work-files-with-encryption"></a>Şifreli çalışma dosyalarını koruma doğrulaması

**İlkeyi düzenle** bölmesinde **Kayıp veya çalınan cihazlara karşı koruma**'nın yanındaki **Düzenle**'yi seçip **Cihazlar kaybolur veya çalınırsa iş dosyalarını koru** bölümünü genişletin ve **İş dosyalarını şifreyle koru** seçeneğinin **Açık**, **Kullanıcıları, tüm iş dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin ise **Kapalı** olarak ayarlandığından emin olun.
  
1. Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.
    
2. Birkaç resim dosyası eki içeren bir e-postayı açın.
    
3. Eke dokunun ve sonrasında altındaki **Kaydet** seçeneğine dokunun. 
    
4. Giriş ekranından **Fotoğraflar** uygulamasını açın. Şifreli bir resmin (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) kaydedildiğini, ancak şifrelenmiş olduğunu görürsünüz. 
    
---

