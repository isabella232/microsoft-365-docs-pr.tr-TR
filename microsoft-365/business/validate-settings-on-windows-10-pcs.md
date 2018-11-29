---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 aygıtları'nda bulunan Microsoft 365 iş app koruma ayarlarını doğrulamak öğrenin.
ms.openlocfilehash: db05c86bd75cc30e22e025034a3dab478d0f5365
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982710"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>10 PC'lerde Windows aygıtı koruma ayarlarını doğrula

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10 aygıt ilkeleri ayarlandığını doğrulayın

[Aygıtları ilkelerini kurun](protection-settings-for-windows-10-pcs.md)sonra onu ilkesi kullanıcıların aygıtları üzerinde etkili olması birkaç saat sürebilir. İlkeleri kullanıcıların aygıtlarda çeşitli Windows ayarları ekranlar bakarak etkisi geçen onaylayabilirsiniz. Kullanıcılar Windows 10 aygıtlarında Windows Update ve Windows Defender virüsten koruma ayarlarını değiştirmek mümkün değildir çünkü bu seçenekleri bir sürü dışarı gri.
  
1. **Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **yeniden başlatma seçenekleri** ve tüm ayarları kullanıma gri olduğunu onaylayın. 
    
    ![Yeniden başlatma seçenekleri, dışarı gri.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. **Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **Gelişmiş Seçenekleri** ve tüm ayarları kullanıma gri olduğunu onaylayın. 
    
    ![Windows Gelişmiş Seçenekler güncelleştirmeleri tüm nda.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. **Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **Gelişmiş Seçenekler** \> **Seç güncelleştirmeleri nasıl dağıtılır**.
    
    Gizli ya da kuruluşunuz tarafından yönetilen bazı ayarları ve seçenekleri nda iletide (kırmızı) görebilirsiniz onaylayın.
    
    ![Güncelleştirmeleri nasıl dağıtılır seçin sayfa ayarları gizli veya kuruluşunuz tarafından yönetilen gösterir.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Windows Defender'ın Güvenlik Merkezi'ni açmak için **ayarları** ' na gidin \> **güncelleştirme &amp; güvenlik** \> **Windows Defender** \> **Windows Defender Güvenlik Merkezi'ni Aç** öğesini \> **virüs &amp; iş parçacığı koruma** \> **virüs &amp; iş parçacığı koruma ayarlarını**. 
    
5. Out tüm seçenekler gri olduğunu doğrulayın. 
    
    ![Virüs ve tehdit koruması ayarları nda.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>İlgili Konular

[Microsoft 365 İş belgeleri ve kaynakları](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 İş ile çalışmaya başlama](microsoft-365-business-overview.md)
  
[Microsoft 365 İş yönetimi](manage.md)
  
[Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama](protection-settings-for-windows-10-pcs.md)
  

