---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 cihazlarında Microsoft 365 İş uygulaması koruma ayarlarını nasıl doğrulayayarılamayı öğrenin.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721810"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarında aygıt koruma ayarlarını doğrulama

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10 aygıt ilkelerinin ayarlı olduğunu doğrulama

[Aygıtlar ilkelerini ayarladıktan](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcıların aygıtları üzerinde etkili olması birkaç saat kadar sürebilir. Kullanıcıların cihazlarındaki çeşitli Windows Ayarları ekranlarına bakarak ilkelerin etkili olduğunu doğrulayabilirsiniz. Kullanıcılar Windows 10 cihazlarında Windows Update ve Windows Defender Antivirus ayarlarını değiştiremeyeceğinden, birçok seçenek gri renkte olacaktır.
  
1. **Ayarlar** \> **Güvenlik &amp; Güncelleştirme** \> **Windows Update** \> **Yeniden Başlatma seçeneklerine** gidin ve tüm ayarların gri renkte olduğunu onaylayın. 
    
    ![Tüm Yeniden Başlatma seçenekleri gri renkte.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. **Ayarlar** \> **Güvenlik &amp; Güncelleştirme** \> **Windows Update** \> **Gelişmiş seçeneklerine** gidin ve tüm ayarların gri renkte olduğunu onaylayın. 
    
    ![Windows Advanced güncelleştirmeleri seçeneklerinin tümü gri renktedir.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. **Ayarlar** \> Güncelleştirme \> **güvenliğiwindows** \> **update &amp; ** **Gelişmiş seçeneklerine** \> gidin **Güncelleştirmelerin nasıl teslim edilebildiğini seçin.**
    
    Bazı ayarların kuruluşunuz tarafından gizlendiğini veya yönetildiğini ve tüm seçeneklerin gri renkte olduğunu iletisini (kırmızı renkte) görebileceğinizi doğrulayın.
    
    ![Ayarların kuruluşunuz tarafından gizlenip yönetildiğini belirten sayfanın nasıl teslim edileceğini seçin.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Windows Defender Güvenlik Merkezi'ni açmak için **Ayarlar** \> **Güncelleştirme &amp; güvenlik** \> **Windows Defender'a** \> gidin Windows Defender Güvenlik Merkezi \> **Virüs &amp; iş parçacığı koruması** \> virüs ** &amp; tehdit koruma ayarlarını** **açın'** ı tıklatın. 
    
5. Tüm seçeneklerin gri renkte olduğunu doğrulayın. 
    
    ![Virüs ve tehdit koruma ayarları gri.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>İlgili Konular

[Microsoft 365 İş belgeleri ve kaynakları](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Microsoft 365 İş ile çalışmaya başlama](microsoft-365-business-overview.md)
  
[Microsoft 365 İş yönetimi](manage.md)
  
[Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama](protection-settings-for-windows-10-pcs.md)
  

