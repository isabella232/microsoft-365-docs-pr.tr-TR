---
title: AutoPilot profillerini oluşturma ve düzenleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Oluşturmak, düzenlemek, silmek veya kaldırmak AutoPilot profilleri hakkında bilgi edinin. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277181"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot profillerini oluşturma ve düzenleme

## <a name="create-a-profile"></a>Profil oluşturma

Profiller bir cihaza veya cihaz grubuna uygulanır,
  
1. Microsoft 365 iş Yönetim Merkezi'nde **cihaz** seçmenizi \> **AutoPilot**.
  
2. **AutoPilot** sayfasında, **Profiller** sekmesini seçin \> **Profil Oluştur**.
    
3. **Profil oluştur** sayfasında, profili tanımanıza yardımcı olacak bir ad (örneğin, Pazarlama) girin, istediğiniz ayarı açın (daha fazla bilgi edinmek için bkz. [AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md)) ve **Kaydet**'i seçin.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Cihaza profil uygulama

Profili oluşturduktan sonra bir cihaza veya cihaz grubuna uygulayabilirsiniz. [Adım adım kılavuzdan](add-autopilot-devices-and-profile.md) mevcut bir profili seçip yeni cihazlara uygulayabilir ya da bir cihaza veya cihaz grubuna yönelik mevcut bir profili değiştirebilirsiniz. 
  
1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profili düzenleme, silme veya kaldırma

Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir. 
  
### <a name="edit-a-profile"></a>Profili düzenleme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.
    
    Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.
    
### <a name="delete-a-profile"></a>Profili silme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Bir cihaz adının yanındaki onay kutusuna tıklayın ve **Profil** bölmesinden **Profili sil** \> **Kaydet**'e tıklayın.
    
    Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.
    
### <a name="remove-a-profile"></a>Profili kaldırma

1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.
    
