---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
ms.openlocfilehash: fcb463fd98f692f7d4802689e0c03fe4e3e648a1
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579852"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="448cc-103">Windows 10 bilgisayarlarda cihaz koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="448cc-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="448cc-104">Windows 10 cihaz ilkelerinin ayar olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="448cc-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="448cc-105">Cihaz [ilkelerini ayardikten](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcıların cihazlarında etkili olarak yer almaları birkaç saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="448cc-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="448cc-106">İlkelerin, kullanıcıların cihazlarında çeşitli Windows Ayarları ekranlarına bakarak etkili olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="448cc-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="448cc-107">Kullanıcılar Windows 10 cihazlarında Windows Update ve Windows Defender Virüsten Koruma ayarlarını değiştiremayacaklarından, birçok seçenek gri görünür.</span><span class="sxs-lookup"><span data-stu-id="448cc-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="448cc-108">Ayarlar  \> **Güncelleştirmesi &amp; güvenlik** \> **Windows Update Yeniden** Başlatma \> **seçeneklerine** gidin ve tüm ayarların gri renkte görüntüde olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="448cc-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Tüm Yeniden Başlatma seçenekleri gri görünür.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="448cc-110">Ayarlar  \> **Güncelleştirmesi &amp; güvenliği** \> **Windows Update Gelişmiş** \> **seçeneklerine** gidin ve tüm ayarların gri olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="448cc-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Gelişmiş güncelleştirme seçeneklerinin hepsi gri görünür.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="448cc-112">Ayarlar **Güncelleştirmesi** \> **güvenliği Windows Update &amp;** \> **Gelişmiş seçeneklerine** gidin \>  \> **Güncelleştirmelerin nasıl teslim alınarak teslim edileceklerini seçin.**</span><span class="sxs-lookup"><span data-stu-id="448cc-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="448cc-113">Bazı ayarların kuruluş tarafından gizlenmiş veya yönetiliyor olduğunu ve tüm seçeneklerin gri renkte olduğunu (kırmızı renkle) gördüğünüzden emin olun.</span><span class="sxs-lookup"><span data-stu-id="448cc-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Güncelleştirmelerin nasıl teslim edilir sayfasında ayarların gizli olduğunu veya kuruluş tarafından yönetil olduğunu seçin.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="448cc-115">Windows Defender Güvenlik Merkezi'ne  gitmek için Windows Defender'ın Ayarlar Güncelleştirmesi güvenliğine gidin, Windows Defender Güvenlik Merkezi Virüs iş parçacığı koruması Virüs tehdit koruması ayarlarını \> **&amp;** \>  \>  \> **&amp;** \> **&amp; aç'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="448cc-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="448cc-116">Tüm seçeneklerin gri renkte olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="448cc-116">Verify that all options are grayed out.</span></span> 
    
    ![Virüs ve tehdit koruması ayarları gri görünür.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="448cc-118">İlgili Konular</span><span class="sxs-lookup"><span data-stu-id="448cc-118">Related Topics</span></span>

[<span data-ttu-id="448cc-119">İşletmeler için Microsoft 365 belgeleri ve kaynakları</span><span class="sxs-lookup"><span data-stu-id="448cc-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="448cc-120">Microsoft 365 İş ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="448cc-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="448cc-121">Microsoft 365 İş'i yönetme</span><span class="sxs-lookup"><span data-stu-id="448cc-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="448cc-122">Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="448cc-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
