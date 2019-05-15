---
title: AutoPilot profillerini oluşturma ve düzenleme
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
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Oluşturmak, düzenlemek, silmek veya kaldırmak AutoPilot profilleri hakkında bilgi edinin. '
ms.openlocfilehash: 7987cafb3ea234d81be72c79aee8e584a3770875
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073500"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="9d5ac-103">AutoPilot profillerini oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="9d5ac-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="9d5ac-104">Profil oluşturma</span><span class="sxs-lookup"><span data-stu-id="9d5ac-104">Create a profile</span></span>

<span data-ttu-id="9d5ac-105">Profiller bir cihaza veya cihaz grubuna uygulanır,</span><span class="sxs-lookup"><span data-stu-id="9d5ac-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="9d5ac-106">Microsoft 365 iş Yönetim Merkezi'nde **cihaz** seçmenizi \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="9d5ac-107">**AutoPilot** sayfasında, **Profiller** sekmesini seçin \> **Profil Oluştur**.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="9d5ac-108">**Profil oluştur** sayfasında, profili tanımanıza yardımcı olacak bir ad (örneğin, Pazarlama) girin, istediğiniz ayarı açın (daha fazla bilgi edinmek için bkz. [AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md)) ve **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="9d5ac-110">Cihaza profil uygulama</span><span class="sxs-lookup"><span data-stu-id="9d5ac-110">Apply profile to a device</span></span>

<span data-ttu-id="9d5ac-p101">Profili oluşturduktan sonra bir cihaza veya cihaz grubuna uygulayabilirsiniz. [Adım adım kılavuzdan](add-autopilot-devices-and-profile.md) mevcut bir profili seçip yeni cihazlara uygulayabilir ya da bir cihaza veya cihaz grubuna yönelik mevcut bir profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="9d5ac-113">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9d5ac-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="9d5ac-116">Profili düzenleme, silme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="9d5ac-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="9d5ac-p102">Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="9d5ac-120">Profili düzenleme</span><span class="sxs-lookup"><span data-stu-id="9d5ac-120">Edit a profile</span></span>

1. <span data-ttu-id="9d5ac-121">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9d5ac-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="9d5ac-123">Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="9d5ac-124">Profili silme</span><span class="sxs-lookup"><span data-stu-id="9d5ac-124">Delete a profile</span></span>

1. <span data-ttu-id="9d5ac-125">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9d5ac-126">Bir cihaz adının yanındaki onay kutusuna tıklayın ve **Profil** bölmesinden **Profili sil** \> **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="9d5ac-127">Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="9d5ac-128">Profili kaldırma</span><span class="sxs-lookup"><span data-stu-id="9d5ac-128">Remove a profile</span></span>

1. <span data-ttu-id="9d5ac-129">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9d5ac-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="9d5ac-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
