---
title: AutoPilot cihazlarını oluşturma ve düzenleme
f1.keywords:
- NOCSH
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
ms.openlocfilehash: 640e4af7cccde83c87d90a875c1d44dead7255ca
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42066002"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot cihazlarını oluşturma ve düzenleme

## <a name="upload-a-list-of-devices"></a>Cihaz listesini karşıya yükleme

Aygıtyüklemek için [adım adım kılavuzunu](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak **Aygıtlar** sekmesine aygıt yükleyebilirsiniz. 
  
Aygıtlar bu gereksinimleri karşılamalıdır:
  
- Windows 10, sürüm 1703 veya sonrası
    
- Windows'dan kutudan çıkma deneyiminden geçmemiş yeni aygıtlar

1. Microsoft 365 Business Admin merkezinde, **Cihazlar** \> **Otomatik Pilot'u**seçin.
  
2. Otomatik **Pilot** sayfasında, **Aygıtlar** \> sekmesini seçin **aygıtlar ekle.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Aygıt **ekle** panelinde, **Kaydet** \> **Kapat'ı**kaydet'i \> hazırladığınız [Aygıt listesi CSV dosyasına](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) göz atın.
    
    Bu bilgileri donanım satıcınızdan alabilir veya Bir CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell komut dosyasını](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Cihaza veya cihaz grubuna profil atama

1. **Windows'u Hazırla** sayfasında **Aygıtlar** sekmesini seçin ve bir veya daha fazla aygıtın yanındaki onay kutusunu seçin. 
    
2. **Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin. 
    
    Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md). 
    
