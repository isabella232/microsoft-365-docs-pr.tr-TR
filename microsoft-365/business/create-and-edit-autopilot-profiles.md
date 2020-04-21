---
title: AutoPilot profillerini oluşturma ve düzenleme
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Bir Otomatik Pilot profili oluşturmayı ve bir aygıta uygulamayı, profili düzenlemeyi veya silmeyi veya bir profili aygıttan kaldırmayı öğrenin.
ms.openlocfilehash: a6e02ab56faeb08718a9831657b55cff0356a4ec
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627384"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot profillerini oluşturma ve düzenleme

## <a name="create-a-profile"></a>Profil oluşturma

Profiller bir cihaza veya cihaz grubuna uygulanır,
  
1. Microsoft 365 yönetici merkezinde, **Cihazlar** \> **Otomatik Pilot**seçin.
  
2. Otomatik **Pilot** sayfasında **Profiller** sekmesini \> seçin **profil oluştur.**
    
3. Profil **Oluştur** sayfasında, profilin kimliğini belirlemenize yardımcı olacak bir ad girin, örneğin Pazarlama. İstediğiniz ayarı açın ve sonra **Kaydet'i**seçin. Otomatik Pilot profil ayarları hakkında daha fazla bilgi [için, Otomatik Pilot Profil ayarları hakkında](autopilot-profile-settings.md)bakın.
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Cihaza profil uygulama

Bir profil oluşturduktan sonra, profili bir aygıta veya aygıt grubuna uygulayabilirsiniz. [Adım adım kılavuzda](add-autopilot-devices-and-profile.md) varolan bir profili seçebilir ve yeni aygıtlara uygulayabilir veya aygıt veya aygıt grubu için varolan profili değiştirebilirsiniz. 
  
1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Aygıt adının yanındaki onay kutusunu seçin ve **Aygıt** panelinde, **Atanan profil** açılır listesinden \> bir profil seçin **Kaydet**.
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profili düzenleme, silme veya kaldırma

Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir. 
  
### <a name="edit-a-profile"></a>Profili düzenleme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Bir aygıt adının yanındaki onay kutusunu seçin ve **Profil** panelinde kullanılabilir \> ayarlardan herhangi birini **kaydet'i**güncelleştirin.
    
    Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.
    
### <a name="delete-a-profile"></a>Profili silme

1. **Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin. 
    
2. Aygıt adının yanındaki onay kutusunu seçin ve **Profil** panelinde **Profili** \> **Sil'i**seçin.
    
    Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.
    
### <a name="remove-a-profile"></a>Profili kaldırma

1. **Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin. 
    
2. Aygıt adının yanındaki onay kutusunu seçin ve **Aygıt** panelinde **Atanan profil** açılır listesinden \> **Kaydet'i**yok'u seçin. **None**
    
