---
title: AutoPilot profillerini oluşturma ve düzenleme
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
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Bir Otomatik Pilot profili oluşturmayı ve bir aygıta uygulamayı, profili düzenlemeyi veya silmeyi veya bir profili aygıttan kaldırmayı öğrenin.
ms.openlocfilehash: e58418813ed0b4d23a5fa7e1d23aae33d8850e7f
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400984"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="36680-103">AutoPilot profillerini oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="36680-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="36680-104">Profil oluşturma</span><span class="sxs-lookup"><span data-stu-id="36680-104">Create a profile</span></span>

<span data-ttu-id="36680-105">Profiller bir cihaza veya cihaz grubuna uygulanır,</span><span class="sxs-lookup"><span data-stu-id="36680-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="36680-106">Microsoft 365 yönetici merkezinde, **Cihazlar** \> **Otomatik Pilot**seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="36680-107">Otomatik **Pilot** sayfasında **Profiller** sekmesini seçin \> **profil oluştur.**</span><span class="sxs-lookup"><span data-stu-id="36680-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="36680-108">Profil **Oluştur** sayfasında, profilin kimliğini belirlemenize yardımcı olacak bir ad girin, örneğin Pazarlama.</span><span class="sxs-lookup"><span data-stu-id="36680-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="36680-109">İstediğiniz ayarı açın ve sonra **Kaydet'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="36680-110">Otomatik Pilot profil ayarları hakkında daha fazla bilgi [için, Otomatik Pilot Profil ayarları hakkında](autopilot-profile-settings.md)bakın.</span><span class="sxs-lookup"><span data-stu-id="36680-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="36680-112">Cihaza profil uygulama</span><span class="sxs-lookup"><span data-stu-id="36680-112">Apply profile to a device</span></span>

<span data-ttu-id="36680-113">Bir profil oluşturduktan sonra, profili bir aygıta veya aygıt grubuna uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="36680-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="36680-114">[Adım adım kılavuzda](add-autopilot-devices-and-profile.md) varolan bir profili seçebilir ve yeni aygıtlara uygulayabilir veya aygıt veya aygıt grubu için varolan profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="36680-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="36680-115">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="36680-116">Aygıt adının yanındaki onay kutusunu seçin ve **Aygıt** panelinde, **Atanan profil** açılır listesinden bir profil seçin \> **Kaydet**.</span><span class="sxs-lookup"><span data-stu-id="36680-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="36680-118">Profili düzenleme, silme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="36680-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="36680-p103">Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir.</span><span class="sxs-lookup"><span data-stu-id="36680-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="36680-122">Profili düzenleme</span><span class="sxs-lookup"><span data-stu-id="36680-122">Edit a profile</span></span>

1. <span data-ttu-id="36680-123">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="36680-124">Bir aygıt adının yanındaki onay kutusunu seçin ve **Profil** panelinde kullanılabilir ayarlardan herhangi birini \> **kaydet'i**güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="36680-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="36680-125">Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.</span><span class="sxs-lookup"><span data-stu-id="36680-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="36680-126">Profili silme</span><span class="sxs-lookup"><span data-stu-id="36680-126">Delete a profile</span></span>

1. <span data-ttu-id="36680-127">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="36680-128">Aygıt adının yanındaki onay kutusunu seçin ve **Profil** panelinde **Profili** \> **Sil'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="36680-129">Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="36680-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="36680-130">Profili kaldırma</span><span class="sxs-lookup"><span data-stu-id="36680-130">Remove a profile</span></span>

1. <span data-ttu-id="36680-131">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="36680-132">Aygıt adının yanındaki onay kutusunu seçin ve **Aygıt** panelinde **Atanan profil** açılır listesinden **Kaydet'i** yok'u \> **Save**seçin.</span><span class="sxs-lookup"><span data-stu-id="36680-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
