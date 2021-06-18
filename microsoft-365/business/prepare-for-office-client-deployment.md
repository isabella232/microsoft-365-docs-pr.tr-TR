---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
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
description: Windows 10 bilgisayarlarına 32 bit Office uygulamalarını otomatik olarak yükleme ve bunları güncelleştirme hakkında bilgi edinin.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924237"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="4a656-103">Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı</span><span class="sxs-lookup"><span data-stu-id="4a656-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="4a656-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="4a656-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="4a656-105">İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı</span><span class="sxs-lookup"><span data-stu-id="4a656-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="4a656-106">32 bit Office uygulamalarını Windows 10 bilgisayarlara otomatik olarak yüklemek ve güncelleştirmelerle güncel tutmak için Microsoft 365 İş Ekstra'ya kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4a656-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="4a656-107">Otomatik yükleme en iyi şekilde, son kullanıcının bilgisayarı Windows 10 Business'da ise ve:</span><span class="sxs-lookup"><span data-stu-id="4a656-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="4a656-108">Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="4a656-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="4a656-109">veya</span><span class="sxs-lookup"><span data-stu-id="4a656-109">or</span></span>
    
- <span data-ttu-id="4a656-110">Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4a656-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="4a656-111">Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin.</span><span class="sxs-lookup"><span data-stu-id="4a656-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="4a656-112">Aşağıdaki şekilde **gösterildiği gibi Office** Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="4a656-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="4a656-114">**Bu özele sahip olmak kimlerin avantajlarına sahip olacak?**</span><span class="sxs-lookup"><span data-stu-id="4a656-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="4a656-115">Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:</span><span class="sxs-lookup"><span data-stu-id="4a656-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="4a656-116">**Windows**  10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update vardır ve Azure Active Directory'ye katılmış durumdadır.</span><span class="sxs-lookup"><span data-stu-id="4a656-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="4a656-117">**64** bit Office uygulamaları (örneğin: Word, Excel, PowerPoint) yok.</span><span class="sxs-lookup"><span data-stu-id="4a656-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="4a656-118">64 bit Office uygulamaları gerekli ise, bu özellik uygun değildir çünkü microsoft 365 İş yönetici konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği yoktur.</span><span class="sxs-lookup"><span data-stu-id="4a656-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="4a656-119">Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**.</span><span class="sxs-lookup"><span data-stu-id="4a656-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="4a656-120">Microsoft 365 İş, Office'i Office 2016'nın Tıkla-Çalıştır sürümüne yükselter ve bu da Office 2016 MSI tek başına uygulamalarıyla işe yaramadı.</span><span class="sxs-lookup"><span data-stu-id="4a656-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="4a656-121">Aşağıdaki tabloda, son kullanıcıların/yöneticilerin, başlangıç durumlarına bağlı olarak, işletmeler için Microsoft 365 yönetici konsolundan Office'in 32 bit Tıkla-Çalıştır sürümünün dağıtımını başarılı bir şekilde yapmak için hangi eylemi uygulaması gerekten olduğu görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="4a656-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span><br/>


|<span data-ttu-id="4a656-122">Başlangıçtaki Office yükleme durumu</span><span class="sxs-lookup"><span data-stu-id="4a656-122">Starting Office install status</span></span>|<span data-ttu-id="4a656-123">Microsoft 365 İş Office'i yüklemeden önce at gereken eylem</span><span class="sxs-lookup"><span data-stu-id="4a656-123">Action to take before Microsoft 365 for business Office install</span></span>|<span data-ttu-id="4a656-124">Son durum</span><span class="sxs-lookup"><span data-stu-id="4a656-124">End state</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a656-125">Hiçbir Office paketi yüklü değil</span><span class="sxs-lookup"><span data-stu-id="4a656-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="4a656-126">Yok</span><span class="sxs-lookup"><span data-stu-id="4a656-126">None</span></span>  <br/> |<span data-ttu-id="4a656-127">Tıkla-Çalıştır kullanılarak Office 2016 32 bit yüklenir</span><span class="sxs-lookup"><span data-stu-id="4a656-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="4a656-128">Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok</span><span class="sxs-lookup"><span data-stu-id="4a656-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="4a656-129">Yok</span><span class="sxs-lookup"><span data-stu-id="4a656-129">None</span></span>  <br/> |<span data-ttu-id="4a656-130">Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\***</span><span class="sxs-lookup"><span data-stu-id="4a656-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="4a656-131">Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit tek başına Office uygulamaları (örneğin, Visio, Project) var</span><span class="sxs-lookup"><span data-stu-id="4a656-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="4a656-132">Yok</span><span class="sxs-lookup"><span data-stu-id="4a656-132">None</span></span>  <br/> |<span data-ttu-id="4a656-133">Tek başına uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="4a656-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="4a656-134">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="4a656-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="4a656-135">Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var</span><span class="sxs-lookup"><span data-stu-id="4a656-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="4a656-136">Yok</span><span class="sxs-lookup"><span data-stu-id="4a656-136">None</span></span>  <br/> |<span data-ttu-id="4a656-137">Tek başına uygulamalar etkilenmez.</span><span class="sxs-lookup"><span data-stu-id="4a656-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="4a656-138">Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="4a656-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="4a656-139">Office'in Tıkla-Çalıştır 64 bit sürümü var</span><span class="sxs-lookup"><span data-stu-id="4a656-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="4a656-140">64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmek sorun yoksa bunları kaldırın</span><span class="sxs-lookup"><span data-stu-id="4a656-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="4a656-141">Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir</span><span class="sxs-lookup"><span data-stu-id="4a656-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="4a656-142">Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="4a656-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="4a656-143">MSI Office 2016'yı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="4a656-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="4a656-p106">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz</span><span class="sxs-lookup"><span data-stu-id="4a656-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="4a656-146">Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="4a656-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="4a656-147">Yok</span><span class="sxs-lookup"><span data-stu-id="4a656-147">None</span></span>  <br/> |<span data-ttu-id="4a656-148">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır</span><span class="sxs-lookup"><span data-stu-id="4a656-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="4a656-149">**(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez.</span><span class="sxs-lookup"><span data-stu-id="4a656-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="4a656-150">Düzeltme için çalışma devam etmektedir.</span><span class="sxs-lookup"><span data-stu-id="4a656-150">A fix is in progress.</span></span> 
  
