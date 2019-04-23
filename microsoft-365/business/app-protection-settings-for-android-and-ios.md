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
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="38c18-103">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="38c18-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="38c18-104">Uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="38c18-104">Create an app management policy</span></span>

1. <span data-ttu-id="38c18-105">[Microsoft 365 iş Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=837890) genel yönetim kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="38c18-105">Sign in to [Microsoft 365 Business admin center ](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="38c18-106">Yönetim Merkezi'nde **cihaz** seçmenizi \> **ilkeleri** \> **İlkesi Ekle**.</span><span class="sxs-lookup"><span data-stu-id="38c18-106">In the admin center, choose **Devices** \> **Policies** \> **Add policy**.</span></span>
  
3. <span data-ttu-id="38c18-107">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="38c18-107">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="38c18-108">**İlke türü**'nün altında, oluşturmak istediğiniz ilke grubuna bağlı olarak **Android için Uygulama Yönetimi**'ni veya **iOS için Uygulama Yönetimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="38c18-108">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="38c18-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="38c18-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="38c18-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="38c18-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="38c18-111">Daha fazla bilgi için bkz: [kullanılabilir ayarları](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="38c18-111">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="38c18-112">Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38c18-112">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="38c18-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="38c18-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="38c18-116">Son olarak **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="38c18-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="38c18-117">Uygulama yönetimi ilkesini düzenleme</span><span class="sxs-lookup"><span data-stu-id="38c18-117">Edit an app management policy</span></span>

1. <span data-ttu-id="38c18-118">**İlkeleri** kartında **ilkesini Düzenle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="38c18-118">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="38c18-119">**İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="38c18-119">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="38c18-p103">İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin. Değiştirdiğiniz değerler otomatik olarak ilkeye kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="38c18-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="38c18-122">İşiniz bittiğinde **İlkeyi düzenle** bölmesini kapatın.</span><span class="sxs-lookup"><span data-stu-id="38c18-122">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="38c18-123">Uygulama yönetimi ilkesini silme</span><span class="sxs-lookup"><span data-stu-id="38c18-123">Delete an app management policy</span></span>

1. <span data-ttu-id="38c18-124">**İlkeler** kartında **İlkeyi sil**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="38c18-124">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="38c18-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span><span class="sxs-lookup"><span data-stu-id="38c18-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="38c18-126">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="38c18-126">Available settings</span></span>

<span data-ttu-id="38c18-127">Aşağıdaki tablolarda, cihazdaki iş dosyalarını koruma ve kullanıcıların Office dosyalarına mobil cihazlarından erişimini denetleyen ayarlar hakkında ayrıntılı bilgi verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="38c18-127">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="38c18-128">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="38c18-128">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="38c18-129">İş dosyalarını koruyan ayarlar</span><span class="sxs-lookup"><span data-stu-id="38c18-129">Settings that protect work files</span></span>

<span data-ttu-id="38c18-130">Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="38c18-130">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="38c18-131">Ayar</span><span class="sxs-lookup"><span data-stu-id="38c18-131">Setting</span></span>  <br/> |<span data-ttu-id="38c18-132">Açıklama</span><span class="sxs-lookup"><span data-stu-id="38c18-132">Description</span></span>  <br/> |
|<span data-ttu-id="38c18-133">İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil</span><span class="sxs-lookup"><span data-stu-id="38c18-133">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="38c18-134">Bir cihaz, burada belirttiğiniz gün sayısı boyunca kullanılmazsa, cihazda depolanan tüm iş dosyaları otomatik olarak silinir.</span><span class="sxs-lookup"><span data-stu-id="38c18-134">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="38c18-135">Tüm kullanıcıları iş dosyalarını OneDrive İş üzerine kaydetmeye zorla</span><span class="sxs-lookup"><span data-stu-id="38c18-135">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="38c18-136">Bu ayar **Açık** olduğunda, iş dosyaları yalnızca OneDrive İş konumuna kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="38c18-136">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="38c18-137">İş dosyalarını şifrele</span><span class="sxs-lookup"><span data-stu-id="38c18-137">Encrypt work files</span></span>  <br/> |<span data-ttu-id="38c18-p104">İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun. Cihaz kaybolsa veya çalınsa bile hiç kimse şirket verilerinizi okuyamaz.  </span><span class="sxs-lookup"><span data-stu-id="38c18-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="38c18-140">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="38c18-140">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="38c18-141">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="38c18-141">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="38c18-142">Ayar</span><span class="sxs-lookup"><span data-stu-id="38c18-142">Setting</span></span>  <br/> |<span data-ttu-id="38c18-143">Açıklama</span><span class="sxs-lookup"><span data-stu-id="38c18-143">Description</span></span>  <br/> |
|<span data-ttu-id="38c18-144">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="38c18-144">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="38c18-145">Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="38c18-145">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="38c18-146">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="38c18-146">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="38c18-147">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="38c18-147">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="38c18-148">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="38c18-148">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="38c18-149">Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="38c18-149">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="38c18-150">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="38c18-150">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="38c18-p105">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  </span><span class="sxs-lookup"><span data-stu-id="38c18-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="38c18-154">Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver</span><span class="sxs-lookup"><span data-stu-id="38c18-154">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="38c18-155">Bu duruma varsayılan olarak izin verilir, ancak bu ayar **Açık** olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel bir dosyaya aktarabilir.</span><span class="sxs-lookup"><span data-stu-id="38c18-155">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="38c18-156">Ayar **Kapalı** durumdaysa, kullanıcı iş hesabındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.</span><span class="sxs-lookup"><span data-stu-id="38c18-156">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

