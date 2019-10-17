---
title: AutoPilot cihazlarını oluşturma ve düzenleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Microsoft 365 Business'ta Otomatik Pilot'u kullanarak cihazları nasıl yükleyin öğrenin. Bir aygıta veya aygıt grubuna profil atayabilirsiniz.
ms.openlocfilehash: 4eadaa800aa174bcd9cac50375f68c8471e1684e
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575418"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot cihazlarını oluşturma ve düzenleme

## <a name="upload-a-list-of-devices"></a>Cihaz listesini karşıya yükleme

Cihazları karşıya yüklemek için [Adım adım kılavuzu](add-autopilot-devices-and-profile.md) kullanabileceğiniz gibi, **Cihazlar** sekmesinde de karşıya yükleyebilirsiniz. 
  
Cihazların şu gereksinimleri karşılaması gerekir:
  
- Windows 10, sürüm 1703 veya üstü.
    
- Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.

1. Microsoft 365 Business Admin merkezinde, **Cihazlar** \> **Otomatik Pilot'u**seçin.
  
2. Otomatik **Pilot** sayfasında, **Aygıtlar** \> sekmesini seçin **aygıtlar ekle.**
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Aygıt **ekle** panelinde, \> **Kaydet** \> **Kapat'ı**kaydet'i hazırladığınız [Aygıt listesi CSV dosyasına](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) göz atın.
    
    Bu bilgileri donanım satıcınızdan alabilir veya csv dosyasını oluşturmak için [Get-WindowsAutoPilotInfo PowerShell betiğini](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Cihaza veya cihaz grubuna profil atama

1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin ve bir veya birden çok cihazın yanındaki onay kutusunu işaretleyin. 
    
2. **Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin. 
    
    Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md). 
    
