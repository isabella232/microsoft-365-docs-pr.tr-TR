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
description: İş uygulaması koruma ayarları için Microsoft 365'in kullanıcılarınızın Windows 10 aygıtlarında etkili olduğunu nasıl doğrulayabilirsiniz öğrenin.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403600"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="418a7-103">Windows 10 bilgisayarlarında aygıt koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="418a7-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="418a7-104">Windows 10 aygıt ilkelerinin ayarlı olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="418a7-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="418a7-105">[Aygıtlar ilkelerini ayarladıktan](protection-settings-for-windows-10-pcs.md)sonra, ilkenin kullanıcıların aygıtları üzerinde etkili olması birkaç saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="418a7-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="418a7-106">Kullanıcıların cihazlarındaki çeşitli Windows Ayarları ekranlarına bakarak ilkelerin etkili olduğunu doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="418a7-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="418a7-107">Kullanıcılar Windows 10 cihazlarında Windows Update ve Windows Defender Antivirus ayarlarını değiştiremeyeceğinden, birçok seçenek gri renkte olacaktır.</span><span class="sxs-lookup"><span data-stu-id="418a7-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="418a7-108">Ayarlar **Settings** \> **Güvenlik &amp; Güncelleştirme** Windows \> **Update** Yeniden \> **Başlatma seçeneklerine** gidin ve tüm ayarların gri renkte olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="418a7-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Tüm Yeniden Başlatma seçenekleri gri renkte.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="418a7-110">Ayarlar **Settings** \> **Güvenlik &amp; Güncelleştirme** Windows \> **Update** \> **Gelişmiş seçeneklerine** gidin ve tüm ayarların gri renkte olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="418a7-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows Advanced güncelleştirmeleri seçeneklerinin tümü gri renktedir.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="418a7-112">**Ayarlar** Güncelleştirme \> \*\* &amp; güvenliğiwindows\*\* \> **update** \> **Gelişmiş seçeneklerine** gidin \> **Güncelleştirmelerin nasıl teslim edilebildiğini seçin.**</span><span class="sxs-lookup"><span data-stu-id="418a7-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="418a7-113">Bazı ayarların kuruluşunuz tarafından gizlendiğini veya yönetildiğini ve tüm seçeneklerin gri renkte olduğunu iletisini (kırmızı renkte) görebileceğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="418a7-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Ayarların kuruluşunuz tarafından gizlenip yönetildiğini belirten sayfanın nasıl teslim edileceğini seçin.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="418a7-115">Windows Defender Güvenlik Merkezi'ni açmak için **Ayarlar** \> **Güncelleştirme &amp; güvenlik** \> **Windows Defender'a** gidin Windows Defender Güvenlik Merkezi Virüs iş parçacığı \> koruması virüs tehdit koruma **Open Windows Defender Security Center** \> \*\* &amp; \*\* \> \*\* &amp; ayarlarını\*\*açın' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="418a7-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="418a7-116">Tüm seçeneklerin gri renkte olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="418a7-116">Verify that all options are grayed out.</span></span> 
    
    ![Virüs ve tehdit koruma ayarları gri.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="418a7-118">İlgili Konular</span><span class="sxs-lookup"><span data-stu-id="418a7-118">Related Topics</span></span>

[<span data-ttu-id="418a7-119">İş belgeleri ve kaynakları için Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="418a7-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="418a7-120">İşletmeler için Microsoft 365 ile başlayın</span><span class="sxs-lookup"><span data-stu-id="418a7-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="418a7-121">İşletmeler için Microsoft 365'i yönetin</span><span class="sxs-lookup"><span data-stu-id="418a7-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="418a7-122">Windows 10 bilgisayarlarında cihaz yapılandırmalarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="418a7-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

