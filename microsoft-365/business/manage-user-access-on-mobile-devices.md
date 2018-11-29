---
title: Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Güvenli erişim için Office uygulamaları mobil aygıtlardan yardımcı olabilir koruma ilkeleri hakkında bilgi edinin.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983190"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="d7e84-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="d7e84-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="d7e84-p101">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır. Android, iOS ve Windows 10 için tüm kullanıcılar için geçerli olan uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz. Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d7e84-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="d7e84-107">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="d7e84-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="d7e84-108">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="d7e84-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d7e84-109">Ayar</span><span class="sxs-lookup"><span data-stu-id="d7e84-109">Setting</span></span>  <br/> |<span data-ttu-id="d7e84-110">Açıklama</span><span class="sxs-lookup"><span data-stu-id="d7e84-110">Description</span></span>  <br/> |
|<span data-ttu-id="d7e84-111">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="d7e84-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="d7e84-112">Bu ayar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d7e84-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="d7e84-113">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="d7e84-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="d7e84-114">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için, belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="d7e84-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="d7e84-115">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="d7e84-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="d7e84-116">Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="d7e84-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="d7e84-117">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="d7e84-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="d7e84-p102">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  </span><span class="sxs-lookup"><span data-stu-id="d7e84-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="d7e84-121">Kullanıcıların, Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver</span><span class="sxs-lookup"><span data-stu-id="d7e84-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="d7e84-p103">Bu duruma varsayılan olarak izin verilir, ancak ayar **Açık** durumda olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel dosyaya kopyalayabilir. Ayar **Kapalı** durumdaysa, kullanıcı iş dosyasındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.  </span><span class="sxs-lookup"><span data-stu-id="d7e84-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

