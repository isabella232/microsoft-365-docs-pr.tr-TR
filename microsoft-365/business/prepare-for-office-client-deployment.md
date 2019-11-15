---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak nasıl yükleyip güncel tutacağınızı öğrenin.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640779"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="50e56-103">Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı</span><span class="sxs-lookup"><span data-stu-id="50e56-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="50e56-104">İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı</span><span class="sxs-lookup"><span data-stu-id="50e56-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="50e56-105">Microsoft 365 Business'ı kullanarak Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yükleyebilir ve güncelleştirmelerle güncel tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="50e56-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="50e56-106">Son kullanıcının bilgisayarı Windows 10 Business'taysa otomatik yükleme en iyi şekilde çalışır ve:</span><span class="sxs-lookup"><span data-stu-id="50e56-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="50e56-107">Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="50e56-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="50e56-108">veya</span><span class="sxs-lookup"><span data-stu-id="50e56-108">or</span></span>
    
- <span data-ttu-id="50e56-109">Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="50e56-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="50e56-110">Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin.</span><span class="sxs-lookup"><span data-stu-id="50e56-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="50e56-111">**Office Güncelleştirmeleri'ni** aşağıdaki şekilde gösterildiği gibi görürseniz, yükleme Tıkla-Çalıştır kullanılarak yapılmıştır.</span><span class="sxs-lookup"><span data-stu-id="50e56-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="50e56-113">**Bu özelliğe sahip olmaktan kimler yararlanır?**</span><span class="sxs-lookup"><span data-stu-id="50e56-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="50e56-114">Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:</span><span class="sxs-lookup"><span data-stu-id="50e56-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="50e56-115">Windows 10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update **bulunur** ve Azure Active Directory'ye katılmıştır.</span><span class="sxs-lookup"><span data-stu-id="50e56-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="50e56-116">64 bit Office uygulamaları **yok** (örnek: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="50e56-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="50e56-117">64 bit Office uygulamaları gerekiyorsa, Microsoft 365 Business yönetici konsolundan Office'in 64 bit 2016 Tıkla çalıştır sürümünü tetiklemek için destek olmadığından bu özellik uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="50e56-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="50e56-118">Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**.</span><span class="sxs-lookup"><span data-stu-id="50e56-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="50e56-119">Microsoft 365 Business, Office 2016'nın Tıkla Çalıştır sürümüne Office'i yükseltir ve bu office 2016 MSI bağımsız uygulamalarıyla çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="50e56-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="50e56-120">Aşağıdaki tablo, Microsoft 365 Business yönetici konsolundan Office dağıtımının 32 bit'lik başarılı bir Tıklamayla Çalıştır sürümüne sahip olmak için, başlangıç durumlarına bağlı olarak son kullanıcıların/yöneticilerin hangi eylemi üstlenmeleri gerekebileceğini gösterir.</span><span class="sxs-lookup"><span data-stu-id="50e56-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="50e56-121">**Başlangıçtaki Office yükleme durumu**</span><span class="sxs-lookup"><span data-stu-id="50e56-121">**Starting Office install status**</span></span>|<span data-ttu-id="50e56-122">**Microsoft 365 İş Office yüklemesinden önce yapılması gereken işlem**</span><span class="sxs-lookup"><span data-stu-id="50e56-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="50e56-123">**Son durum**</span><span class="sxs-lookup"><span data-stu-id="50e56-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="50e56-124">Hiçbir Office paketi yüklü değil</span><span class="sxs-lookup"><span data-stu-id="50e56-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="50e56-125">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="50e56-125">None</span></span>  <br/> |<span data-ttu-id="50e56-126">Office 2016 32 bit Tıkla çalıştır kullanılarak yüklenir</span><span class="sxs-lookup"><span data-stu-id="50e56-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="50e56-127">Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok</span><span class="sxs-lookup"><span data-stu-id="50e56-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="50e56-128">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="50e56-128">None</span></span>  <br/> |<span data-ttu-id="50e56-129">Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\***</span><span class="sxs-lookup"><span data-stu-id="50e56-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="50e56-130">Office'in 32 bit'lik mevcut Click-to-Run sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit bağımsız Office uygulamaları (örneğin, Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="50e56-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="50e56-131">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="50e56-131">None</span></span>  <br/> |<span data-ttu-id="50e56-132">Bağımsız uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="50e56-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="50e56-133">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="50e56-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="50e56-134">Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var</span><span class="sxs-lookup"><span data-stu-id="50e56-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="50e56-135">Hiçbiri</span><span class="sxs-lookup"><span data-stu-id="50e56-135">None</span></span>  <br/> |<span data-ttu-id="50e56-136">Bağımsız uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="50e56-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="50e56-137">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="50e56-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="50e56-138">Office'in Tıkla-Çalıştır 64 bit sürümü var</span><span class="sxs-lookup"><span data-stu-id="50e56-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="50e56-139">64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmenin sakıncası yoksa, kaldırın</span><span class="sxs-lookup"><span data-stu-id="50e56-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="50e56-140">Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir</span><span class="sxs-lookup"><span data-stu-id="50e56-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="50e56-141">Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="50e56-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="50e56-142">MSI Office 2016'yı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="50e56-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="50e56-p106">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz</span><span class="sxs-lookup"><span data-stu-id="50e56-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="50e56-145">Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="50e56-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="50e56-146">Yok</span><span class="sxs-lookup"><span data-stu-id="50e56-146">None</span></span>  <br/> |<span data-ttu-id="50e56-147">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır</span><span class="sxs-lookup"><span data-stu-id="50e56-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="50e56-148">**(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez.</span><span class="sxs-lookup"><span data-stu-id="50e56-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="50e56-149">Bir düzeltme devam ediyor.</span><span class="sxs-lookup"><span data-stu-id="50e56-149">A fix is in progress.</span></span> 
  