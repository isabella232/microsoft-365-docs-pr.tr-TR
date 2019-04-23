---
title: AutoPilot cihazlarını oluşturma ve düzenleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: 365 işletmede AutoPilot kullanan aygıtları yüklemek nasıl öğrenin. Bir aygıt ya da aygıt grubu için bir profil atayabilirsiniz.
ms.openlocfilehash: fff2dbc6af45ef9d4189f23849d638172c19dfb2
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277085"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="d1f8a-104">AutoPilot cihazlarını oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="d1f8a-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="d1f8a-105">Cihaz listesini karşıya yükleme</span><span class="sxs-lookup"><span data-stu-id="d1f8a-105">Upload a list of devices</span></span>

<span data-ttu-id="d1f8a-106">Cihazları karşıya yüklemek için [Adım adım kılavuzu](add-autopilot-devices-and-profile.md) kullanabileceğiniz gibi, **Cihazlar** sekmesinde de karşıya yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="d1f8a-107">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="d1f8a-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="d1f8a-108">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="d1f8a-109">Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="d1f8a-110">Microsoft 365 iş Yönetim Merkezi'nde **cihaz** seçmenizi \> **AutoPilot** \> **Ekle**.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot** \> **Add**.</span></span>
  
2. <span data-ttu-id="d1f8a-111">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesi \> **Cihaz ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-111">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="d1f8a-113">Hazırladığınız bir [aygıt listesi CSV dosyası](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) **Ekle aygıtları** panelde göz \> **kaydetmek** \> **Kapat**.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="d1f8a-114">Bu bilgileri donanım satıcınızdan alabilir veya csv dosyasını oluşturmak için [Get-WindowsAutoPilotInfo PowerShell betiğini](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="d1f8a-115">Cihaza veya cihaz grubuna profil atama</span><span class="sxs-lookup"><span data-stu-id="d1f8a-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="d1f8a-116">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin ve bir veya birden çok cihazın yanındaki onay kutusunu işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="d1f8a-117">**Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin.</span><span class="sxs-lookup"><span data-stu-id="d1f8a-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="d1f8a-118">Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="d1f8a-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
