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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 cihazlarında Microsoft 365 İş uygulaması koruma ayarlarını nasıl doğrulayayarılamayı öğrenin.
ms.openlocfilehash: 66e83df19e44419b37bcc1c5678ab13317162dbc
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288605"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="b746d-103">Windows 10 bilgisayarlarında aygıt koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="b746d-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="b746d-104">Windows 10 aygıt ilkelerinin ayarlı olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="b746d-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="b746d-105">[Aygıtlar ilkelerini ayarladıktan](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcıların aygıtları üzerinde etkili olması birkaç saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="b746d-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="b746d-106">Kullanıcıların cihazlarındaki çeşitli Windows Ayarları ekranlarına bakarak ilkelerin etkili olduğunu doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b746d-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="b746d-107">Kullanıcılar Windows 10 cihazlarında Windows Update ve Windows Defender Antivirus ayarlarını değiştiremeyeceklerinden, bu seçeneklerin çoğu soluklanır.</span><span class="sxs-lookup"><span data-stu-id="b746d-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="b746d-108">**Ayarlar** \> **Güvenlik &amp; Güncelleştirme** \> **Windows Update** \> **Yeniden Başlatma seçeneklerine** gidin ve tüm ayarların soluk olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="b746d-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Tüm Yeniden Başlatma seçenekleri soluk.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="b746d-110">**Ayarlar** \> **Güvenlik &amp; Güncelleştirme** \> **Windows Update** \> **Gelişmiş seçeneklerine** gidin ve tüm ayarların soluk olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="b746d-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Windows Advanced güncelleştirmeleri seçeneklerinin tümü soluk.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="b746d-112">**Ayarlar** \> Güncelleştirme \> **güvenliğiwindows** \> \*\*update &amp; \*\* **Gelişmiş seçeneklerine** \> gidin **Güncelleştirmelerin nasıl teslim edilebildiğini seçin.**</span><span class="sxs-lookup"><span data-stu-id="b746d-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="b746d-113">Bazı ayarların kuruluşunuz tarafından gizlendiğini veya yönetildiğini ve tüm seçeneklerin soluk olarak dağıtıladığını iletiyi (kırmızı renkte) görebileceğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b746d-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Ayarların kuruluşunuz tarafından gizlenip yönetildiğini belirten sayfanın nasıl teslim edileceğini seçin.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="b746d-115">Windows Defender Güvenlik Merkezi'ni açmak için **Ayarlar** \> **Güncelleştirme &amp; güvenlik** \> **Windows Defender'a** \> gidin Windows Defender Güvenlik Merkezi \> Virüs \*\*\*\* \*\* &amp; iş parçacığı aç'ı tıklatın koruma\*\* \> \*\* &amp; Virüs tehdit koruma ayarları\*\*.</span><span class="sxs-lookup"><span data-stu-id="b746d-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="b746d-116">Tüm seçeneklerin soluk olduğundan doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="b746d-116">Verify that all options are greyed out.</span></span> 
    
    ![Virüs ve tehdit koruma ayarları soluk.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="b746d-118">İlgili Konular</span><span class="sxs-lookup"><span data-stu-id="b746d-118">Related Topics</span></span>

[<span data-ttu-id="b746d-119">Microsoft 365 İş belgeleri ve kaynakları</span><span class="sxs-lookup"><span data-stu-id="b746d-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="b746d-120">Microsoft 365 İş ile çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="b746d-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="b746d-121">Microsoft 365 İş yönetimi</span><span class="sxs-lookup"><span data-stu-id="b746d-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="b746d-122">Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="b746d-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

