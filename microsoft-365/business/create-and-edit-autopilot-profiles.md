---
title: AutoPilot profillerini oluşturma ve düzenleme
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: AutoPilot profilini oluşturma ve bir cihaza uygulamanın yanı sıra profili düzenlemeyi veya silmeyi veya cihazdan profili kaldırmayı öğrenin.
ms.openlocfilehash: 414243da88fb6f39f8e6067d19d49ffe955f725f
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580264"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="2b001-103">AutoPilot profillerini oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="2b001-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="2b001-104">Profil oluşturma</span><span class="sxs-lookup"><span data-stu-id="2b001-104">Create a profile</span></span>

<span data-ttu-id="2b001-105">Profiller bir cihaza veya cihaz grubuna uygulanır,</span><span class="sxs-lookup"><span data-stu-id="2b001-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="2b001-106">Microsoft 365 yönetim merkezinde  Cihazlar \> **AutoPilot'u seçin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="2b001-107">**AutoPilot sayfasında** Profil oluştur **sekmesini** \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="2b001-108">Profil **oluştur sayfasında,** profili tanımlamanıza yardımcı olacak bir ad (örneğin, Pazarlama) girin.</span><span class="sxs-lookup"><span data-stu-id="2b001-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="2b001-109">Istediğiniz ayarı seçin ve kaydet'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="2b001-110">AutoPilot profil ayarları hakkında daha fazla bilgi için bkz. [AutoPilot Profili ayarları hakkında.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="2b001-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="2b001-112">Cihaza profil uygulama</span><span class="sxs-lookup"><span data-stu-id="2b001-112">Apply profile to a device</span></span>

<span data-ttu-id="2b001-113">Profili oluşturdukta, bir cihaza veya cihaz grubuna uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2b001-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="2b001-114">Adım adım kılavuzda mevcut [](add-autopilot-devices-and-profile.md) bir profili seçerek yeni cihazlara uygulayabilir veya bir cihaz ya da cihaz grubu için mevcut profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2b001-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="2b001-115">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="2b001-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="2b001-116">Cihaz adının yanındaki onay kutusunu seçin ve  Cihaz panelinde Atanan profil açılan listesinden **bir** profil \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="2b001-118">Profili düzenleme, silme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="2b001-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="2b001-p103">Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir.</span><span class="sxs-lookup"><span data-stu-id="2b001-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="2b001-122">Profili düzenleme</span><span class="sxs-lookup"><span data-stu-id="2b001-122">Edit a profile</span></span>

1. <span data-ttu-id="2b001-123">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="2b001-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="2b001-124">Cihaz adının yanındaki onay kutusunu seçin ve Profil panelinde, **kullanılabilir** Kaydet ayarlarından herhangi birini \> **güncelleştirin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="2b001-125">Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.</span><span class="sxs-lookup"><span data-stu-id="2b001-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="2b001-126">Profili silme</span><span class="sxs-lookup"><span data-stu-id="2b001-126">Delete a profile</span></span>

1. <span data-ttu-id="2b001-127">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="2b001-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="2b001-128">Cihaz adının yanındaki onay kutusunu seçin ve  Profil panelinde Profil Kaydet'i **sil'i** \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="2b001-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="2b001-129">Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="2b001-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="2b001-130">Profili kaldırma</span><span class="sxs-lookup"><span data-stu-id="2b001-130">Remove a profile</span></span>

1. <span data-ttu-id="2b001-131">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="2b001-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="2b001-132">Cihaz adının yanındaki onay kutusunu seçin ve  Cihaz panelinde Atanan  profil **açılan** listesinde Kaydet'i \> seçin.</span><span class="sxs-lookup"><span data-stu-id="2b001-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
