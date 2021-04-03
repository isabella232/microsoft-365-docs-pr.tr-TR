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
# <a name="troubleshoot-autopilot-device-errors"></a>AutoPilot cihazı sorunlarını giderme

## <a name="device-file-error-messages"></a>Cihaz dosyası hata iletileri

Microsoft 365 İş Ekstra'da AutoPilot cihaz dosyalarıyla çalışırken gördüğünüz hatalardan bazıları hakkında bilgi edinebilirsiniz. 
  
|**Hata kodu**|**Denemek için düzeltme**|
|:-----|:-----|
|Geçersiz istek gövdesi  <br/> |Bu hata çok seyrek olarak görülür, bu hatayı görüyorsanız işlemi yeniden deneyin.  <br/> |
|Bir cihaz için donanım karma değeri doğru değil.  <br/> |Bu hatayı görüyorsanız, CSV dosyanıza bir cihazın donanım karması için sağladığınız değer doğru değildir. İlk olarak, değerin doğru yaz olduğunu doğrulayın. Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.  <br/> |
|Başka bir kiracıya atanmış cihaz  <br/> |Bu hatayı görüyorsanız, CSV dosyanıza bir veya birden çok cihazın seri numarası veya ürün anahtarı için sağladığınız değer doğru değildir. İlk olarak, değerin doğru yaz olduğunu doğrulayın. Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.  <br/> |
|CSV dosyası geçersiz bir seri numarası veya ürün anahtarı içeriyor  <br/> |Bu hatayı görüyorsanız, kaydolmaya çalışıyorsanız cihaz zaten başka bir kuruluş tarafından kaydedilmiş demektir. Bu hatayı düzeltmek için donanım satıcınıza yardım sorun.  <br/> |
|Bu cihaz AutoPilot kullanarak kurulum için desteklenmiyor  <br/> | Bu hata, cihazın AutoPilot dağıtım gereksinimlerini karşılamıyor olduğu anlamına gelir. Cihazların şu gereksinimleri karşılaması gerekir:  <br/>  Windows 10, sürüm 1703 veya üstü.  <br/>  Windows'un ilk gelen deneyimine henüz sahip olmayan yeni cihazlar.  <br/> |
|Cihaz bulunamadı  <br/> |Bu hata, CSV dosyanız içinde yer alan bir veya birden çok cihaz kuruma kayıtlı değil demektir. Bunu düzeltmek için donanım satıcınıza yardım sorun.  <br/> |
