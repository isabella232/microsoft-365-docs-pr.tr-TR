---
title: Bilgisayarlar için uygulama koruma Windows 10 doğrulama
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
description: İşletmeler için Microsoft 365 koruma ayarlarının kullanıcılarınızı ve cihazlarınızı nasıl Windows 10 öğrenin.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925269"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="9f7f9-103">Bilgisayarlar için cihaz koruma Windows 10 doğrulama</span><span class="sxs-lookup"><span data-stu-id="9f7f9-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="9f7f9-104">Cihaz ilkelerinin Windows 10 ayar olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="9f7f9-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="9f7f9-105">Cihaz [ilkelerini ayarladikten](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcı cihazlarında etkili olmazken birkaç saat sürebilir.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="9f7f9-106">İlkelerin, kullanıcıların cihazlarında çeşitli ekranlara bakarak Windows Ayarlar olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="9f7f9-107">Kullanıcılar mobil cihazlarında Güncelleştirme Windows Güncelleştirme Windows Defender Virüsten Koruma ayarlarını değiştire Windows 10, pek çok seçenek gri görünür.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="9f7f9-108">Güvenlik  ayarlarını \> **&amp; Ayarlar'Windows** \> **Yeniden Başlatma seçeneklerini** \> **güncelleştir'e** gidin ve tüm ayarların gri olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Yeniden başlatma seçeneklerinin tüm seçenekleri gri gösterilir.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="9f7f9-110">Gelişmiş **Ayarlar** \> **Güncelleştirme &amp;** \> **Windows'e** \> **gidin** ve tüm ayarların gri olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Gelişmiş güncelleştirme seçeneklerinin hepsi gri renkte.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="9f7f9-112">Güncelleştirme  \> **Ayarlar-Posta &amp; Windows** \> **Güncelleştirme Gelişmiş seçenekleri** \>  \> **Güncelleştirmelerin nasıl teslim edileceklerini seçin seçeneğine gidin.**</span><span class="sxs-lookup"><span data-stu-id="9f7f9-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="9f7f9-113">Bazı ayarların kuruluş tarafından gizlenmiş veya yönetilen bir ileti (kırmızı renkle) olduğunu ve tüm seçeneklerin gri renkte olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Güncelleştirmelerin nasıl teslim edileceklerini seçin sayfası ayarların kuruluş tarafından gizlendi veya yönetiliyor olduğunu gösterir.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="9f7f9-115">Güvenlik Merkezi'Windows Defender açmak için Ayarlar Güvenliği **güncelleştir'e Windows Defender** Windows Defender Merkezi Virüs iş parçacığı koruması Virüs tehdit koruması ayarlarını \> **&amp;** \>  \>  \> **&amp;** \> **&amp; aç'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="9f7f9-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="9f7f9-116">Tüm seçeneklerin gri renkte olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="9f7f9-116">Verify that all options are grayed out.</span></span> 
    
    ![Virüs ve tehdit koruması ayarları gri görünür.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="9f7f9-118">İlgili Konular</span><span class="sxs-lookup"><span data-stu-id="9f7f9-118">Related Topics</span></span>

[<span data-ttu-id="9f7f9-119">Microsoft 365 belgeleri ve kaynakları için belgeler</span><span class="sxs-lookup"><span data-stu-id="9f7f9-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="9f7f9-120">Microsoft 365 İş ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="9f7f9-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="9f7f9-121">İşletmeler Microsoft 365 yönetme</span><span class="sxs-lookup"><span data-stu-id="9f7f9-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="9f7f9-122">Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="9f7f9-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
