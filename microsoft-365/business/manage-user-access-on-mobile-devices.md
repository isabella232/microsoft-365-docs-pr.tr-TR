---
title: Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Kullanıcıların mobil cihazlardan Office uygulamalarına ve iş dosyalarına nasıl erişeceklerini yönetmenize olanak sağlayan koruma ilkeleri hakkında bilgi edinin.
ms.openlocfilehash: a48aa241c9e70cf087da3f1701e859dae7238024
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578397"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="f3bdf-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="f3bdf-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="f3bdf-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f3bdf-105">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="f3bdf-106">Android, iOS ve Windows 10 için tüm kullanıcılara uygun uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="f3bdf-107">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="f3bdf-108">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="f3bdf-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="f3bdf-109">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="f3bdf-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="f3bdf-110">Ayar</span><span class="sxs-lookup"><span data-stu-id="f3bdf-110">Setting</span></span>  <br/> |<span data-ttu-id="f3bdf-111">Açıklama</span><span class="sxs-lookup"><span data-stu-id="f3bdf-111">Description</span></span>  <br/> |
|<span data-ttu-id="f3bdf-112">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="f3bdf-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="f3bdf-113">Bu ayar **On** ise, kullanıcıların mobil cihazlarında Office uygulamalarını kullanamadan önce kullanıcı adı ve parolalarının yanı sıra başka bir kimlik doğrulama biçimi de sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="f3bdf-114">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="f3bdf-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="f3bdf-115">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="f3bdf-116">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="f3bdf-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="f3bdf-117">Bu ayar, bir kullanıcıdan yeniden oturum açması istenmeden önce ne kadar süre boşta bırakıla olacağını belirler.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="f3bdf-118">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="f3bdf-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="f3bdf-119">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="f3bdf-120">Bu, kullanıcının işletim sistemini değiştirerek cihazın kötü amaçlı yazılımlara karşı daha duyarlı hale geldiğini gösterir.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="f3bdf-121">Bu ayar **Açık** olduğunda böyle cihazlar engellenir.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="f3bdf-122">Kullanıcıların Office uygulamalarına kişisel uygulamalara içerik kopyalamasına izin verme</span><span class="sxs-lookup"><span data-stu-id="f3bdf-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="f3bdf-123">Ayar On **olduğunda,** kullanıcı iş dosyasındaki bilgileri kişisel bir dosyaya kopyalayıp kopyalayıp alamazsanız.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="f3bdf-124">Bu ayar Kapalı **ise,** kullanıcı bir iş dosyasındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalar.</span><span class="sxs-lookup"><span data-stu-id="f3bdf-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

