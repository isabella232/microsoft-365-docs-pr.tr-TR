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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 aygıtları'nda bulunan Microsoft 365 iş app koruma ayarlarını doğrulamak öğrenin.
ms.openlocfilehash: 15c2d54c6281369875d15985c9d4ed16f0114176
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072250"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="1f78b-103">10 PC'lerde Windows aygıtı koruma ayarlarını doğrula</span><span class="sxs-lookup"><span data-stu-id="1f78b-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="1f78b-104">Windows 10 aygıt ilkeleri ayarlandığını doğrulayın</span><span class="sxs-lookup"><span data-stu-id="1f78b-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="1f78b-105">[Aygıtları ilkelerini kurun](protection-settings-for-windows-10-pcs.md)sonra onu ilkesi kullanıcıların aygıtları üzerinde etkili olması birkaç saat sürebilir.</span><span class="sxs-lookup"><span data-stu-id="1f78b-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="1f78b-106">İlkeleri kullanıcıların aygıtlarda çeşitli Windows ayarları ekranlar bakarak etkisi geçen onaylayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f78b-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="1f78b-107">Kullanıcılar Windows 10 aygıtlarında Windows Update ve Windows Defender virüsten koruma ayarlarını değiştirmek mümkün değildir çünkü bu seçenekleri bir sürü dışarı gri.</span><span class="sxs-lookup"><span data-stu-id="1f78b-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="1f78b-108">**Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **yeniden başlatma seçenekleri** ve tüm ayarları kullanıma gri olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="1f78b-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Yeniden başlatma seçenekleri, dışarı gri.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="1f78b-110">**Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **Gelişmiş Seçenekleri** ve tüm ayarları kullanıma gri olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="1f78b-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Windows Gelişmiş Seçenekler güncelleştirmeleri tüm nda.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="1f78b-112">**Ayarlar** Git \> **güncelleştirme &amp; güvenlik** \> **Windows Update** \> **Gelişmiş Seçenekler** \> **Seç güncelleştirmeleri nasıl dağıtılır**.</span><span class="sxs-lookup"><span data-stu-id="1f78b-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="1f78b-113">Gizli ya da kuruluşunuz tarafından yönetilen bazı ayarları ve seçenekleri nda iletide (kırmızı) görebilirsiniz onaylayın.</span><span class="sxs-lookup"><span data-stu-id="1f78b-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Güncelleştirmeleri nasıl dağıtılır seçin sayfa ayarları gizli veya kuruluşunuz tarafından yönetilen gösterir.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="1f78b-115">Windows Defender'ın Güvenlik Merkezi'ni açmak için **ayarları** ' na gidin \> **güncelleştirme &amp; güvenlik** \> **Windows Defender** \> **Windows Defender Güvenlik Merkezi'ni Aç** öğesini \> **virüs &amp; iş parçacığı koruma** \> **virüs &amp; iş parçacığı koruma ayarlarını**.</span><span class="sxs-lookup"><span data-stu-id="1f78b-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="1f78b-116">Out tüm seçenekler gri olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="1f78b-116">Verify that all options are greyed out.</span></span> 
    
    ![Virüs ve tehdit koruması ayarları nda.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="1f78b-118">İlgili Konular</span><span class="sxs-lookup"><span data-stu-id="1f78b-118">Related Topics</span></span>

[<span data-ttu-id="1f78b-119">Microsoft 365 İş belgeleri ve kaynakları</span><span class="sxs-lookup"><span data-stu-id="1f78b-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="1f78b-120">Microsoft 365 İş ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="1f78b-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="1f78b-121">Microsoft 365 İş yönetimi</span><span class="sxs-lookup"><span data-stu-id="1f78b-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="1f78b-122">Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="1f78b-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

