---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Kullanıcılarınızı Windows 10 cihazlarında Microsoft 365 İş uygulama koruma ayarlarının geçerli olduğunu doğrulamayı öğrenin.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912424"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarda cihaz koruma ayarlarını doğrulama

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10 cihaz ilkelerinin ayar olduğunu doğrulama

Cihaz [ilkelerini ayardikten](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcıların cihazlarında etkili olarak yer almaları birkaç saat kadar sürebilir. İlkelerin, kullanıcıların cihazlarında çeşitli Windows Ayarları ekranlarına bakarak etkili olduğunu onaylayın. Kullanıcılar Windows 10 cihazlarında Windows Update ve Windows Defender Virüsten Koruma ayarlarını değiştiremayacaklarından, birçok seçenek gri görünür.
  
1. Ayarlar  \> **Güncelleştirmesi &amp; güvenlik** \> **Windows Update Yeniden** Başlatma \> **seçeneklerine** gidin ve tüm ayarların gri renkte görüntüde olduğunu onaylayın. 
    
    ![Tüm Yeniden Başlatma seçenekleri gri görünür.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Ayarlar  \> **Güncelleştirmesi &amp; güvenliği** \> **Windows Update Gelişmiş** \> **seçeneklerine** gidin ve tüm ayarların gri olduğunu onaylayın. 
    
    ![Windows Gelişmiş güncelleştirme seçeneklerinin hepsi gri görünür.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Ayarlar **Güncelleştirmesi** \> **güvenliği Windows Update &amp;** \> **Gelişmiş seçeneklerine** gidin \>  \> **Güncelleştirmelerin nasıl teslim alınarak teslim edileceklerini seçin.**
    
    Bazı ayarların kuruluş tarafından gizlenmiş veya yönetiliyor olduğunu ve tüm seçeneklerin gri renkte olduğunu (kırmızı renkle) gördüğünüzden emin olun.
    
    ![Güncelleştirmelerin nasıl teslim edilir sayfasında ayarların gizli olduğunu veya kuruluş tarafından yönetil olduğunu seçin.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Windows Defender Güvenlik Merkezi'ne  gitmek için Windows Defender'ın Ayarlar Güncelleştirmesi güvenliğine gidin, Windows Defender Güvenlik Merkezi Virüs iş parçacığı koruması Virüs tehdit koruması ayarlarını \> **&amp;** \>  \>  \> **&amp;** \> **&amp; aç'a tıklayın.** 
    
5. Tüm seçeneklerin gri renkte olduğunu doğrulayın. 
    
    ![Virüs ve tehdit koruması ayarları gri görünür.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>İlgili Konular

[İşletmeler için Microsoft 365 belgeleri ve kaynakları](./index.yml)
  
[Microsoft 365 İş ile çalışmaya başlama](microsoft-365-business-overview.md)
  
[Microsoft 365 İş'i yönetme](manage.md)
  
[Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama](protection-settings-for-windows-10-pcs.md)
