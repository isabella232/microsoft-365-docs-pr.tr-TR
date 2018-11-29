---
title: AutoPilot cihazlarını oluşturma ve düzenleme
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: 365 işletmede AutoPilot kullanan aygıtları yüklemek nasıl öğrenin. Bir aygıt ya da aygıt grubu için bir profil atayabilirsiniz.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982940"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="19088-104">AutoPilot cihazlarını oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="19088-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="19088-105">Cihaz listesini karşıya yükleme</span><span class="sxs-lookup"><span data-stu-id="19088-105">Upload a list of devices</span></span>

<span data-ttu-id="19088-106">Cihazları karşıya yüklemek için [Adım adım kılavuzu](add-autopilot-devices-and-profile.md) kullanabileceğiniz gibi, **Cihazlar** sekmesinde de karşıya yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="19088-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="19088-107">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="19088-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="19088-108">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="19088-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="19088-109">Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.</span><span class="sxs-lookup"><span data-stu-id="19088-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="19088-110">Microsoft 365 İş Yönetim merkezinde **Cihaz eylemleri** kartında **Windows'u AutoPilot ile Dağıt**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="19088-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="19088-112">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesi \> **Cihaz ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="19088-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="19088-114">Hazırladığınız bir [aygıt listesi CSV dosyası](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) **Ekle aygıtları** panelde göz \> **kaydetmek** \> **Kapat**.</span><span class="sxs-lookup"><span data-stu-id="19088-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="19088-115">Bu bilgileri donanım satıcınızdan alabilir veya csv dosyasını oluşturmak için [Get-WindowsAutoPilotInfo PowerShell betiğini](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="19088-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="19088-116">Cihaza veya cihaz grubuna profil atama</span><span class="sxs-lookup"><span data-stu-id="19088-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="19088-117">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin ve bir veya birden çok cihazın yanındaki onay kutusunu işaretleyin.</span><span class="sxs-lookup"><span data-stu-id="19088-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="19088-118">**Cihaz** panelinde, **Atanan profil** açılan listesinden bir profil seçin.</span><span class="sxs-lookup"><span data-stu-id="19088-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="19088-119">Henüz hiç profiliniz yoksa, yönergeler için bkz. [AutoPilot profillerini oluşturma ve düzenleme](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="19088-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
