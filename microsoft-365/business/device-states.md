---
title: Cihaz durumları
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: 365 işletmede aygıt durumları hakkında bilgi edinin.
ms.openlocfilehash: bd6f1ad7f7671d9616fd14d477dfcfb164ff6bd0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982910"
---
# <a name="device-states"></a><span data-ttu-id="e427f-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="e427f-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="e427f-104">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="e427f-104">Device states</span></span>

<span data-ttu-id="e427f-105">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="e427f-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="e427f-107">**Durum**</span><span class="sxs-lookup"><span data-stu-id="e427f-107">**Status**</span></span>|<span data-ttu-id="e427f-108">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="e427f-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e427f-109">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="e427f-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="e427f-110">Microsoft 365 İş tarafından yönetilir.</span><span class="sxs-lookup"><span data-stu-id="e427f-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="e427f-111">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="e427f-111">Retire pending</span></span>  <br/> |<span data-ttu-id="e427f-112">Microsoft 365 İş, cihazdan şirket verilerini kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="e427f-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e427f-113">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="e427f-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="e427f-114">Microsoft 365 İş şu anda cihazdan şirket verilerini kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="e427f-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e427f-115">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="e427f-115">Retire failed</span></span>  <br/> | <span data-ttu-id="e427f-116">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="e427f-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="e427f-117">Kullanımdan kaldırma işlemi iptal edildi</span><span class="sxs-lookup"><span data-stu-id="e427f-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="e427f-118">Kullanımdan kaldırma eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="e427f-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="e427f-119">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="e427f-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="e427f-120">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="e427f-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="e427f-121">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="e427f-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="e427f-122">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="e427f-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="e427f-123">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="e427f-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="e427f-124">Fabrika sıfırlaması yapılamadı.</span><span class="sxs-lookup"><span data-stu-id="e427f-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="e427f-125">Temizleme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="e427f-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="e427f-126">Fabrika temizleme işlemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="e427f-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="e427f-127">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="e427f-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="e427f-128">Bu, bir eylemin beklemede olduğu (veya sürdüğü) ama cihazın 30+ gün boyunca iade edilmediği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="e427f-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="e427f-129">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="e427f-129">Delete pending</span></span>  <br/> |<span data-ttu-id="e427f-130">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="e427f-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="e427f-131">Bulundu</span><span class="sxs-lookup"><span data-stu-id="e427f-131">Discovered</span></span>  <br/> |<span data-ttu-id="e427f-132">Microsoft 365 İş cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="e427f-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
