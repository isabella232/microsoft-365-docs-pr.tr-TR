---
title: Cihaz durumları
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Microsoft 365 İş'in Yönetici giriş sayfasındaki Cihaz eylemleri listesinde çeşitli cihaz durumları hakkında bilgi edinebilirsiniz.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578477"
---
# <a name="device-states"></a><span data-ttu-id="1287b-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="1287b-103">Device states</span></span>

<span data-ttu-id="1287b-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="1287b-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="1287b-105">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="1287b-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="1287b-107">**Durum**</span><span class="sxs-lookup"><span data-stu-id="1287b-107">**Status**</span></span>|<span data-ttu-id="1287b-108">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="1287b-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1287b-109">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="1287b-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="1287b-110">Microsoft 365 İş Ekstra tarafından yönetilir.</span><span class="sxs-lookup"><span data-stu-id="1287b-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="1287b-111">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="1287b-111">Retire pending</span></span>  <br/> |<span data-ttu-id="1287b-112">Microsoft 365 İş Ekstra, cihazdan şirket verilerini kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="1287b-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1287b-113">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="1287b-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="1287b-114">Microsoft 365 İş Ekstra şu anda cihazdan şirket verilerini kaldır çalışıyor.</span><span class="sxs-lookup"><span data-stu-id="1287b-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="1287b-115">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="1287b-115">Retire failed</span></span>  <br/> | <span data-ttu-id="1287b-116">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="1287b-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="1287b-117">İptal edildi</span><span class="sxs-lookup"><span data-stu-id="1287b-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="1287b-118">Kaldır eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="1287b-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="1287b-119">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="1287b-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="1287b-120">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="1287b-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="1287b-121">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="1287b-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="1287b-122">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="1287b-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="1287b-123">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="1287b-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="1287b-124">Fabrika sıfırlaması yapamadım.</span><span class="sxs-lookup"><span data-stu-id="1287b-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="1287b-125">Temizleme işlemi iptal edildi</span><span class="sxs-lookup"><span data-stu-id="1287b-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="1287b-126">Fabrika temizleme işlemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="1287b-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="1287b-127">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="1287b-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="1287b-128">Bekleyen (veya devam eden) bir eylem var, ancak cihaz 30 gün boyunca iade edildi.</span><span class="sxs-lookup"><span data-stu-id="1287b-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="1287b-129">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="1287b-129">Delete pending</span></span>  <br/> |<span data-ttu-id="1287b-130">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="1287b-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="1287b-131">Bulundu</span><span class="sxs-lookup"><span data-stu-id="1287b-131">Discovered</span></span>  <br/> |<span data-ttu-id="1287b-132">Microsoft 365 İş Ekstra cihazı algıladı.</span><span class="sxs-lookup"><span data-stu-id="1287b-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
