---
title: Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Bir uygulama yönetimi ilkesi oluşturabilir ve iş dosyalarını Windows 10 aygıtlarda korumak öğrenin.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278206"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="303ec-103">Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="303ec-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="303ec-104">Windows 10 için uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="303ec-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="303ec-105">Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="303ec-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="303ec-106">[Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=837890) genel yönetim kimlik bilgileri ile oturum açın.</span><span class="sxs-lookup"><span data-stu-id="303ec-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> <span data-ttu-id="303ec-107">Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin.</span><span class="sxs-lookup"><span data-stu-id="303ec-107">Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="303ec-108">**Aygıtlar** üzerinde sol nav, seçim \> **ilkeleri** \> **Ekle**.</span><span class="sxs-lookup"><span data-stu-id="303ec-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="303ec-109">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="303ec-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="303ec-110">**İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="303ec-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="303ec-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span><span class="sxs-lookup"><span data-stu-id="303ec-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="303ec-112">**İş dosyalarını şifrele** seçeneği otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="303ec-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="303ec-113">Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="303ec-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="303ec-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="303ec-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="303ec-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="303ec-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="303ec-116">Daha fazla bilgi için bkz: [kullanılabilir ayarları](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="303ec-116">See [Available settings](#available-settings)for more information.</span></span> 
    
    <span data-ttu-id="303ec-117">Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="303ec-117">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="303ec-118">**Windows cihazlarındaki verileri kurtar** seçeneğini genişletin; bu seçeneği **Açık** duruma getirmeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="303ec-118">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="303ec-p103">Veri Kurtarma Aracısı sertifikasının konumuna göz atabilmeniz için, önce bir sertifika oluşturmanız gerekir. Yönergeler için bkz. [Şifreleme Dosya Sistemi (EFS) Veri Kurtarma Aracısı (DRA) sertifikasını oluşturma ve doğrulama](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="303ec-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="303ec-p104">Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir. Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir. Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir. Dosyanın şifresini çözmek için yönetici, Veri Kurtarma Aracısı (DRA) sertifikası kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="303ec-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="303ec-p105">Listelenen tüm uygulamalardaki dosyaların korunduğundan emin olmak için başka etki alanları veya SharePoint Online konumları eklemek istiyorsanız, **Ek ağ ve bulut konumlarını koru** seçeneğini genişletin. Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın.</span><span class="sxs-lookup"><span data-stu-id="303ec-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="303ec-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="303ec-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="303ec-131">Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="303ec-131">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="303ec-132">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="303ec-132">Available settings</span></span>

<span data-ttu-id="303ec-133">Kullanıcıların Office iş dosyalarına erişimini yönetmek şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="303ec-133">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="303ec-134">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="303ec-134">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="303ec-135">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="303ec-135">**Setting**</span></span>|<span data-ttu-id="303ec-136">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="303ec-136">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="303ec-137">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="303ec-137">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="303ec-138">Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="303ec-138">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="303ec-139">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="303ec-139">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="303ec-140">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="303ec-140">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="303ec-141">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="303ec-141">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="303ec-142">Bu ayar, bir kullanıcının yeniden oturum açması istenmeden önce ne kadar süreliğine boşta kalabileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="303ec-142">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

