---
title: AutoPilot cihazlarını oluşturma ve düzenleme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Microsoft 365 İş Ekstra'da AutoPilot kullanarak cihazları karşıya Microsoft 365 İş Ekstra. Bir cihaza veya cihaz grubuna profil atabilirsiniz.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867046"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot cihazlarını oluşturma ve düzenleme

## <a name="upload-a-list-of-devices"></a>Cihaz listesini karşıya yükleme

Cihazları karşıya yüklemek [için Adım adım kılavuzu kullanabilirsiniz,](add-autopilot-devices-and-profile.md) ancak cihazları Cihazlar sekmesinden de karşıya **yükleyebilirsiniz.** 
  
Cihazlar şu gereksinimleri karşılamalıdır:
  
- Windows 10, sürüm 1703 veya sonrası
    
- Henüz ilk ve en son Windows yeni cihazlar

1. Daha fazla Microsoft 365 yönetim merkezi **Devices** \> **AutoPilot'ı seçin.**
  
2. **AutoPilot sayfasında** Cihazlar sekmesini Cihaz  \> **ekle'yi seçin.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Cihaz **ekle panelinde,** Kapat'ı [Kaydet'i hazırlığında hazır bulundurarak cihaz](../admin/misc/device-list.md) listesi CSV \> **dosyasına** \> **göz atabilirsiniz.**
    
    Bu bilgileri donanım satıcıdan edinebilirsiniz veya CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) betiği kullanabilirsiniz. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Cihaza veya cihaz grubuna profil atama

1. Şu cihazları **Windows** Cihazlar sekmesini **seçin ve** bir veya birden çok cihaz yanındaki onay kutusunu seçin. 
    
2. **Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin. 
    
    Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md). 
