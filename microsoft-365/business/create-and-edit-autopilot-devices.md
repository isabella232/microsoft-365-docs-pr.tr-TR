---
title: AutoPilot cihazlarını oluşturma ve düzenleme
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Microsoft 365 Business Premium'da Otomatik Pilot'u kullanarak cihazları nasıl yükleyin öğrenin. Bir aygıta veya aygıt grubuna profil atayabilirsiniz.
ms.openlocfilehash: 83c027cfe019e037518c4ca13eb331e5300fc2c1
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165871"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="123a3-104">AutoPilot cihazlarını oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="123a3-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="123a3-105">Cihaz listesini karşıya yükleme</span><span class="sxs-lookup"><span data-stu-id="123a3-105">Upload a list of devices</span></span>

<span data-ttu-id="123a3-106">Aygıtyüklemek için [adım adım kılavuzunu](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak **Aygıtlar** sekmesine aygıt yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="123a3-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="123a3-107">Aygıtlar bu gereksinimleri karşılamalıdır:</span><span class="sxs-lookup"><span data-stu-id="123a3-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="123a3-108">Windows 10, sürüm 1703 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="123a3-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="123a3-109">Windows'dan kutudan çıkma deneyiminden geçmemiş yeni aygıtlar</span><span class="sxs-lookup"><span data-stu-id="123a3-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="123a3-110">Microsoft 365 yönetici merkezinde, **Cihazlar** \> **Otomatik Pilot**seçin.</span><span class="sxs-lookup"><span data-stu-id="123a3-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="123a3-111">Otomatik **Pilot** sayfasında, **Aygıtlar** \> sekmesini seçin **aygıtlar ekle.**</span><span class="sxs-lookup"><span data-stu-id="123a3-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="123a3-113">Aygıt **ekle** panelinde, **Kaydet** \> **Kapat'ı**kaydet'i \> hazırladığınız [Aygıt listesi CSV dosyasına](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) göz atın.</span><span class="sxs-lookup"><span data-stu-id="123a3-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="123a3-114">Bu bilgileri donanım satıcınızdan alabilir veya Bir CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell komut dosyasını](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="123a3-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="123a3-115">Cihaza veya cihaz grubuna profil atama</span><span class="sxs-lookup"><span data-stu-id="123a3-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="123a3-116">**Windows'u Hazırla** sayfasında **Aygıtlar** sekmesini seçin ve bir veya daha fazla aygıtın yanındaki onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="123a3-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="123a3-117">**Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin.</span><span class="sxs-lookup"><span data-stu-id="123a3-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="123a3-118">Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="123a3-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
