---
title: AutoPilot profillerini oluşturma ve düzenleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983140"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot profillerini oluşturma ve düzenleme

## <a name="create-a-profile"></a>Profil oluşturma

Profiller bir cihaza veya cihaz grubuna uygulanır,
  
1. Microsoft 365 İş Yönetim merkezinde **Cihaz eylemleri** kartında **Windows'u AutoPilot ile Dağıt**'ı seçin. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. **Windows'u Hazırla** sayfasında **Profiller** sekmesi \> **Profil oluştur**'u seçin.
    
3. **Profil oluştur** sayfasında, profili tanımanıza yardımcı olacak bir ad (örneğin, Pazarlama) girin, istediğiniz ayarı açın (daha fazla bilgi edinmek için bkz. [AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md)) ve **Kaydet**'i seçin.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Cihaza profil uygulama

Profili oluşturduktan sonra bir cihaza veya cihaz grubuna uygulayabilirsiniz. [Adım adım kılavuzdan](add-autopilot-devices-and-profile.md) mevcut bir profili seçip yeni cihazlara uygulayabilir ya da bir cihaza veya cihaz grubuna yönelik mevcut bir profili değiştirebilirsiniz. 
  
1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Onay kutusunu aygıt adının yanındaki ve **Aygıt** Bölmesi'ni tıklatın, **atanan profil** açılan listesinden bir profil seçin \> **kaydedin**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profili düzenleme, silme veya kaldırma

Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir. 
  
### <a name="edit-a-profile"></a>Profili düzenleme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Aygıt adının yanındaki onay kutusunu tıklatın ve **Profil** paneli kullanılabilir ayarlarını güncelleştirmek \> **kaydedin**.
    
    Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.
    
### <a name="delete-a-profile"></a>Profili silme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Bir cihaz adının yanındaki onay kutusuna tıklayın ve **Profil** bölmesinden **Profili sil** \> **Kaydet**'e tıklayın.
    
    Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.
    
### <a name="remove-a-profile"></a>Profili kaldırma

1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Onay kutusunu aygıt adının yanındaki ve **Aygıt** Bölmesi'ni tıklatın, **Hiçbiri** **atanmadı profil** açılan listesinden seçin \> **kaydedin**.
    
