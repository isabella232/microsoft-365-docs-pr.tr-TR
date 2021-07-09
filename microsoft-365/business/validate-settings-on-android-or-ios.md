---
title: Android veya iOS cihazlarda uygulama koruma ayarlarını doğrulama
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Android veya iOS cihazlarınıza Microsoft 365 İş Ekstra koruma ayarlarını doğrulamayı öğrenin.
ms.openlocfilehash: 43e74b548711550090021c39096b1647cee9e039
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339340"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="8f8dc-103">Android veya iOS cihazlarda uygulama koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="8f8dc-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="8f8dc-104">Android veya iOS cihazlarında uygulama koruma ayarlarını doğrulamak için aşağıdaki bölümlerde verilen yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="8f8dc-105">Android</span><span class="sxs-lookup"><span data-stu-id="8f8dc-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="8f8dc-106">Uygulama koruma ayarlarının kullanıcı cihazlarda çalış çalış çalışı kontrol edin</span><span class="sxs-lookup"><span data-stu-id="8f8dc-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="8f8dc-107">Uygulamaları korumak amacıyla [Android cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="8f8dc-108">İlk olarak, ilkenin doğrulamayı yapacak olacağınız uygulama için geçerli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="8f8dc-109">yönetim Microsoft 365 İş Ekstra , [İlkeleri](https://admin.microsoft.com)Düzenleme **ilkesi** \> **'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="8f8dc-109">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="8f8dc-110">Kurulum **sırasında oluşturduğunuz ayarlarda Android** için uygulama ilkesi'ne veya oluşturduğunuz başka bir ilkeye tıklayın ve örneğin, Android için zorunlu Outlook doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="8f8dc-112">Office uygulamalarına erişim için PIN veya parmak izi isteme doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="8f8dc-113">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Uygulamalara erişmek için PIN veya parmak izi Office'in On olarak ayar olduğundan emin olun.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="8f8dc-115">Kullanıcının Android cihazında Oturum Outlook açın ve kullanıcının kullanıcı kimlik bilgileriyle Microsoft 365 İş Ekstra açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="8f8dc-116">Ayrıca bir PIN girmeniz veya parmak izi girmeniz de istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="8f8dc-118">Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="8f8dc-119">İlkeyi düzenle **bölmesinde, Office** belgelerine erişim denetimi'nin yanındaki Düzenle'yi seçin, Kullanıcıların mobil cihazlarda **Office** dosyalarına nasıl erişeceklerini yönet'i genişletin ve Birkaç başarısız girişimden sonra **PIN'i** sıfırla'nın bir sayı olarak ayarlanmış olduğundan emin olun.  </span><span class="sxs-lookup"><span data-stu-id="8f8dc-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="8f8dc-120">Bu varsayılan olarak 5'tir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="8f8dc-121">Kullanıcının Android cihazında Oturum Outlook açın ve kullanıcının kullanıcı kimlik bilgileriyle Microsoft 365 İş Ekstra açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="8f8dc-122">İlke tarafından belirtilen sayıda yanlış PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="8f8dc-123">PIN Deneme Sınırına Ulaşıldı uyarılarını ve **PIN'i sıfırlamayı** sizen bir istem görüntüler.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="8f8dc-125">**PIN'i Sıfırla**'ya basın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-125">Press **Reset PIN**.</span></span> <span data-ttu-id="8f8dc-126">Kullanıcının kimlik bilgileriyle oturum açmanız ve ardından yeni bir PIN Microsoft 365 İş Ekstra girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="8f8dc-127">Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="8f8dc-128">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="8f8dc-130">Kullanıcının Android cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-131">Eki olan bir e-posta açın ve ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="8f8dc-133">Ekranın en **altında Cihaza** kaydedilem'i görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="8f8dc-135">Şu anda Android için OneDrive İş'e kaydetme etkinleştirilmemiştir; dolayısıyla, yalnızca yerel olarak kaydetmenin engellendiğini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="8f8dc-136">Office uygulamaları şu kadar süre boşta kalırsa kullanıcıların yeniden oturum açmasını isteme doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="8f8dc-137">İlkeyi düzenle **bölmesinde, Office** belgelerine erişim denetimi'nin yanındaki Düzenle'yi seçin, Kullanıcıların mobil cihazlarda **Office** dosyalarına nasıl erişeceklerini yönet 'i genişletin ve Office uygulamaları belirli bir süre boşta kaldıktan sonra kullanıcıların yeniden oturum açmasını gerekli hale gelecek şekilde ayarlayın.   </span><span class="sxs-lookup"><span data-stu-id="8f8dc-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="8f8dc-138">Bu, varsayılan olarak 30 dakikadır.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="8f8dc-139">Kullanıcının Android cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-p105">Şimdi Outlook gelen kutusunu görüyor olmalısınız. Android cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın ve boşta beklemesini sağlayın. Cihaz büyük olasılıkla kararacaktır.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="8f8dc-143">Android Outlook Yeniden Erişin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="8f8dc-144">E-postanıza yeniden erişmeden önce PIN'inizi Outlook istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="8f8dc-145">Şifreli çalışma dosyalarını koruma doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="8f8dc-146">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Şifreli çalışma dosyalarını koru** seçeneğinin **Açık**, **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Kapalı** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="8f8dc-147">Kullanıcının Android cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-148">Birkaç resim dosyası eki içeren bir e-postayı açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="8f8dc-149">Kaydetmek için ekin bilgilerinin yanındaki aşağı ok simgesine dokunun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="8f8dc-p106">Outlook'un cihazınızdaki fotoğraflara, medyaya ve dosyalara erişmesine izin vermeniz istenebilir. **İzin Ver**'e dokunun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="8f8dc-153">Ekranın en altında, **Cihaza Kaydet**'i seçin ve ardından **Galeri** uygulamasını açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="8f8dc-p107">Listede şifrelenmiş bir fotoğraf (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) görüyor olmalısınız. Resimler listesinde, ortasında beyaz bir dairenin içinde beyaz bir ünlem işareti bulunan gri bir kare olarak gösteriliyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="8f8dc-157">iOS</span><span class="sxs-lookup"><span data-stu-id="8f8dc-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="8f8dc-158">Uygulama koruma ayarlarının kullanıcı cihazlarında çalışıp çalışmadığını denetleme</span><span class="sxs-lookup"><span data-stu-id="8f8dc-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="8f8dc-159">Uygulamaları korumak amacıyla [iOS cihazları için uygulama yapılandırmalarını ayarlayın](app-protection-settings-for-android-and-ios.md) ve seçtiğiniz ayarların çalıştığını doğrulamak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="8f8dc-160">İlk olarak, ilkenin doğrulamayı yapacak olacağınız uygulama için geçerli olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="8f8dc-161">yönetim Microsoft 365 İş Ekstra , [İlkeleri](https://admin.microsoft.com)Düzenleme **ilkesi** \> **'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="8f8dc-161">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="8f8dc-162">Kurulum **sırasında oluşturduğunuz ayarlarda iOS** için uygulama ilkesi'ne veya oluşturduğunuz başka bir ilkeye tıklayın ve örneğin, bu ilkenin Outlook doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="8f8dc-164">Office uygulamalarına erişmek için PIN istemeyi doğrulama</span><span class="sxs-lookup"><span data-stu-id="8f8dc-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="8f8dc-165">**İlkeyi düzenle** bölmesinde **Office belgelerine erişim denetimi**'nin yanındaki **Düzenle**'yi seçin, **Kullanıcıların mobil cihazlardan Office dosyalarına erişimini yönet**'i genişletin ve **Office uygulamalarına erişim için PIN veya parmak izi iste** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Uygulamalara erişmek için PIN veya parmak izi Office'in On olarak ayar olduğundan emin olun.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="8f8dc-167">Kullanıcının iOS cihazında Oturum Outlook açın ve kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="8f8dc-168">Ayrıca bir PIN girmeniz veya parmak izi girmeniz de istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="8f8dc-170">Birkaç başarısız girişimden sonra PIN sıfırlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="8f8dc-171">İlkeyi düzenle **bölmesinde, Office** belgelerine erişim denetimi'nin yanındaki Düzenle'yi seçin, Kullanıcıların mobil cihazlarda **Office** dosyalarına nasıl erişeceklerini yönet'i genişletin ve Birkaç başarısız girişimden sonra **PIN'i** sıfırla'nın bir sayı olarak ayarlanmış olduğundan emin olun.  </span><span class="sxs-lookup"><span data-stu-id="8f8dc-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="8f8dc-172">Bu varsayılan olarak 5'tir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="8f8dc-173">Kullanıcının iOS cihazında Oturum Outlook açın ve kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="8f8dc-174">İlke tarafından belirtilen sayıda yanlış PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="8f8dc-175">PIN Deneme Sınırına Ulaşıldı uyarılarını ve **PIN'i sıfırlamayı** sizen bir istem görüntüler.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="8f8dc-177">**Tamam**'a basın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-177">Press **OK**.</span></span> <span data-ttu-id="8f8dc-178">Kullanıcının kimlik bilgileriyle oturum açmanız ve ardından yeni bir PIN Microsoft 365 İş Ekstra girmeniz istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="8f8dc-179">Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorlama doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="8f8dc-180">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Açık** olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="8f8dc-182">Kullanıcının iOS cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-183">Ek içeren bir e-postayı açın ve eki açıp ekranın altındaki **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="8f8dc-185">OneDrive İş için yalnızca bir seçenek görüyor olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="8f8dc-186">Hesap Ekle'ye **dokunun ve** hesap **OneDrive İş'den** Hesap **Ekle Depolama** seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="8f8dc-187">İstendiğinde, son Microsoft 365 İş Ekstra oturum açma bilgilerini sağlama.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="8f8dc-188">**Kaydet**'e tıklayıp **OneDrive İş**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="8f8dc-189">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcının tekrardan oturum açmasını istemeyi doğrulama</span><span class="sxs-lookup"><span data-stu-id="8f8dc-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="8f8dc-190">İlkeyi düzenle **bölmesinde, Office** belgelerine erişim denetimi'nin yanındaki Düzenle'yi seçin, Kullanıcıların mobil cihazlarda **Office** dosyalarına nasıl erişeceklerini yönet 'i genişletin ve Office uygulamaları belirli bir süre boşta kaldıktan sonra kullanıcıların yeniden oturum açmasını gerekli hale gelecek şekilde ayarlayın.   </span><span class="sxs-lookup"><span data-stu-id="8f8dc-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="8f8dc-191">Bu, varsayılan olarak 30 dakikadır.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="8f8dc-192">Kullanıcının iOS cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-p113">Şimdi Outlook gelen kutusunu görüyor olmanız gerekir. iOS cihazına en az 30 dakika (veya ilkede belirttiğinizden daha uzun bir süre) boyunca dokunmayın. Cihaz büyük olasılıkla kararır.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="8f8dc-196">iOS Outlook Access e-postanıza yeniden erişin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="8f8dc-197">E-postanıza yeniden erişmeden önce PIN'inizi Outlook istenir.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="8f8dc-198">Şifreli çalışma dosyalarını koruma doğrulaması</span><span class="sxs-lookup"><span data-stu-id="8f8dc-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="8f8dc-199">**İlkeyi düzenle** bölmesinde **Kaybolmuş veya çalınmış cihaz koruması**'nın yanındaki **Düzenle**'yi seçin, **Cihaz kaybolursa veya çalınırsa çalışma dosyalarını koru**'yu genişletin ve **Şifreli çalışma dosyalarını koru** seçeneğinin **Açık**, **Kullanıcıları, tüm çalışma dosyalarını OneDrive İş'e kaydetmeye zorla** seçeneğinin **Kapalı** olarak ayarlandığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="8f8dc-200">Kullanıcının iOS cihazında, Outlook'i açın, kullanıcının kimlik bilgileriyle Microsoft 365 İş Ekstra ve istenirse PIN girin.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="8f8dc-201">Birkaç resim dosyası eki içeren bir e-postayı açın.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="8f8dc-202">Eke dokunun ve sonrasında altındaki **Kaydet** seçeneğine dokunun.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="8f8dc-p114">Giriş ekranından **Fotoğraflar** uygulamasını açın. Şifreli bir resmin (birden çok resim dosyası eki kaydettiyseniz daha fazla olabilir) kaydedildiğini, ancak şifrelenmiş olduğunu görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="8f8dc-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

