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
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400964"
---
# <a name="device-states"></a><span data-ttu-id="0066c-103">Cihaz durumları</span><span class="sxs-lookup"><span data-stu-id="0066c-103">Device states</span></span>

<span data-ttu-id="0066c-104">**Cihaz eylemleri** listesindeki (Yönetim giriş sayfası \> **Cihaz eylemleri**) cihazlar aşağıdaki durumlarda olabilir.</span><span class="sxs-lookup"><span data-stu-id="0066c-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="0066c-106">**Durum**</span><span class="sxs-lookup"><span data-stu-id="0066c-106">**Status**</span></span>|<span data-ttu-id="0066c-107">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="0066c-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0066c-108">Intune tarafından yönetilen</span><span class="sxs-lookup"><span data-stu-id="0066c-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="0066c-109">Microsoft 365 Business Premium tarafından yönetildi.</span><span class="sxs-lookup"><span data-stu-id="0066c-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="0066c-110">Devre dışı bırakma bekliyor</span><span class="sxs-lookup"><span data-stu-id="0066c-110">Retire pending</span></span>  <br/> |<span data-ttu-id="0066c-111">Microsoft 365 Business Premium, şirket verilerini aygıttan kaldırmaya hazırlanıyor.</span><span class="sxs-lookup"><span data-stu-id="0066c-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="0066c-112">Devre dışı bırakma sürüyor</span><span class="sxs-lookup"><span data-stu-id="0066c-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="0066c-113">Microsoft 365 Business Premium şu anda şirket verilerini aygıttan kaldırıyor.</span><span class="sxs-lookup"><span data-stu-id="0066c-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="0066c-114">Devre dışı bırakma başarısız</span><span class="sxs-lookup"><span data-stu-id="0066c-114">Retire failed</span></span>  <br/> | <span data-ttu-id="0066c-115">Şirket verilerini kaldırma işlemi başarısız oldu.</span><span class="sxs-lookup"><span data-stu-id="0066c-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="0066c-116">Emekli iptal edildi</span><span class="sxs-lookup"><span data-stu-id="0066c-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="0066c-117">Emekli eylemi iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="0066c-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="0066c-118">Temizleme işlemi beklemede</span><span class="sxs-lookup"><span data-stu-id="0066c-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="0066c-119">Fabrika sıfırlamasının başlatılması bekleniyor.</span><span class="sxs-lookup"><span data-stu-id="0066c-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="0066c-120">Temizleme işlemi sürüyor</span><span class="sxs-lookup"><span data-stu-id="0066c-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="0066c-121">Fabrika sıfırlaması gönderildi.</span><span class="sxs-lookup"><span data-stu-id="0066c-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="0066c-122">Temizleme başarısız oldu</span><span class="sxs-lookup"><span data-stu-id="0066c-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="0066c-123">Fabrika sıfırlama yapamadım.</span><span class="sxs-lookup"><span data-stu-id="0066c-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="0066c-124">Silme iptal edildi</span><span class="sxs-lookup"><span data-stu-id="0066c-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="0066c-125">Fabrika silme iptal edildi.</span><span class="sxs-lookup"><span data-stu-id="0066c-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="0066c-126">Uygun olmayan durumda</span><span class="sxs-lookup"><span data-stu-id="0066c-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="0066c-127">Bir eylem beklemede (veya devam ediyor), ancak aygıt 30+ gündür iade edilmedi.</span><span class="sxs-lookup"><span data-stu-id="0066c-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="0066c-128">Silme bekliyor</span><span class="sxs-lookup"><span data-stu-id="0066c-128">Delete pending</span></span>  <br/> |<span data-ttu-id="0066c-129">Silme eylemi bekliyor.</span><span class="sxs-lookup"><span data-stu-id="0066c-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="0066c-130">Bulundu</span><span class="sxs-lookup"><span data-stu-id="0066c-130">Discovered</span></span>  <br/> |<span data-ttu-id="0066c-131">Microsoft 365 Business Premium cihazı algılamıştır.</span><span class="sxs-lookup"><span data-stu-id="0066c-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
