---
title: Microsoft 365 İş tarafından Office istemci dağıtımına hazırlanma
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yükleme ve bunları güncelleştirme hakkında bilgi edinin.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580064"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="9104c-103">Microsoft 365 İş tarafından Office istemci dağıtımına hazırlanma</span><span class="sxs-lookup"><span data-stu-id="9104c-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="9104c-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9104c-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="9104c-105">İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı</span><span class="sxs-lookup"><span data-stu-id="9104c-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="9104c-106">Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yüklemek ve güncelleştirmelerle güncel tutmak için Microsoft 365 İş Ekstra'ya kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9104c-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="9104c-107">Otomatik yükleme en iyi şekilde çalışır; son kullanıcının bilgisayarı Windows 10 İş'tedir ve:</span><span class="sxs-lookup"><span data-stu-id="9104c-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="9104c-108">Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="9104c-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="9104c-109">veya</span><span class="sxs-lookup"><span data-stu-id="9104c-109">or</span></span>
    
- <span data-ttu-id="9104c-110">Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="9104c-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="9104c-111">Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin.</span><span class="sxs-lookup"><span data-stu-id="9104c-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="9104c-112">Aşağıdaki şekilde **gösterildiği gibi Office** Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="9104c-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="9104c-114">**Bu özelliden yararlananlar**</span><span class="sxs-lookup"><span data-stu-id="9104c-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="9104c-115">Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:</span><span class="sxs-lookup"><span data-stu-id="9104c-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="9104c-116">**Windows**  10 Business kullanıcı lisansına, etkin bir iş için Microsoft 365 lisansına, Windows 10 Creators Update'e sahiptir ve Azure Active Directory'ye katılmış durumdadır.</span><span class="sxs-lookup"><span data-stu-id="9104c-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="9104c-117">**64** bit Office uygulamaları (örneğin: Word, Excel, PowerPoint) yok.</span><span class="sxs-lookup"><span data-stu-id="9104c-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="9104c-118">64 bit Office uygulamaları gerekli ise bu özellik uygun değildir, çünkü işletmeler için Microsoft 365 yönetici konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği yoktur.</span><span class="sxs-lookup"><span data-stu-id="9104c-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="9104c-119">Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**.</span><span class="sxs-lookup"><span data-stu-id="9104c-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="9104c-120">Microsoft 365 İş, Office'i Office 2016'nın Tıkla-Çalıştır sürümüne yükselter ve bu da Office 2016 MSI tek başına uygulamalarıyla işe yaramadı.</span><span class="sxs-lookup"><span data-stu-id="9104c-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="9104c-121">Aşağıdaki tablo, iş için Microsoft 365 yönetici konsolundan Office'in 32 bit Tıkla-Çalıştır sürümünün başarılı bir şekilde dağıtımını yapmak için, son kullanıcıların/yöneticilerin başlangıç durumlarına bağlı olarak hangi eylemi uygulaması gerekten olduğunu gösterir.</span><span class="sxs-lookup"><span data-stu-id="9104c-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="9104c-122">**Başlangıçtaki Office yükleme durumu**</span><span class="sxs-lookup"><span data-stu-id="9104c-122">**Starting Office install status**</span></span>|<span data-ttu-id="9104c-123">**Microsoft 365 İş Office yüklemesi öncesinde 2010'da 2010'da 2013'e kadar devam etmek için gereken işlem**</span><span class="sxs-lookup"><span data-stu-id="9104c-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="9104c-124">**Son durum**</span><span class="sxs-lookup"><span data-stu-id="9104c-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9104c-125">Hiçbir Office paketi yüklü değil</span><span class="sxs-lookup"><span data-stu-id="9104c-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="9104c-126">Yok</span><span class="sxs-lookup"><span data-stu-id="9104c-126">None</span></span>  <br/> |<span data-ttu-id="9104c-127">Office 2016 32 bit, Tıkla-Çalıştır kullanılarak yüklenir</span><span class="sxs-lookup"><span data-stu-id="9104c-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="9104c-128">Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok</span><span class="sxs-lookup"><span data-stu-id="9104c-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="9104c-129">Yok</span><span class="sxs-lookup"><span data-stu-id="9104c-129">None</span></span>  <br/> |<span data-ttu-id="9104c-130">Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\***</span><span class="sxs-lookup"><span data-stu-id="9104c-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="9104c-131">Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit tek başına Office uygulamaları (örneğin, Visio, Project) var</span><span class="sxs-lookup"><span data-stu-id="9104c-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="9104c-132">Yok</span><span class="sxs-lookup"><span data-stu-id="9104c-132">None</span></span>  <br/> |<span data-ttu-id="9104c-133">Tek başına uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9104c-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="9104c-134">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="9104c-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="9104c-135">Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var</span><span class="sxs-lookup"><span data-stu-id="9104c-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="9104c-136">Yok</span><span class="sxs-lookup"><span data-stu-id="9104c-136">None</span></span>  <br/> |<span data-ttu-id="9104c-137">Tek başına uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9104c-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="9104c-138">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="9104c-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="9104c-139">Office'in Tıkla-Çalıştır 64 bit sürümü var</span><span class="sxs-lookup"><span data-stu-id="9104c-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="9104c-140">64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmeniz sorun yoksa kaldırın</span><span class="sxs-lookup"><span data-stu-id="9104c-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="9104c-141">Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir</span><span class="sxs-lookup"><span data-stu-id="9104c-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="9104c-142">Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="9104c-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="9104c-143">MSI Office 2016'yı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="9104c-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="9104c-p106">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz</span><span class="sxs-lookup"><span data-stu-id="9104c-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="9104c-146">Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="9104c-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="9104c-147">Yok</span><span class="sxs-lookup"><span data-stu-id="9104c-147">None</span></span>  <br/> |<span data-ttu-id="9104c-148">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır</span><span class="sxs-lookup"><span data-stu-id="9104c-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="9104c-149">**(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez.</span><span class="sxs-lookup"><span data-stu-id="9104c-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="9104c-150">Bir düzeltme devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="9104c-150">A fix is in progress.</span></span> 
  
