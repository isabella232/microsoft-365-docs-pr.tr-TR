---
title: AutoPilot cihazlarını oluşturma ve düzenleme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Microsoft 365 İş Ekstra'da AutoPilot kullanarak cihazları karşıya yükleme hakkında bilgi edinebilirsiniz. Bir cihaza veya cihaz grubuna profil atabilirsiniz.
ms.openlocfilehash: 506ff44e3cb6656b19174e82688b5af141ea2b79
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578497"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="f3b19-104">AutoPilot cihazlarını oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="f3b19-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="f3b19-105">Cihaz listesini karşıya yükleme</span><span class="sxs-lookup"><span data-stu-id="f3b19-105">Upload a list of devices</span></span>

<span data-ttu-id="f3b19-106">Cihazları karşıya yüklemek [için Adım adım kılavuzu kullanabilirsiniz,](add-autopilot-devices-and-profile.md) ancak cihazlar sekmesinde cihazları da karşıya **yükleyebilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="f3b19-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="f3b19-107">Cihazlar şu gereksinimleri karşılamalıdır:</span><span class="sxs-lookup"><span data-stu-id="f3b19-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="f3b19-108">Windows 10, sürüm 1703 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="f3b19-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="f3b19-109">Windows'un ilk gelen deneyimine henüz sahip olmayan yeni cihazlar</span><span class="sxs-lookup"><span data-stu-id="f3b19-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="f3b19-110">Microsoft 365 yönetim merkezinde  Cihazlar \> **AutoPilot'u seçin.**</span><span class="sxs-lookup"><span data-stu-id="f3b19-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="f3b19-111">**AutoPilot sayfasında** Cihazlar sekmesi Cihaz  \> **ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="f3b19-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="f3b19-113">Cihaz ekle **panelinde,** Kaydet Kapat'ı hazır [bulundurarak hazır](../admin/misc/device-list.md) istediğiniz Cihaz listesi CSV \> **dosyasına** \> **göz atabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="f3b19-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="f3b19-114">Bu bilgileri donanım satıcıdan edinebilirsiniz veya CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) betiği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f3b19-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="f3b19-115">Cihaza veya cihaz grubuna profil atama</span><span class="sxs-lookup"><span data-stu-id="f3b19-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="f3b19-116">**Windows'u Hazırla** sayfasında Cihazlar sekmesini **seçin** ve bir veya birden çok cihaz yanındaki onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="f3b19-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="f3b19-117">**Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin.</span><span class="sxs-lookup"><span data-stu-id="f3b19-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="f3b19-118">Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="f3b19-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
