---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Otomatik olarak bilgisayarlara Windows 10 32 bit Office uygulamaları yükleyin ve güncel kalmasını nasıl öğrenin.
ms.openlocfilehash: 16a8230d60157f1c6731ac639d89533b05aa3afe
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982160"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="61e5d-103">Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı</span><span class="sxs-lookup"><span data-stu-id="61e5d-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="61e5d-104">İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı</span><span class="sxs-lookup"><span data-stu-id="61e5d-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="61e5d-105">Microsoft 365 İş kullanarak Windows 10 bilgisayarlarına 32 bit Office uygulamalarını otomatik olarak yükleyebilir ve güncelleştirmelerle bunların güncelliğini koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="61e5d-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="61e5d-106">Bundan en iyi sonucu elde etmek için kullanıcının bilgisayarı Windows 10 Business çalıştırılıyor olmalı ve şu koşulları sağlamalıdır:</span><span class="sxs-lookup"><span data-stu-id="61e5d-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="61e5d-107">Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.</span><span class="sxs-lookup"><span data-stu-id="61e5d-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="61e5d-108">veya</span><span class="sxs-lookup"><span data-stu-id="61e5d-108">or</span></span>
    
- <span data-ttu-id="61e5d-109">Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="61e5d-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="61e5d-p101">Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin. Aşağıdaki şekilde gösterildiği gibi Office Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılmıştır.</span><span class="sxs-lookup"><span data-stu-id="61e5d-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="61e5d-113">**Bu özelliğe sahip olmak kimlerin işine yarar**</span><span class="sxs-lookup"><span data-stu-id="61e5d-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="61e5d-114">Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:</span><span class="sxs-lookup"><span data-stu-id="61e5d-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="61e5d-115">Windows 10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update **bulunur** ve Azure Active Directory'ye katılmıştır.</span><span class="sxs-lookup"><span data-stu-id="61e5d-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="61e5d-p102">64 bit Office paketi **yoktur** (örneğin: Word, Excel, Powerpoint). 64 bit Office uygulamaları gerekiyorsa, bu özellik uygun değildir. Microsoft 365 İş yönetim konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği sağlanmaz.</span><span class="sxs-lookup"><span data-stu-id="61e5d-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="61e5d-p103">Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**. Microsoft 365 İş, Office'i Office 2016 Tıkla-Çalıştır sürümüne yükseltir ve bu da Office 2016 MSI tek başına uygulamalarıyla çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="61e5d-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="61e5d-120">Aşağıdaki tabloda, son kullanıcıların/yöneticilerin, işleme başladıkları noktaya bağlı olarak Microsoft 365 İş yönetim merkezinden Office'in 32 bit Tıkla-Çalıştır sürümünün dağıtımını başarıyla tamamlaması için gerçekleştirmesi gereken işlemlerin ayrıntılarını bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="61e5d-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="61e5d-121">**Başlangıçtaki Office yükleme durumu**</span><span class="sxs-lookup"><span data-stu-id="61e5d-121">**Starting Office install status**</span></span>|<span data-ttu-id="61e5d-122">**Microsoft 365 İş Office yüklemesinden önce yapılması gereken işlem**</span><span class="sxs-lookup"><span data-stu-id="61e5d-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="61e5d-123">**Son durum**</span><span class="sxs-lookup"><span data-stu-id="61e5d-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="61e5d-124">Hiçbir Office paketi yüklü değil</span><span class="sxs-lookup"><span data-stu-id="61e5d-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="61e5d-125">Yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-125">None</span></span>  <br/> |<span data-ttu-id="61e5d-126">Tıkla-çalıştır kullanılarak Office 2016 32 bit yüklenir</span><span class="sxs-lookup"><span data-stu-id="61e5d-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="61e5d-127">Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="61e5d-128">Yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-128">None</span></span>  <br/> |<span data-ttu-id="61e5d-129">Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\***</span><span class="sxs-lookup"><span data-stu-id="61e5d-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="61e5d-130">Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 veya 64 bit tek başına Office uygulamaları (örneğin, Visio ve Project) var</span><span class="sxs-lookup"><span data-stu-id="61e5d-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="61e5d-131">Yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-131">None</span></span>  <br/> |<span data-ttu-id="61e5d-p104">Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="61e5d-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="61e5d-134">Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var</span><span class="sxs-lookup"><span data-stu-id="61e5d-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="61e5d-135">Yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-135">None</span></span>  <br/> |<span data-ttu-id="61e5d-p105">Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir</span><span class="sxs-lookup"><span data-stu-id="61e5d-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="61e5d-138">Office'in Tıkla-Çalıştır 64 bit sürümü var</span><span class="sxs-lookup"><span data-stu-id="61e5d-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="61e5d-139">64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmek sorun yaratmayacaksa, 64 bit uygulamalarını kaldırın</span><span class="sxs-lookup"><span data-stu-id="61e5d-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="61e5d-140">Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir</span><span class="sxs-lookup"><span data-stu-id="61e5d-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="61e5d-141">Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="61e5d-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="61e5d-142">MSI Office 2016'yı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="61e5d-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="61e5d-p106">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz</span><span class="sxs-lookup"><span data-stu-id="61e5d-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="61e5d-145">Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var</span><span class="sxs-lookup"><span data-stu-id="61e5d-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="61e5d-146">Yok</span><span class="sxs-lookup"><span data-stu-id="61e5d-146">None</span></span>  <br/> |<span data-ttu-id="61e5d-147">Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır</span><span class="sxs-lookup"><span data-stu-id="61e5d-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="61e5d-p107">**(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez. Düzeltme için çalışmalar devam etmektedir.</span><span class="sxs-lookup"><span data-stu-id="61e5d-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


