---
title: Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme
f1.keywords:
- NOCSH
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
ms.openlocfilehash: 0adb103ac3bef72e340c1f5daf54a6b8a184d85c
ms.sourcegitcommit: fce0d5cad32ea60a08ff001b228223284710e2ed
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42894290"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="7899a-103">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="7899a-103">Set app protection settings for Android or iOS devices</span></span>

![Banner bu https://aka.ms/aboutM365previewişaret .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="7899a-105">Uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="7899a-105">Create an app management policy</span></span>

1. <span data-ttu-id="7899a-106">'deki <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine gidin.</span><span class="sxs-lookup"><span data-stu-id="7899a-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="7899a-107">Sol gezinmede, \> **Aygıtİlkeleri** \> **Ekle'yi**seçin. **Devices**</span><span class="sxs-lookup"><span data-stu-id="7899a-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="7899a-108">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="7899a-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="7899a-109">**Politika türüne**göre, oluşturmak istediğiniz politika kümesine bağlı **olarak, iOS için**Android veya Uygulama Yönetimi için **Uygulama Yönetimi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="7899a-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="7899a-110">**Aygıtlar kaybolduğunda veya çalındığında iş dosyalarını koru'nun** genişletilmesi ve **kullanıcıların mobil cihazlardaki Office dosyalarına nasıl erişmelerini yönetin.**</span><span class="sxs-lookup"><span data-stu-id="7899a-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="7899a-111">Ayarları istediğiniz gibi yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="7899a-111">Configure the settings how you would like.</span></span> <span data-ttu-id="7899a-112">**Kullanıcıların mobil cihazlardaki Office dosyalarına nasıl erişeceklerini yönetin** varsayılan olarak **Kapalıdır,** ancak **açmanızı** ve varsayılan değerleri kabul etmeyi öneririz.</span><span class="sxs-lookup"><span data-stu-id="7899a-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="7899a-113">Daha fazla bilgi için [Kullanılabilir ayarlara](#available-settings)bakın.</span><span class="sxs-lookup"><span data-stu-id="7899a-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="7899a-114">Varsayılan ayarlara geri dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** seçeneğini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7899a-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="7899a-116">Next decide **Who will get these settings?**</span><span class="sxs-lookup"><span data-stu-id="7899a-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="7899a-117">Varsayılan **Tüm Kullanıcılar** güvenlik grubunu kullanmak istemiyorsanız, **Değiştir'i**seçin, bu ayarları \> alan güvenlik gruplarını seçin **Seçin.**</span><span class="sxs-lookup"><span data-stu-id="7899a-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="7899a-118">Son olarak, **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="7899a-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="7899a-119">Uygulama yönetimi ilkesini düzenleme</span><span class="sxs-lookup"><span data-stu-id="7899a-119">Edit an app management policy</span></span>

1. <span data-ttu-id="7899a-120">**İlkeler** kartında, **politikayı edit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="7899a-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="7899a-121">**İlkeyi düzenle** bölmesinde değiştirmek istediğiniz ilkeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="7899a-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="7899a-122">İlkedeki değerleri değiştirmek için her ayarın yanında bulunan **Düzenle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7899a-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="7899a-123">Bir değeri değiştirdiğinizde, bu değer otomatik olarak ilke kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="7899a-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="7899a-124">İşiniz bittiğinde, **Edit ilkesi** bölmesini kapatın.</span><span class="sxs-lookup"><span data-stu-id="7899a-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="7899a-125">Uygulama yönetimi ilkesini silme</span><span class="sxs-lookup"><span data-stu-id="7899a-125">Delete an app management policy</span></span>

1. <span data-ttu-id="7899a-126">**İlkeler** sayfasında bir ilke seçin ve sonra **silin.**</span><span class="sxs-lookup"><span data-stu-id="7899a-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="7899a-127">Sil **ilkesi** bölmesinde, seçtiğiniz ilke veya ilkeleri silmek için **Onayla'yı** seçin.</span><span class="sxs-lookup"><span data-stu-id="7899a-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="7899a-128">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="7899a-128">Available settings</span></span>

<span data-ttu-id="7899a-129">Aşağıdaki tablolar, aygıtlarda çalışma dosyalarını korumak için kullanılabilen ayarlar ve kullanıcıların Mobil aygıtlarından Office dosyalarına nasıl erişeceklerini kontrol eden ayarlar hakkında ayrıntılı bilgi verir.</span><span class="sxs-lookup"><span data-stu-id="7899a-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="7899a-130">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="7899a-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="7899a-131">İş dosyalarını koruyan ayarlar</span><span class="sxs-lookup"><span data-stu-id="7899a-131">Settings that protect work files</span></span>

<span data-ttu-id="7899a-132">Bir kullanıcının cihazı kaybolursa veya çalınırsa, iş dosyalarını korumak için aşağıdaki ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="7899a-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="7899a-133">Ayar</span><span class="sxs-lookup"><span data-stu-id="7899a-133">Setting</span></span>  <br/> |<span data-ttu-id="7899a-134">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7899a-134">Description</span></span>  <br/> |
|<span data-ttu-id="7899a-135">İş dosyalarını şu kadar gün sonra etkin olmayan cihazdan sil</span><span class="sxs-lookup"><span data-stu-id="7899a-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="7899a-136">Burada belirttiğiniz gün sayısı için bir aygıt kullanılmazsa, aygıtta depolanan çalışma dosyaları otomatik olarak silinir.</span><span class="sxs-lookup"><span data-stu-id="7899a-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="7899a-137">Tüm kullanıcıları iş dosyalarını OneDrive İş üzerine kaydetmeye zorla</span><span class="sxs-lookup"><span data-stu-id="7899a-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="7899a-138">Bu ayar **Açık**ise, iş dosyaları için kullanılabilir tek kaydetme konumu İş için OneDrive'dır.</span><span class="sxs-lookup"><span data-stu-id="7899a-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="7899a-139">İş dosyalarını şifrele</span><span class="sxs-lookup"><span data-stu-id="7899a-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="7899a-140">İş dosyalarınızın şifreleme ile korunması için bu ayarı **Açık** tutun.</span><span class="sxs-lookup"><span data-stu-id="7899a-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="7899a-141">Cihaz kaybolsa veya çalınmış olsa bile, şirket verilerinizi kimse okuyamaz.</span><span class="sxs-lookup"><span data-stu-id="7899a-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="7899a-142">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="7899a-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="7899a-143">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="7899a-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="7899a-144">Ayar</span><span class="sxs-lookup"><span data-stu-id="7899a-144">Setting</span></span>  <br/> |<span data-ttu-id="7899a-145">Açıklama</span><span class="sxs-lookup"><span data-stu-id="7899a-145">Description</span></span>  <br/> |
|<span data-ttu-id="7899a-146">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="7899a-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="7899a-147">Bu ayar **On** Açık'sa, kullanıcıların mobil cihazlarında Office uygulamalarını kullanabilmeleri için kullanıcı adlarına ve parolalarına ek olarak başka bir kimlik doğrulama biçimi sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="7899a-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="7899a-148">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="7899a-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="7899a-149">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="7899a-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="7899a-150">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="7899a-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="7899a-151">Bu ayar, kullanıcıdan yeniden oturum açması istenmeden önce ne kadar süre yle boşta kalınabileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="7899a-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="7899a-152">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="7899a-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="7899a-p105">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  </span><span class="sxs-lookup"><span data-stu-id="7899a-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="7899a-156">Kullanıcıların Office uygulamalarından gelen içeriği kişisel uygulamalara kopyalamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="7899a-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="7899a-157">Bu duruma varsayılan olarak izin verilir, ancak bu ayar **Açık** olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel bir dosyaya aktarabilir.</span><span class="sxs-lookup"><span data-stu-id="7899a-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="7899a-158">Ayar **Kapalı** durumdaysa, kullanıcı iş hesabındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.</span><span class="sxs-lookup"><span data-stu-id="7899a-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
