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
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471077"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="d1078-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="d1078-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="d1078-104">Bu makale Microsoft 365 Business Premium için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="d1078-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="d1078-105">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="d1078-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="d1078-106">Tüm kullanıcılar için geçerli olan Android, iOS ve Windows 10 için uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="d1078-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="d1078-107">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1078-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="d1078-108">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="d1078-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="d1078-109">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="d1078-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d1078-110">Ayar</span><span class="sxs-lookup"><span data-stu-id="d1078-110">Setting</span></span>  <br/> |<span data-ttu-id="d1078-111">Açıklama</span><span class="sxs-lookup"><span data-stu-id="d1078-111">Description</span></span>  <br/> |
|<span data-ttu-id="d1078-112">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="d1078-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="d1078-113">Bu ayar **On**Açık'taysa, kullanıcıların mobil aygıtlarında Office uygulamalarını kullanabilmeleri için kullanıcı adlarına ve parolalarına ek olarak başka bir kimlik doğrulama biçimi sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="d1078-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="d1078-114">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="d1078-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="d1078-115">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="d1078-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="d1078-116">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="d1078-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="d1078-117">Bu ayar, kullanıcıdan yeniden oturum açması istenmeden önce ne kadar süre yle boşta kalınabileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="d1078-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="d1078-118">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="d1078-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="d1078-119">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir.</span><span class="sxs-lookup"><span data-stu-id="d1078-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="d1078-120">Bu, kullanıcının işletim sistemini değiştirebileceği ve bu da aygıtı kötü amaçlı yazılımlara karşı daha duyarlı hale getirebileceği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="d1078-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="d1078-121">Bu ayar **Açık** olduğunda böyle cihazlar engellenir.</span><span class="sxs-lookup"><span data-stu-id="d1078-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="d1078-122">Kullanıcıların Office uygulamalarından gelen içeriği kişisel uygulamalara kopyalamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="d1078-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="d1078-123">Ayar **Ayarı Ayarı**olduğunda, kullanıcı iş dosyasındaki bilgileri kişisel bir dosyaya kopyalayamaz.</span><span class="sxs-lookup"><span data-stu-id="d1078-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="d1078-124">Ayar **Kapalıysa,** kullanıcı bilgileri bir iş dosyasından kişisel bir uygulamaya veya kişisel hesaba kopyalayabilir.</span><span class="sxs-lookup"><span data-stu-id="d1078-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

