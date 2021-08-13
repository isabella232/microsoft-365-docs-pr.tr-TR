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
description: OnePilot'ta AutoPilot cihaz dosyalarıyla çalışırken gördüğünüz hataların nasıl gider Microsoft 365 İş Ekstra.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809190"
---
# <a name="troubleshoot-autopilot-device-errors"></a>AutoPilot cihazı sorunlarını giderme

## <a name="device-file-error-messages"></a>Cihaz dosyası hata iletileri

Burada, aynı dosyada AutoPilot cihaz dosyalarıyla çalışırken gördüğünüz hatalardan bazıları hakkında Microsoft 365 İş Ekstra. 
  
|**Hata kodu**|**Deneme için düzeltme**|
|:-----|:-----|
|Geçersiz istek gövdesi  <br/> |Bu hata çok seyrek olarak, bu hatayı görüyorsanız işlemi yeniden deneyin.  <br/> |
|Bir cihaz için donanım karma değeri doğru değildir.  <br/> |Bu hatayı görüyorsanız, CSV dosyanıza bir cihazın donanım karması için sağladığınız değer yanlıştır. İlk olarak, değerin doğru yaz hata değerinin doğru yaz olduğunu doğrulayın. Değerin doğru olduğunu düşünüyorsanız ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.  <br/> |
|Başka bir kiracıya atanmış cihaz  <br/> |Bu hatayı görüyorsanız, CSV dosyanıza bir veya birden çok cihazın seri numarası ya da ürün anahtarı için sağladığınız değer yanlıştır. İlk olarak, değerin doğru yaz hata değerinin doğru yaz olduğunu doğrulayın. Değerin doğru olduğunu düşünüyorsanız ancak bu hata hala devam ediyorsa donanım satıcıdan yardım istemeniz gerekir.  <br/> |
|CSV dosyası geçersiz bir seri numarası veya ürün anahtarı içeriyor  <br/> |Bu hatayı görüyorsanız, kaydetmeye çalıştığınız cihaz zaten başka bir kuruluş tarafından kaydedilmiş demektir. Bu hatayı düzeltmek için donanım satıcınıza yardımını sorun.  <br/> |
|Bu cihaz AutoPilot kullanılarak kurulum için desteklenmiyor  <br/> | Bu hata, cihazın AutoPilot dağıtım gereksinimlerini karşılamıyor olduğu anlamına gelir. Cihazların şu gereksinimleri karşılaması gerekir:  <br/>  Windows 10, sürüm 1703 veya üstü.  <br/>  Henüz ilk ve son Windows yeni cihazlar.  <br/> |
|Cihaz bulunamadı  <br/> |Bu hata, CSV dosyanıza bir veya birden çok cihazın kuruma kayıtlı olmadığını gösterir. Bunu düzeltmek için donanım satıcıdan yardım istemeniz gerekir.  <br/> |
