---
title: Android veya iOS cihazlarda uygulama koruma ayarlarını doğrulama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.
ms.openlocfilehash: 19a7ce48e8df5c80964a250b0bc087591a0530c1
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287885"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="5530b-103">Android veya iOS cihazlarda uygulama koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="5530b-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="5530b-104">Android veya iOS cihazlardaki uygulama koruma ayarlarını doğrulamak için sekmelerde yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="5530b-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="5530b-105">Android</span><span class="sxs-lookup"><span data-stu-id="5530b-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="5530b-106">Uygulama koruma ayarlarının kullanıcı cihazlarında çalışıp çalışmadığını denetleme</span><span class="sxs-lookup"><span data-stu-id="5530b-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="5530b-107">Uygulamaları korumak amacıyla [Android cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="5530b-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="5530b-108">Öncelikle, ilkenin doğrulama yapacağınız uygulama için geçerli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="5530b-109">Microsoft 365 Business [yönetim merkezinde](https://portal.office.com) **İlkeler** \> **İlkeyi Düzenle**'ye gidin.</span><span class="sxs-lookup"><span data-stu-id="5530b-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="5530b-110">Kurulum sırasında oluşturduğunuz ayarlarda **Android için uygulama ilkesi**'ni veya oluşturduğunuz başka bir ilkeyi seçin ve bunun uygulandığını (örneğin, Outlook'ta) doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="5530b-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="5530b-112">Office uygulamalarına erişim için PIN veya parmak izi isteme doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="5530b-113">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="5530b-115">Kullanıcının Android cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="5530b-116">Sizden de PIN girmeniz veya parmak izini kullanmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="5530b-118">Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="5530b-119">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Birkaç başarısız girişimden sonra PIN'i sıfırla** seçeneğinin herhangi bir sayıya (varsayılan olarak 5'tir) ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="5530b-120">Kullanıcının Android cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="5530b-p101">İlke tarafından belirtilen sayıda yanlış PIN girin. **PIN Girişimi Sınırına Ulaşıldı** uyarısını veren bir istem görürsünüz ve sonrasında PIN'i sıfırlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5530b-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="5530b-p102">**PIN'i Sıfırla**'ya basın. Kullanıcının Microsoft 365 İş kimlik bilgileri ile oturum açmanız ve sonrasında yeni bir PIN ayarlamanız istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="5530b-126">Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="5530b-127">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="5530b-129">Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-130">Eki olan bir e-posta açın ve ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.</span><span class="sxs-lookup"><span data-stu-id="5530b-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="5530b-132">Ekranın en altında **Cihaza kaydedilemiyor** ifadesini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="5530b-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="5530b-134">Şu anda Android için OneDrive İş'e kaydetme etkinleştirilmemiştir; dolayısıyla, yalnızca yerel olarak kaydetmenin engellendiğini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5530b-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="5530b-135">Office uygulamaları şu kadar süre boşta kalırsa kullanıcıların yeniden oturum açmasını isteme doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="5530b-136">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamaları şu kadar süre boşta kalırsa kullanıcıların yeniden oturum açmasını iste** seçeneğinin herhangi bir dakika sayısına (varsayılan olarak 30 dakikadır) ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="5530b-137">Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-p103">Şimdi Outlook gelen kutusunu görüyor olmalısınız. Android cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın ve boşta beklemesini sağlayın. Cihaz büyük olasılıkla kararacaktır.</span><span class="sxs-lookup"><span data-stu-id="5530b-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="5530b-141">Android cihazından Outlook'a yeniden erişin.</span><span class="sxs-lookup"><span data-stu-id="5530b-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="5530b-142">Outlook'a yeniden erişebilmeniz için önce PIN kodunuzu girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="5530b-143">Şifreli çalışma dosyalarını koruma doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="5530b-144">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Şifreli çalışma dosyalarını koru** seçeneğinin **Açık**, **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Kapalı** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="5530b-145">Kullanıcının Android cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-146">Birkaç resim dosyası eki olan bir e-postayı açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="5530b-147">Kaydetmek için ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.</span><span class="sxs-lookup"><span data-stu-id="5530b-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="5530b-p104">Outlook'un cihazınızdaki fotoğraflara, medyaya ve dosyalara erişmesine izin vermeniz istenebilir. **İzin Ver**'e dokunun.</span><span class="sxs-lookup"><span data-stu-id="5530b-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="5530b-151">Ekranın en altında, **Cihaza Kaydet**'i seçin ve ardından **Galeri** uygulamasını açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="5530b-p105">Listede şifrelenmiş bir fotoğraf (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) görüyor olmalısınız. Resimler listesinde, ortasında beyaz bir dairenin içinde beyaz bir ünlem işareti bulunan gri bir kare olarak gösteriliyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="5530b-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="5530b-155">Ios</span><span class="sxs-lookup"><span data-stu-id="5530b-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="5530b-156">Uygulama koruma ayarlarının kullanıcı cihazlarında çalışıp çalışmadığını denetleme</span><span class="sxs-lookup"><span data-stu-id="5530b-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="5530b-157">Uygulamaları korumak amacıyla [iOS cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="5530b-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="5530b-158">Öncelikle, ilkenin doğrulama yapacağınız uygulama için geçerli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="5530b-159">Microsoft 365 Business [yönetim merkezinde](https://portal.office.com) **İlkeler** \> **İlkeyi düzenle**'ye gidin.</span><span class="sxs-lookup"><span data-stu-id="5530b-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="5530b-160">Kurulum sırasında oluşturduğunuz ayarlarda **iOS için uygulama ilkesi**'ni veya oluşturduğunuz başka bir ilkeyi seçin ve bunun uygulandığını (örneğin, Outlook'ta) doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="5530b-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="5530b-162">Office uygulamalarına erişmek için PIN istemeyi doğrulama</span><span class="sxs-lookup"><span data-stu-id="5530b-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="5530b-163">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="5530b-165">Kullanıcının iOS cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="5530b-166">Sizden de bir PIN girmeniz veya parmak izi kullanmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="5530b-168">Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="5530b-169">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçip **Kullanıcıların mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** bölümünü genişletin ve **Birkaç başarısız girişimden sonra PIN'i sıfırla** seçeneğinin herhangi bir sayı (varsayılan olarak 5'tir) olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="5530b-170">Kullanıcının iOS cihazında Outlook'u açın ve kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="5530b-p106">İlke tarafından belirtilen sayıda yanlış PIN girin. **PIN Deneme Sınırına Ulaşıldı** uyarısını bildiren bir istem görürsünüz ve bundan sonra PIN'i sıfırlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5530b-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="5530b-p107">**Tamam**'a basın. Kullanıcının Microsoft 365 İş kimlik bilgileri ile oturum açmanız ve ardından yeni bir PIN belirlemeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="5530b-176">Kullanıcıları, tüm iş dosyalarını OneDrive İş'e kaydetmeye zorlamayı doğrulama</span><span class="sxs-lookup"><span data-stu-id="5530b-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="5530b-177">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="5530b-179">Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-180">Ek içeren bir e-postayı açın ve eki açıp ekranın altındaki **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5530b-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="5530b-p108">OneDrive İş için yalnızca bir seçenek görüyor olmanız gerekir. Görmüyorsanız **Hesap Ekle**'ye dokunup **Depolama Hesabı Ekle** ekranından **OneDrive İş**'i seçin. İstendiği zaman son kullanıcının Microsoft 365 İş bilgilerini sağlayarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="5530b-185">**Kaydet**'e tıklayıp **OneDrive İş**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5530b-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="5530b-186">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcının tekrardan oturum açmasını istemeyi doğrulama</span><span class="sxs-lookup"><span data-stu-id="5530b-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="5530b-187">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçip **Kullanıcıların mobil cihazlarda Office dosyalarına nasıl erişeceğini yönet** bölümünü genişletin ve **Office uygulamaları şu kadar süre boyunca boşta kalırsa kullanıcıların tekrardan oturum açmasını iste:** seçeneği için dakika cinsinden bir süre (varsayılan olarak 30 dakikadır) belirlendiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="5530b-188">Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-p109">Şimdi Outlook gelen kutusunu görüyor olmanız gerekir. iOS cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın. Cihaz büyük olasılıkla kararır.</span><span class="sxs-lookup"><span data-stu-id="5530b-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="5530b-192">iOS cihazından Outlook'a tekrar erişin.</span><span class="sxs-lookup"><span data-stu-id="5530b-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="5530b-193">Outlook'a yeniden erişebilmeniz için PIN kodunuzu girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="5530b-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="5530b-194">Şifreli çalışma dosyalarını koruma doğrulaması</span><span class="sxs-lookup"><span data-stu-id="5530b-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="5530b-195">**İlkeyi düzenle** bölmesinde **Kayıp veya çalınan cihazlara karşı koruma**'nın yanındaki **Düzenle**'yi seçip **Cihazlar kaybolur veya çalınırsa iş dosyalarını koru** bölümünü genişletin ve **İş dosyalarını şifreyle koru** seçeneğinin **Açık**, **Kullanıcıları, tüm iş dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin ise **Kapalı** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="5530b-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="5530b-196">Kullanıcının iOS cihazında Outlook'u açıp kullanıcının Microsoft 365 İş kimlik bilgileriyle oturum açın ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="5530b-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="5530b-197">Birkaç resim dosyası eki içeren bir e-postayı açın.</span><span class="sxs-lookup"><span data-stu-id="5530b-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="5530b-198">Eke dokunun ve sonrasında altındaki **Kaydet** seçeneğine dokunun.</span><span class="sxs-lookup"><span data-stu-id="5530b-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="5530b-p110">Giriş ekranından **Fotoğraflar** uygulamasını açın. Şifreli bir resmin (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) kaydedildiğini, ancak şifrelenmiş olduğunu görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="5530b-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

