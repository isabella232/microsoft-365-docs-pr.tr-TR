---
title: Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
ms.collection:
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
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Güvenli erişim için Office uygulamaları mobil aygıtlardan yardımcı olabilir koruma ilkeleri hakkında bilgi edinin.
ms.openlocfilehash: b77d30686b26f95de684238d1b9afd57550a7c7f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278619"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="d53cf-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="d53cf-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="d53cf-p101">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır. Android, iOS ve Windows 10 için tüm kullanıcılar için geçerli olan uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz. Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d53cf-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="d53cf-107">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="d53cf-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="d53cf-108">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="d53cf-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d53cf-109">Ayar</span><span class="sxs-lookup"><span data-stu-id="d53cf-109">Setting</span></span>  <br/> |<span data-ttu-id="d53cf-110">Açıklama</span><span class="sxs-lookup"><span data-stu-id="d53cf-110">Description</span></span>  <br/> |
|<span data-ttu-id="d53cf-111">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="d53cf-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="d53cf-112">Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d53cf-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="d53cf-113">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="d53cf-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="d53cf-114">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="d53cf-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="d53cf-115">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="d53cf-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="d53cf-116">Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması isteneceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="d53cf-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="d53cf-117">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="d53cf-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="d53cf-p102">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir. Bu, işletim sisteminin kullanıcı tarafından değiştirilebileceği ve dolayısıyla, cihazın kötü amaçlı yazılımlara karşı daha savunmasız hale gelebileceği anlamına gelir. Bu ayar **Açık** olduğunda böyle cihazlar engellenir.  </span><span class="sxs-lookup"><span data-stu-id="d53cf-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="d53cf-121">Kullanıcıların, Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver</span><span class="sxs-lookup"><span data-stu-id="d53cf-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="d53cf-p103">Bu duruma varsayılan olarak izin verilir, ancak ayar **Açık** durumda olduğunda kullanıcı bir iş dosyasındaki bilgileri kişisel dosyaya kopyalayabilir. Ayar **Kapalı** durumdaysa, kullanıcı iş dosyasındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayamaz.  </span><span class="sxs-lookup"><span data-stu-id="d53cf-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

