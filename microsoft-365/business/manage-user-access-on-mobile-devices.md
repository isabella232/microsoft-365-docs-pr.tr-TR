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
description: Kullanıcıların mobil cihazlardan uygulama ve iş dosyalarına nasıl erişeceklerini Office koruma ilkeleri hakkında bilgi edinin.
ms.openlocfilehash: 7602b712f2dfc3ba369fd76979baaaa8d5da5c5c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925289"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="b8d2d-103">Kullanıcıların mobil cihazlarda Office belgelerine nasıl erişeceğini yönetme</span><span class="sxs-lookup"><span data-stu-id="b8d2d-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="b8d2d-104">Bu makale diğer Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b8d2d-105">Kullanıcıların mobil cihazlarından Office dosyalarına erişimini denetleyen ilke ayarları varsayılan olarak **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="b8d2d-106">Android, iOS ve Windows 10 için uygulama ilkeleri oluşturmak için kurulum sırasında varsayılan değerleri kabul etmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="b8d2d-107">Kurulum tamamlandıktan sonra daha fazla ilke oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="b8d2d-108">Kullanıcıların Office dosyalarına mobil cihazlardan erişimini denetleyen ayarlar</span><span class="sxs-lookup"><span data-stu-id="b8d2d-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="b8d2d-109">Kullanıcıların Office iş dosyalarına erişimini yönetmek için şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="b8d2d-109">The following settings are available to manage how users access Office work files:</span></span>

|<span data-ttu-id="b8d2d-110">Ayar</span><span class="sxs-lookup"><span data-stu-id="b8d2d-110">Setting</span></span>  <br/> |<span data-ttu-id="b8d2d-111">Açıklama</span><span class="sxs-lookup"><span data-stu-id="b8d2d-111">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="b8d2d-112">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="b8d2d-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="b8d2d-113">Bu ayar On **ise,** kullanıcıların mobil cihazlarında Office uygulamalarını kullanamadan önce kullanıcı adı ve parolalarının yanı sıra başka bir kimlik doğrulama biçimi daha sağlamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="b8d2d-114">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="b8d2d-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="b8d2d-115">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="b8d2d-116">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="b8d2d-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="b8d2d-117">Bu ayar, bir kullanıcının ne kadar süre boşta kaldıktan sonra yeniden oturum açması istendiğinde belirler.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="b8d2d-118">Jailbreak uygulanmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle</span><span class="sxs-lookup"><span data-stu-id="b8d2d-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="b8d2d-119">Akıllı kullanıcılar, bir cihaza jailbreak uygulamış veya kök erişim izni sağlamış olabilir.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="b8d2d-120">Bu, kullanıcının işletim sistemini değiştirerek, cihazın kötü amaçlı yazılımlara karşı daha duyarlı hale geldiğini gösterir.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="b8d2d-121">Bu ayar **Açık** olduğunda böyle cihazlar engellenir.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="b8d2d-122">Kullanıcıların kişisel uygulamalara veya kişisel uygulamalara Office izin verme</span><span class="sxs-lookup"><span data-stu-id="b8d2d-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="b8d2d-123">Ayar On **olduğunda,** kullanıcı iş dosyasındaki bilgileri kişisel bir dosyaya kopyayamıyor.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="b8d2d-124">Ayar Kapalı olarak **ayarlarsanız,** kullanıcı bir iş dosyasındaki bilgileri kişisel bir uygulamaya veya kişisel hesaba kopyalayıp bu dosyayı kopya olabilir.</span><span class="sxs-lookup"><span data-stu-id="b8d2d-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

