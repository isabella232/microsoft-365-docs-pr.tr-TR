---
title: Cihaz durumları
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: İşletmeler için Microsoft 365'teki Yönetici evindeki Aygıt eylemleri listesindeki çeşitli aygıt durumları hakkında bilgi edinin.
ms.openlocfilehash: 1a66e76dd3a74428923292427b01551db2449e48
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627256"
---
# <a name="device-states"></a><span data-ttu-id="50c53-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="50c53-103">Device states</span></span>

<span data-ttu-id="50c53-104">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="50c53-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="50c53-106">**Durum**</span><span class="sxs-lookup"><span data-stu-id="50c53-106">**Status**</span></span>|<span data-ttu-id="50c53-107">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="50c53-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50c53-108">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="50c53-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="50c53-109">Microsoft 365 Business Premium tarafından yönetildi.</span><span class="sxs-lookup"><span data-stu-id="50c53-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="50c53-110">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="50c53-110">Retire pending</span></span>  <br/> |<span data-ttu-id="50c53-111">Microsoft 365 Business Premium, şirket verilerini aygıttan kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="50c53-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="50c53-112">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="50c53-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="50c53-113">Microsoft 365 Business Premium şu anda şirket verilerini aygıttan kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="50c53-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="50c53-114">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="50c53-114">Retire failed</span></span>  <br/> | <span data-ttu-id="50c53-115">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="50c53-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="50c53-116">Emekli iptal edildi</span><span class="sxs-lookup"><span data-stu-id="50c53-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="50c53-117">Emekli eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="50c53-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="50c53-118">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="50c53-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="50c53-119">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="50c53-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="50c53-120">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="50c53-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="50c53-121">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="50c53-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="50c53-122">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="50c53-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="50c53-123">Fabrika sıfırlama yapamadım.</span><span class="sxs-lookup"><span data-stu-id="50c53-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="50c53-124">Silme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="50c53-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="50c53-125">Fabrika silme iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="50c53-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="50c53-126">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="50c53-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="50c53-127">Bir eylem beklemede (veya devam ediyor), ancak aygıt 30+ gündür iade edilmedi.</span><span class="sxs-lookup"><span data-stu-id="50c53-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="50c53-128">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="50c53-128">Delete pending</span></span>  <br/> |<span data-ttu-id="50c53-129">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="50c53-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="50c53-130">Bulundu</span><span class="sxs-lookup"><span data-stu-id="50c53-130">Discovered</span></span>  <br/> |<span data-ttu-id="50c53-131">Microsoft 365 Business Premium cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="50c53-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
