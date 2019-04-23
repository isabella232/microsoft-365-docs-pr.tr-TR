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
# <a name="troubleshoot-autopilot-device-errors"></a>AutoPilot cihazı sorunlarını giderme

## <a name="device-file-error-messages"></a>Aygıt dosyası hata iletileri

Bazı hatalar buraya ait bilgileri Microsoft 365 iş AutoPilot aygıt dosyalarıyla çalışırken görebilirsiniz. 
  
|**Hata kodu**|**Denemek için düzeltme**|
|:-----|:-----|
|Geçersiz istek gövdesi  <br/> |Bu hatayı görüyorsanız, bu hata nadiren, yapılması gerekenleri işlemi yeniden deneyin.  <br/> |
|Bir aygıt için donanım karma değeri doğru değil.  <br/> |Bu hatayı görüyorsanız, CSV dosyanızdaki bir aygıtın donanım karma değeri için sağlanan değerin doğru olmadığını gösterir. İlk olarak, değeri doğru yazdığınızdan emin olun. Değerin doğru olduğunu, ancak bu hatayı hala olmuyor düşünüyorsanız, donanım satıcınıza Yardım isteyin.  <br/> |
|Başka bir kiracı için atanmış olan aygıt  <br/> |Bu hatayı görüyorsanız, CSV dosyanızda seri numarasını veya ürün anahtarı bir veya daha fazla aygıt için sağlanan değerin doğru olmadığını gösterir. İlk olarak, değeri doğru yazdığınızdan emin olun. Değerin doğru olduğunu, ancak bu hatayı hala olmuyor düşünüyorsanız, donanım satıcınıza Yardım isteyin.  <br/> |
|CSV dosyasını bir seri numarası geçersiz veya ürün anahtarı içerir.  <br/> |Bu hatayı görürseniz oluştu kaydetmek için olan aygıt zaten başka bir kuruluş tarafından kayıtlı anlamına gelir. Bu sorunu gidermek için donanım satıcınıza Yardım isteyin.  <br/> |
|Bu aygıt için bir kurulum AutoPilot kullanarak desteklenmiyor  <br/> | Bu hata, aygıt AutoPilot dağıtım gereksinimlerini karşılamıyor anlamına gelir. Cihazların şu gereksinimleri karşılaması gerekir:  <br/>  Windows 10, sürüm 1703 veya üstü.  <br/>  Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.  <br/> |
|Aygıt bulunamadı  <br/> |Bu hata, bir veya daha fazla aygıt, CSV dosyanızdaki kayıtlı değil, kuruluşunuz için anlamına gelir. Bu sorunu gidermek için donanım satıcınıza Yardım isteyin.  <br/> |
   
