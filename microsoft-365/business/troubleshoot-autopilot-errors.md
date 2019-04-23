---
title: AutoPilot cihazı sorunlarını giderme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: AutoPilot aygıt dosyası hatalarında sorun giderme yöntemlerini öğrenin.
ms.openlocfilehash: 9d4a47f78c38d8c076f5b3876a36b6bf46eaaaf3
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279848"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="eeff9-103">AutoPilot cihazı sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="eeff9-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="eeff9-104">Aygıt dosyası hata iletileri</span><span class="sxs-lookup"><span data-stu-id="eeff9-104">Device file error messages</span></span>

<span data-ttu-id="eeff9-105">Bazı hatalar buraya ait bilgileri Microsoft 365 iş AutoPilot aygıt dosyalarıyla çalışırken görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eeff9-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="eeff9-106">**Hata kodu**</span><span class="sxs-lookup"><span data-stu-id="eeff9-106">**Error code**</span></span>|<span data-ttu-id="eeff9-107">**Denemek için düzeltme**</span><span class="sxs-lookup"><span data-stu-id="eeff9-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eeff9-108">Geçersiz istek gövdesi</span><span class="sxs-lookup"><span data-stu-id="eeff9-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="eeff9-109">Bu hatayı görüyorsanız, bu hata nadiren, yapılması gerekenleri işlemi yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="eeff9-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="eeff9-110">Bir aygıt için donanım karma değeri doğru değil.</span><span class="sxs-lookup"><span data-stu-id="eeff9-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="eeff9-111">Bu hatayı görüyorsanız, CSV dosyanızdaki bir aygıtın donanım karma değeri için sağlanan değerin doğru olmadığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="eeff9-112">İlk olarak, değeri doğru yazdığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="eeff9-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="eeff9-113">Değerin doğru olduğunu, ancak bu hatayı hala olmuyor düşünüyorsanız, donanım satıcınıza Yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="eeff9-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="eeff9-114">Başka bir kiracı için atanmış olan aygıt</span><span class="sxs-lookup"><span data-stu-id="eeff9-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="eeff9-115">Bu hatayı görüyorsanız, CSV dosyanızda seri numarasını veya ürün anahtarı bir veya daha fazla aygıt için sağlanan değerin doğru olmadığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="eeff9-116">İlk olarak, değeri doğru yazdığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="eeff9-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="eeff9-117">Değerin doğru olduğunu, ancak bu hatayı hala olmuyor düşünüyorsanız, donanım satıcınıza Yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="eeff9-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="eeff9-118">CSV dosyasını bir seri numarası geçersiz veya ürün anahtarı içerir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="eeff9-119">Bu hatayı görürseniz oluştu kaydetmek için olan aygıt zaten başka bir kuruluş tarafından kayıtlı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-119">If you see this error it means that the device you are tyring to register is already registered by an other organization.</span></span> <span data-ttu-id="eeff9-120">Bu sorunu gidermek için donanım satıcınıza Yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="eeff9-120">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="eeff9-121">Bu aygıt için bir kurulum AutoPilot kullanarak desteklenmiyor</span><span class="sxs-lookup"><span data-stu-id="eeff9-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="eeff9-122">Bu hata, aygıt AutoPilot dağıtım gereksinimlerini karşılamıyor anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-122">This error means the device does not meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="eeff9-123">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="eeff9-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="eeff9-124">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="eeff9-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="eeff9-125">Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.</span><span class="sxs-lookup"><span data-stu-id="eeff9-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="eeff9-126">Aygıt bulunamadı</span><span class="sxs-lookup"><span data-stu-id="eeff9-126">Device not found</span></span>  <br/> |<span data-ttu-id="eeff9-127">Bu hata, bir veya daha fazla aygıt, CSV dosyanızdaki kayıtlı değil, kuruluşunuz için anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="eeff9-127">This error means that one or more devices in your CSV file is not registered to your organization.</span></span> <span data-ttu-id="eeff9-128">Bu sorunu gidermek için donanım satıcınıza Yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="eeff9-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
