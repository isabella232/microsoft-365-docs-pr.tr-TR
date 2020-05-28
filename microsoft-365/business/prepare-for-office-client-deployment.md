---
title: Microsoft 365 tarafından iş için Office istemci dağıtımına hazırlanın
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak nasıl yükleyip güncel tutacağınızı öğrenin.
ms.openlocfilehash: 6f3a80be9729a3818607c0f42e2cc7ece66a07ee
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401332"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="9e938-103">Microsoft 365 tarafından iş için Office istemci dağıtımına hazırlanın</span><span class="sxs-lookup"><span data-stu-id="9e938-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="9e938-104">İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı</span><span class="sxs-lookup"><span data-stu-id="9e938-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="9e938-105">Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yüklemek ve güncelleştirmelerle güncel tutmak için iş için Microsoft 365'i kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9e938-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="9e938-106">Son kullanıcının bilgisayarı Windows 10 Business'taysa otomatik yükleme en iyi şekilde çalışır ve:</span><span class="sxs-lookup"><span data-stu-id="9e938-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="9e938-107">Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="9e938-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="9e938-108">veya</span><span class="sxs-lookup"><span data-stu-id="9e938-108">or</span></span>
    
- <span data-ttu-id="9e938-109">Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="9e938-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="9e938-110">Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin.</span><span class="sxs-lookup"><span data-stu-id="9e938-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="9e938-111">**Office Güncelleştirmeleri'ni** aşağıdaki şekilde gösterildiği gibi görürseniz, yükleme Tıkla-Çalıştır kullanılarak yapılmıştır.</span><span class="sxs-lookup"><span data-stu-id="9e938-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="9e938-113">**Bu özelliğe sahip olmaktan kimler yararlanır?**</span><span class="sxs-lookup"><span data-stu-id="9e938-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="9e938-114">Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:</span><span class="sxs-lookup"><span data-stu-id="9e938-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="9e938-115">Windows 10 Business kullanıcı lisansına, işletme lisansı için etkin bir Microsoft 365'e, Windows 10 Creators Update'e **sahiptir** ve Azure Active Directory'ye katılır.</span><span class="sxs-lookup"><span data-stu-id="9e938-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="9e938-116">64 bit Office uygulamaları **yok** (örnek: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="9e938-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="9e938-117">64 bit Office uygulamaları gerekiyorsa, iş yöneticisi konsolu için Microsoft 365'ten Office'in 64 bit 2016 Tıkla çalıştır sürümünü tetiklemek için destek olmadığından bu özellik uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="9e938-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="9e938-118">Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**.</span><span class="sxs-lookup"><span data-stu-id="9e938-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="9e938-119">İş için Microsoft 365, Office'i Office 2016'nın Tıkla Çalıştır sürümüne yükseltir ve bu office 2016 MSI bağımsız uygulamalarıyla çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="9e938-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="9e938-120">Aşağıdaki tablo, iş yöneticisi konsolu için Microsoft 365'ten Office dağıtımının başarılı bir 32 bit Click-to-Run sürümüne sahip olmak için, başlangıç durumlarına bağlı olarak son kullanıcıların/yöneticilerin hangi eylemi üstlenmeleri gerekebileceğini gösterir.</span><span class="sxs-lookup"><span data-stu-id="9e938-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="9e938-121">**Başlangıçtaki Office yükleme durumu**</span><span class="sxs-lookup"><span data-stu-id="9e938-121">**Starting Office install status**</span></span>|<span data-ttu-id="9e938-122">**İş Office yüklemesi için Microsoft 365'ten önce yapılacak işlem**</span><span class="sxs-lookup"><span data-stu-id="9e938-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="9e938-123">**Son durum**</span><span class="sxs-lookup"><span data-stu-id="9e938-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9e938-124">Hiçbir Office paketi yüklü değil</span><span class="sxs-lookup"><span data-stu-id="9e938-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="9e938-125">Yok</span><span class="sxs-lookup"><span data-stu-id="9e938-125">None</span></span>  <br/> |<span data-ttu-id="9e938-126">Office 2016 32 bit Tıkla çalıştır kullanılarak yüklenir</span><span class="sxs-lookup"><span data-stu-id="9e938-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="9e938-127">Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok</span><span class="sxs-lookup"><span data-stu-id="9e938-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="9e938-128">Yok</span><span class="sxs-lookup"><span data-stu-id="9e938-128">None</span></span>  <br/> |<span data-ttu-id="9e938-129">Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\***</span><span class="sxs-lookup"><span data-stu-id="9e938-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="9e938-130">Office'in 32 bit'lik mevcut Click-to-Run sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit bağımsız Office uygulamaları (örneğin, Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="9e938-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="9e938-131">Yok</span><span class="sxs-lookup"><span data-stu-id="9e938-131">None</span></span>  <br/> |<span data-ttu-id="9e938-132">Bağımsız uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9e938-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="9e938-133">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="9e938-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="9e938-134">Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var</span><span class="sxs-lookup"><span data-stu-id="9e938-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="9e938-135">Yok</span><span class="sxs-lookup"><span data-stu-id="9e938-135">None</span></span>  <br/> |<span data-ttu-id="9e938-136">Bağımsız uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="9e938-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="9e938-137">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="9e938-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="9e938-138">Office'in Tıkla-Çalıştır 64 bit sürümü var</span><span class="sxs-lookup"><span data-stu-id="9e938-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="9e938-139">64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmenin sakıncası yoksa, kaldırın</span><span class="sxs-lookup"><span data-stu-id="9e938-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="9e938-140">Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir</span><span class="sxs-lookup"><span data-stu-id="9e938-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="9e938-141">Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="9e938-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="9e938-142">MSI Office 2016'yı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="9e938-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="9e938-p106">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz</span><span class="sxs-lookup"><span data-stu-id="9e938-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="9e938-145">Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="9e938-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="9e938-146">Yok</span><span class="sxs-lookup"><span data-stu-id="9e938-146">None</span></span>  <br/> |<span data-ttu-id="9e938-147">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır</span><span class="sxs-lookup"><span data-stu-id="9e938-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="9e938-148">**(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez.</span><span class="sxs-lookup"><span data-stu-id="9e938-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="9e938-149">Bir düzeltme devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="9e938-149">A fix is in progress.</span></span> 
  
