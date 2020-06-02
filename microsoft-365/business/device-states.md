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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: İşletmeler için Microsoft 365'teki Yönetici evindeki Aygıt eylemleri listesindeki çeşitli aygıt durumları hakkında bilgi edinin.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471189"
---
# <a name="device-states"></a><span data-ttu-id="5aa67-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="5aa67-103">Device states</span></span>

<span data-ttu-id="5aa67-104">Bu makale Microsoft 365 Business Premium için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="5aa67-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="5aa67-105">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="5aa67-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="5aa67-107">**Durum**</span><span class="sxs-lookup"><span data-stu-id="5aa67-107">**Status**</span></span>|<span data-ttu-id="5aa67-108">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="5aa67-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5aa67-109">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="5aa67-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="5aa67-110">Microsoft 365 Business Premium tarafından yönetildi.</span><span class="sxs-lookup"><span data-stu-id="5aa67-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="5aa67-111">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="5aa67-111">Retire pending</span></span>  <br/> |<span data-ttu-id="5aa67-112">Microsoft 365 Business Premium, şirket verilerini aygıttan kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="5aa67-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="5aa67-113">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="5aa67-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="5aa67-114">Microsoft 365 Business Premium şu anda şirket verilerini aygıttan kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="5aa67-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="5aa67-115">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="5aa67-115">Retire failed</span></span>  <br/> | <span data-ttu-id="5aa67-116">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="5aa67-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="5aa67-117">Emekli iptal edildi</span><span class="sxs-lookup"><span data-stu-id="5aa67-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="5aa67-118">Emekli eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="5aa67-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="5aa67-119">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="5aa67-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="5aa67-120">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="5aa67-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="5aa67-121">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="5aa67-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="5aa67-122">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="5aa67-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="5aa67-123">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="5aa67-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="5aa67-124">Fabrika sıfırlama yapamadım.</span><span class="sxs-lookup"><span data-stu-id="5aa67-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="5aa67-125">Silme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="5aa67-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="5aa67-126">Fabrika silme iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="5aa67-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="5aa67-127">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="5aa67-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="5aa67-128">Bir eylem beklemede (veya devam ediyor), ancak aygıt 30+ gündür iade edilmedi.</span><span class="sxs-lookup"><span data-stu-id="5aa67-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="5aa67-129">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="5aa67-129">Delete pending</span></span>  <br/> |<span data-ttu-id="5aa67-130">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="5aa67-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="5aa67-131">Bulundu</span><span class="sxs-lookup"><span data-stu-id="5aa67-131">Discovered</span></span>  <br/> |<span data-ttu-id="5aa67-132">Microsoft 365 Business Premium cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="5aa67-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
