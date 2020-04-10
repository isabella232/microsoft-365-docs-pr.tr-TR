---
title: AutoPilot cihazı sorunlarını giderme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Microsoft 365 Business'ta AutoPilot aygıt dosyalarıyla çalışırken görebileceğiniz hataları nasıl giderdiğinizi öğrenin.
ms.openlocfilehash: 8b99e848fa040711785b921d12548f16dadb09af
ms.sourcegitcommit: 4a34b48584071e0c43c920bb35025e34cb4f5d15
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43212143"
---
# <a name="troubleshoot-autopilot-device-errors"></a>AutoPilot cihazı sorunlarını giderme

## <a name="device-file-error-messages"></a>Aygıt dosyası hata iletileri

Microsoft 365 Business'ta AutoPilot aygıt dosyalarıyla çalışırken görebileceğiniz bazı hatalar hakkında bilgiler aşağıda verilmiştir. 
  
|**Hata kodu**|**Denemek için düzeltme**|
|:-----|:-----|
|Geçersiz istek gövdesi  <br/> |Bu hatayı nadiren olur, bu hatayı görürseniz işlemi yeniden deneyin.  <br/> |
|Aygıt için donanım karma değeri doğru değildir.  <br/> |Bu hatayı görürseniz, bir aygıtın donanım karma için CSV dosyanızda sağladığınız değerdoğru olmadığı anlamına gelir. İlk olarak, değerin doğru yazıldığını doğrulayın. Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala oluyorsa, donanım satıcınızdan yardım isteyin.  <br/> |
|Başka bir kiracıya atanan aygıt  <br/> |Bu hatayı görürseniz, csv dosyanızda bir veya daha fazla aygıtın seri numarası veya ürün anahtarı için sağladığınız değerin doğru olmadığı anlamına gelir. İlk olarak, değerin doğru yazıldığını doğrulayın. Değerin doğru olduğunu düşünüyorsanız, ancak bu hata hala oluyorsa, donanım satıcınızdan yardım isteyin.  <br/> |
|CSV dosyası geçersiz bir seri numarası veya ürün anahtarı içerir  <br/> |Bu hatayı görürseniz, kaydetmeye çalıştığınız aygıtın başka bir kuruluş tarafından zaten kaydedilmiş olduğu anlamına gelir. Bu hatayı gidermek için donanım satıcınızdan yardım isteyin.  <br/> |
|Bu cihaz Otomatik Pilot kullanılarak kurulum için desteklenmez  <br/> | Bu hata, aygıtın Otomatik Pilot dağıtım gereksinimlerini karşılamadığı anlamına gelir. Cihazların şu gereksinimleri karşılaması gerekir:  <br/>  Windows 10, sürüm 1703 veya üstü.  <br/>  Windows'un kutudan çıkma deneyiminden geçmemiş yeni aygıtlar.  <br/> |
|Aygıt bulunamadı  <br/> |Bu hata, CSV dosyanızdaki bir veya daha fazla aygıtın kuruluşunuza kayıtlı olmadığı anlamına gelir. Bunu düzeltmek için donanım satıcınızdan yardım isteyin.  <br/> |
