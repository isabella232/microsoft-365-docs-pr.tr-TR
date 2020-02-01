---
title: AutoPilot cihazı sorunlarını giderme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
description: Otomatik Pilot aygıt dosyası hatalarını nasıl gidereceklerini öğrenin.
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594218"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="ce75e-103">AutoPilot cihazı sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="ce75e-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="ce75e-104">Aygıt dosyası hata iletileri</span><span class="sxs-lookup"><span data-stu-id="ce75e-104">Device file error messages</span></span>

<span data-ttu-id="ce75e-105">Microsoft 365 Business'ta AutoPilot aygıt dosyalarıyla çalışırken görebileceğiniz bazı hatalar hakkında bilgiler aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="ce75e-106">**Hata kodu**</span><span class="sxs-lookup"><span data-stu-id="ce75e-106">**Error code**</span></span>|<span data-ttu-id="ce75e-107">**Denemek için düzeltme**</span><span class="sxs-lookup"><span data-stu-id="ce75e-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce75e-108">Geçersiz istek gövdesi</span><span class="sxs-lookup"><span data-stu-id="ce75e-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="ce75e-109">Bu hatayı nadiren olur, bu hatayı görürseniz işlemi yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="ce75e-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="ce75e-110">Aygıt için donanım karma değeri doğru değildir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="ce75e-111">Bu hatayı görürseniz, bir aygıtın donanım karma için CSV dosyanızda sağladığınız değerdoğru olmadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="ce75e-112">İlk olarak, değerin doğru yazıldığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="ce75e-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ce75e-113">Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala oluyorsa, donanım satıcınızdan yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="ce75e-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce75e-114">Başka bir kiracıya atanan aygıt</span><span class="sxs-lookup"><span data-stu-id="ce75e-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="ce75e-115">Bu hatayı görürseniz, csv dosyanızda bir veya daha fazla aygıtın seri numarası veya ürün anahtarı için sağladığınız değerin doğru olmadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="ce75e-116">İlk olarak, değerin doğru yazıldığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="ce75e-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="ce75e-117">Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala oluyorsa, donanım satıcınızdan yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="ce75e-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce75e-118">CSV dosyası geçersiz bir seri numarası veya ürün anahtarı içerir</span><span class="sxs-lookup"><span data-stu-id="ce75e-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="ce75e-119">Bu hatayı görürseniz, kaydetmeye çalıştığınız aygıtın başka bir kuruluş tarafından zaten kaydedilmiş olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="ce75e-120">Bu hatayı gidermek için donanım satıcınızdan yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="ce75e-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="ce75e-121">Bu cihaz Otomatik Pilot kullanılarak kurulum için desteklenmez</span><span class="sxs-lookup"><span data-stu-id="ce75e-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="ce75e-122">Bu hata, aygıtın Otomatik Pilot dağıtım gereksinimlerini karşılamadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="ce75e-123">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="ce75e-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="ce75e-124">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="ce75e-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="ce75e-125">Windows'un kutudan çıkma deneyiminden geçmemiş yeni aygıtlar.</span><span class="sxs-lookup"><span data-stu-id="ce75e-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="ce75e-126">Aygıt bulunamadı</span><span class="sxs-lookup"><span data-stu-id="ce75e-126">Device not found</span></span>  <br/> |<span data-ttu-id="ce75e-127">Bu hata, CSV dosyanızdaki bir veya daha fazla aygıtın kuruluşunuza kayıtlı olmadığı anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="ce75e-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="ce75e-128">Bunu düzeltmek için donanım satıcınızdan yardım isteyin.</span><span class="sxs-lookup"><span data-stu-id="ce75e-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
