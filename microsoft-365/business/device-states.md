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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Microsoft 365 Business'taki Yönetici evindeki Aygıt eylemleri listesindeki çeşitli aygıt durumları hakkında bilgi edinin.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415675"
---
# <a name="device-states"></a><span data-ttu-id="fab32-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="fab32-103">Device states</span></span>

<span data-ttu-id="fab32-104">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="fab32-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="fab32-106">**Durum**</span><span class="sxs-lookup"><span data-stu-id="fab32-106">**Status**</span></span>|<span data-ttu-id="fab32-107">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="fab32-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fab32-108">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="fab32-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="fab32-109">Microsoft 365 İş tarafından yönetilir.</span><span class="sxs-lookup"><span data-stu-id="fab32-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="fab32-110">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="fab32-110">Retire pending</span></span>  <br/> |<span data-ttu-id="fab32-111">Microsoft 365 İş, cihazdan şirket verilerini kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="fab32-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fab32-112">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="fab32-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="fab32-113">Microsoft 365 İş şu anda cihazdan şirket verilerini kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="fab32-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fab32-114">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="fab32-114">Retire failed</span></span>  <br/> | <span data-ttu-id="fab32-115">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="fab32-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="fab32-116">Emekli iptal edildi</span><span class="sxs-lookup"><span data-stu-id="fab32-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="fab32-117">Emekli eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="fab32-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="fab32-118">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="fab32-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="fab32-119">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="fab32-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="fab32-120">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="fab32-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="fab32-121">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="fab32-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="fab32-122">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="fab32-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="fab32-123">Fabrika sıfırlama yapamadım.</span><span class="sxs-lookup"><span data-stu-id="fab32-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="fab32-124">Silme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="fab32-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="fab32-125">Fabrika silme iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="fab32-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="fab32-126">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="fab32-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="fab32-127">Bir eylem beklemede (veya devam ediyor), ancak aygıt 30+ gündür iade edilmedi.</span><span class="sxs-lookup"><span data-stu-id="fab32-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="fab32-128">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="fab32-128">Delete pending</span></span>  <br/> |<span data-ttu-id="fab32-129">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="fab32-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="fab32-130">Bulundu</span><span class="sxs-lookup"><span data-stu-id="fab32-130">Discovered</span></span>  <br/> |<span data-ttu-id="fab32-131">Microsoft 365 İş cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="fab32-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
