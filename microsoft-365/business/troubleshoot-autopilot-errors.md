---
title: AutoPilot cihazı sorunlarını giderme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Microsoft 365 İş Ekstra'da AutoPilot cihaz dosyalarıyla çalışırken gördüğünüz hataların nasıl giderilir öğrenin.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578097"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="5de3f-103">AutoPilot cihazı sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="5de3f-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="5de3f-104">Cihaz dosyası hata iletileri</span><span class="sxs-lookup"><span data-stu-id="5de3f-104">Device file error messages</span></span>

<span data-ttu-id="5de3f-105">Microsoft 365 İş Ekstra'da AutoPilot cihaz dosyalarıyla çalışırken gördüğünüz hatalardan bazıları hakkında bilgi edinebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5de3f-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="5de3f-106">**Hata kodu**</span><span class="sxs-lookup"><span data-stu-id="5de3f-106">**Error code**</span></span>|<span data-ttu-id="5de3f-107">**Denemek için düzeltme**</span><span class="sxs-lookup"><span data-stu-id="5de3f-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5de3f-108">Geçersiz istek gövdesi</span><span class="sxs-lookup"><span data-stu-id="5de3f-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="5de3f-109">Bu hata çok seyrek olarak görülür, bu hatayı görüyorsanız işlemi yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="5de3f-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="5de3f-110">Bir cihaz için donanım karma değeri doğru değil.</span><span class="sxs-lookup"><span data-stu-id="5de3f-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="5de3f-111">Bu hatayı görüyorsanız, CSV dosyanıza bir cihazın donanım karması için sağladığınız değer doğru değildir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="5de3f-112">İlk olarak, değerin doğru yaz olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="5de3f-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="5de3f-113">Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5de3f-114">Başka bir kiracıya atanmış cihaz</span><span class="sxs-lookup"><span data-stu-id="5de3f-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="5de3f-115">Bu hatayı görüyorsanız, CSV dosyanıza bir veya birden çok cihazın seri numarası veya ürün anahtarı için sağladığınız değer doğru değildir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="5de3f-116">İlk olarak, değerin doğru yaz olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="5de3f-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="5de3f-117">Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5de3f-118">CSV dosyası geçersiz bir seri numarası veya ürün anahtarı içeriyor</span><span class="sxs-lookup"><span data-stu-id="5de3f-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="5de3f-119">Bu hatayı görüyorsanız, kaydolmaya çalışıyorsanız cihaz zaten başka bir kuruluş tarafından kaydedilmiş demektir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="5de3f-120">Bu hatayı düzeltmek için donanım satıcınıza yardım sorun.</span><span class="sxs-lookup"><span data-stu-id="5de3f-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="5de3f-121">Bu cihaz AutoPilot kullanarak kurulum için desteklenmiyor</span><span class="sxs-lookup"><span data-stu-id="5de3f-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="5de3f-122">Bu hata, cihazın AutoPilot dağıtım gereksinimlerini karşılamıyor olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="5de3f-123">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="5de3f-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="5de3f-124">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="5de3f-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="5de3f-125">Windows'un ilk gelen deneyimine henüz sahip olmayan yeni cihazlar.</span><span class="sxs-lookup"><span data-stu-id="5de3f-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="5de3f-126">Cihaz bulunamadı</span><span class="sxs-lookup"><span data-stu-id="5de3f-126">Device not found</span></span>  <br/> |<span data-ttu-id="5de3f-127">Bu hata, CSV dosyanız içinde yer alan bir veya birden çok cihaz kuruma kayıtlı değil demektir.</span><span class="sxs-lookup"><span data-stu-id="5de3f-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="5de3f-128">Bunu düzeltmek için donanım satıcınıza yardım sorun.</span><span class="sxs-lookup"><span data-stu-id="5de3f-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
