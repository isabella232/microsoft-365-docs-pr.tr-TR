---
title: Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Kullanıcıların Office uygulamalarına ve mobil cihazlardan dosyaları nasıl çalıştırdığını yönetmenize olanak tanıyan koruma ilkeleri hakkında bilgi edinin.
ms.openlocfilehash: f613e518c3607010cae55443456be9d3ddc3d689
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403088"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="24400-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="24400-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="24400-104">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="24400-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="24400-105">Tüm kullanıcılar için geçerli olan Android, iOS ve Windows 10 için uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="24400-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="24400-106">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="24400-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="24400-107">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="24400-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="24400-108">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="24400-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="24400-109">Ayar</span><span class="sxs-lookup"><span data-stu-id="24400-109">Setting</span></span>  <br/> |<span data-ttu-id="24400-110">Açıklama</span><span class="sxs-lookup"><span data-stu-id="24400-110">Description</span></span>  <br/> |
|<span data-ttu-id="24400-111">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="24400-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="24400-112">Bu ayar **On**Açık'taysa, kullanıcıların mobil aygıtlarında Office uygulamalarını kullanabilmeleri için kullanıcı adlarına ve parolalarına ek olarak başka bir kimlik doğrulama biçimi sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="24400-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="24400-113">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="24400-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="24400-114">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="24400-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="24400-115">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="24400-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="24400-116">Bu ayar, kullanıcıdan yeniden oturum açması istenmeden önce ne kadar süre yle boşta kalınabileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="24400-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="24400-117">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="24400-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="24400-118">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir.</span><span class="sxs-lookup"><span data-stu-id="24400-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="24400-119">Bu, kullanıcının işletim sistemini değiştirebileceği ve bu da aygıtı kötü amaçlı yazılımlara karşı daha duyarlı hale getirebileceği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="24400-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="24400-120">Bu ayar **Açık** olduğunda böyle cihazlar engellenir.</span><span class="sxs-lookup"><span data-stu-id="24400-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="24400-121">Kullanıcıların Office uygulamalarından gelen içeriği kişisel uygulamalara kopyalamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="24400-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="24400-122">Ayar **Ayarı Ayarı**olduğunda, kullanıcı iş dosyasındaki bilgileri kişisel bir dosyaya kopyalayamaz.</span><span class="sxs-lookup"><span data-stu-id="24400-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="24400-123">Ayar **Kapalıysa,** kullanıcı bilgileri bir iş dosyasından kişisel bir uygulamaya veya kişisel hesaba kopyalayabilir.</span><span class="sxs-lookup"><span data-stu-id="24400-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

