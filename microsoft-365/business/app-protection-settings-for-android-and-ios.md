---
title: Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Android veya iOS cihazlardaki çalışma dosyalarını nasıl oluşturup, düzenlemeyi veya silmeyi ve çalışma dosyalarını nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: a829cfbcb3209313a53e0a1406f5252d3d5580d8
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574748"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="1866c-103">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="1866c-103">Set app protection settings for Android or iOS devices</span></span>

![Banner bu https://aka.ms/aboutM365previewişaret .](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="1866c-105">Uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="1866c-105">Create an app management policy</span></span>

1. <span data-ttu-id="1866c-106">'deki <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine gidin.</span><span class="sxs-lookup"><span data-stu-id="1866c-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="1866c-107">Sol gezinmede, \> **Aygıtİlkeleri** \> **Ekle'yi**seçin. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="1866c-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="1866c-108">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="1866c-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="1866c-109">**İlke türü**'nün altında, oluşturmak istediğiniz ilke grubuna bağlı olarak **Android için Uygulama Yönetimi**'ni veya **iOS için Uygulama Yönetimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="1866c-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="1866c-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="1866c-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="1866c-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="1866c-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="1866c-112">Daha fazla bilgi için [kullanılabilir ayarlara](#available-settings) bakın.</span><span class="sxs-lookup"><span data-stu-id="1866c-112">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="1866c-113">Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1866c-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="1866c-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="1866c-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="1866c-117">Son olarak **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="1866c-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="1866c-118">Uygulama yönetimi ilkesini düzenleme</span><span class="sxs-lookup"><span data-stu-id="1866c-118">Edit an app management policy</span></span>

1. <span data-ttu-id="1866c-119">**İlkeler** kartında, **politikayı edit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="1866c-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="1866c-120">**İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="1866c-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="1866c-p103">İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin. Değiştirdiğiniz değerler otomatik olarak ilkeye kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="1866c-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="1866c-123">İşiniz bittiğinde **İlkeyi düzenle** bölmesini kapatın.</span><span class="sxs-lookup"><span data-stu-id="1866c-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="1866c-124">Uygulama yönetimi ilkesini silme</span><span class="sxs-lookup"><span data-stu-id="1866c-124">Delete an app management policy</span></span>

1. <span data-ttu-id="1866c-125">**İlkeler** sayfasında bir ilke seçin ve sonra **silin.**</span><span class="sxs-lookup"><span data-stu-id="1866c-125">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="1866c-126">Silme **ilkesi** bölmesinde seçtiğiniz ilke veya ilkeleri silmek için **Onayla'yı** seçin.</span><span class="sxs-lookup"><span data-stu-id="1866c-126">On the **Delete policy** pane choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="1866c-127">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="1866c-127">Available settings</span></span>

<span data-ttu-id="1866c-128">Aşağıdaki tablolarda, cihazdaki iş dosyalarını koruma ve kullanıcıların Office dosyalarına mobil cihazlarından erişimini denetleyen ayarlar hakkında ayrıntılı bilgi verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="1866c-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="1866c-129">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="1866c-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="1866c-130">İş dosyalarını koruyan ayarlar</span><span class="sxs-lookup"><span data-stu-id="1866c-130">Settings that protect work files</span></span>

<span data-ttu-id="1866c-131">Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="1866c-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="1866c-132">Ayar</span><span class="sxs-lookup"><span data-stu-id="1866c-132">Setting</span></span>  <br/> |<span data-ttu-id="1866c-133">Açıklama</span><span class="sxs-lookup"><span data-stu-id="1866c-133">Description</span></span>  <br/> |
|<span data-ttu-id="1866c-134">İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil</span><span class="sxs-lookup"><span data-stu-id="1866c-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="1866c-135">Bir cihaz, burada belirttiğiniz gün sayısı boyunca kullanılmazsa, cihazda depolanan tüm iş dosyaları otomatik olarak silinir.</span><span class="sxs-lookup"><span data-stu-id="1866c-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="1866c-136">Tüm kullanıcıları iş dosyalarını OneDrive İş üzerine kaydetmeye zorla</span><span class="sxs-lookup"><span data-stu-id="1866c-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="1866c-137">Bu ayar **Açık** olduğunda, iş dosyaları yalnızca OneDrive İş konumuna kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="1866c-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="1866c-138">İş dosyalarını şifrele</span><span class="sxs-lookup"><span data-stu-id="1866c-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="1866c-p104">İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun. Cihaz kaybolsa veya çalınsa bile hiç kimse şirket verilerinizi okuyamaz.  </span><span class="sxs-lookup"><span data-stu-id="1866c-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="1866c-141">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="1866c-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="1866c-142">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="1866c-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="1866c-143">Ayar</span><span class="sxs-lookup"><span data-stu-id="1866c-143">Setting</span></span>  <br/> |<span data-ttu-id="1866c-144">Açıklama</span><span class="sxs-lookup"><span data-stu-id="1866c-144">Description</span></span>  <br/> |
|<span data-ttu-id="1866c-145">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="1866c-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="1866c-146">Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="1866c-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="1866c-147">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="1866c-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="1866c-148">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="1866c-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="1866c-149">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="1866c-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="1866c-150">Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="1866c-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="1866c-151">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="1866c-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="1866c-p105">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  </span><span class="sxs-lookup"><span data-stu-id="1866c-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="1866c-155">Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver</span><span class="sxs-lookup"><span data-stu-id="1866c-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="1866c-156">Bu duruma varsayılan olarak izin verilir, ancak bu ayar **Açık** olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel bir dosyaya aktarabilir.</span><span class="sxs-lookup"><span data-stu-id="1866c-156">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="1866c-157">Ayar **Kapalı** durumdaysa, kullanıcı iş hesabındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.</span><span class="sxs-lookup"><span data-stu-id="1866c-157">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

