---
title: Cihaz durumları
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: 365 işletmede aygıt durumları hakkında bilgi edinin.
ms.openlocfilehash: 15114835a5014f5bfac600eac79bcdffdaec481a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277001"
---
# <a name="device-states"></a><span data-ttu-id="7b894-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="7b894-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="7b894-104">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="7b894-104">Device states</span></span>

<span data-ttu-id="7b894-105">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="7b894-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="7b894-107">**Durum**</span><span class="sxs-lookup"><span data-stu-id="7b894-107">**Status**</span></span>|<span data-ttu-id="7b894-108">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="7b894-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7b894-109">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="7b894-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="7b894-110">Microsoft 365 İş tarafından yönetilir.</span><span class="sxs-lookup"><span data-stu-id="7b894-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="7b894-111">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="7b894-111">Retire pending</span></span>  <br/> |<span data-ttu-id="7b894-112">Microsoft 365 İş, cihazdan şirket verilerini kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="7b894-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7b894-113">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="7b894-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="7b894-114">Microsoft 365 İş şu anda cihazdan şirket verilerini kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="7b894-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7b894-115">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="7b894-115">Retire failed</span></span>  <br/> | <span data-ttu-id="7b894-116">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="7b894-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="7b894-117">Kullanımdan kaldırma işlemi iptal edildi</span><span class="sxs-lookup"><span data-stu-id="7b894-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="7b894-118">Kullanımdan kaldırma eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="7b894-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="7b894-119">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="7b894-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="7b894-120">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="7b894-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="7b894-121">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="7b894-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="7b894-122">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="7b894-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="7b894-123">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="7b894-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="7b894-124">Fabrika sıfırlaması yapılamadı.</span><span class="sxs-lookup"><span data-stu-id="7b894-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="7b894-125">Temizleme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="7b894-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="7b894-126">Fabrika temizleme işlemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="7b894-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="7b894-127">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="7b894-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="7b894-128">Bu, bir eylemin beklemede olduğu (veya sürdüğü) ama cihazın 30+ gün boyunca iade edilmediği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="7b894-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="7b894-129">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="7b894-129">Delete pending</span></span>  <br/> |<span data-ttu-id="7b894-130">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="7b894-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="7b894-131">Bulundu</span><span class="sxs-lookup"><span data-stu-id="7b894-131">Discovered</span></span>  <br/> |<span data-ttu-id="7b894-132">Microsoft 365 İş cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="7b894-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
