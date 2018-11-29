---
title: AutoPilot profillerini oluşturma ve düzenleme
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Oluşturmak, düzenlemek, silmek veya kaldırmak AutoPilot profilleri hakkında bilgi edinin. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983140"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="96de0-103">AutoPilot profillerini oluşturma ve düzenleme</span><span class="sxs-lookup"><span data-stu-id="96de0-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="96de0-104">Profil oluşturma</span><span class="sxs-lookup"><span data-stu-id="96de0-104">Create a profile</span></span>

<span data-ttu-id="96de0-105">Profiller bir cihaza veya cihaz grubuna uygulanır,</span><span class="sxs-lookup"><span data-stu-id="96de0-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="96de0-106">Microsoft 365 İş Yönetim merkezinde **Cihaz eylemleri** kartında **Windows'u AutoPilot ile Dağıt**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="96de0-108">**Windows'u Hazırla** sayfasında **Profiller** sekmesi \> **Profil oluştur**'u seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="96de0-109">**Profil oluştur** sayfasında, profili tanımanıza yardımcı olacak bir ad (örneğin, Pazarlama) girin, istediğiniz ayarı açın (daha fazla bilgi edinmek için bkz. [AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md)) ve **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="96de0-111">Cihaza profil uygulama</span><span class="sxs-lookup"><span data-stu-id="96de0-111">Apply profile to a device</span></span>

<span data-ttu-id="96de0-p101">Profili oluşturduktan sonra bir cihaza veya cihaz grubuna uygulayabilirsiniz. [Adım adım kılavuzdan](add-autopilot-devices-and-profile.md) mevcut bir profili seçip yeni cihazlara uygulayabilir ya da bir cihaza veya cihaz grubuna yönelik mevcut bir profili değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="96de0-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="96de0-114">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="96de0-115">Onay kutusunu aygıt adının yanındaki ve **Aygıt** Bölmesi'ni tıklatın, **atanan profil** açılan listesinden bir profil seçin \> **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="96de0-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="96de0-117">Profili düzenleme, silme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="96de0-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="96de0-p102">Bir profili bir cihaza atadıktan sonra, cihazı daha önce bir kullanıcıya vermiş olsanız bile profili güncelleştirebilirsiniz. Cihaz İnternet'e bağlandığında, kurulum sırasında profilinizin en son sürümünü indirir. Kullanıcı cihazı varsayılan fabrika ayarlarına sıfırladığında da cihaz, profilinize yönelik en son güncelleştirmeleri indirir.</span><span class="sxs-lookup"><span data-stu-id="96de0-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="96de0-121">Profili düzenleme</span><span class="sxs-lookup"><span data-stu-id="96de0-121">Edit a profile</span></span>

1. <span data-ttu-id="96de0-122">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="96de0-123">Aygıt adının yanındaki onay kutusunu tıklatın ve **Profil** paneli kullanılabilir ayarlarını güncelleştirmek \> **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="96de0-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="96de0-124">Bunu cihaz bir kullanıcı tarafından İnternet'e bağlanmadan önce gerçekleştirirseniz, profil kurulum işlemine uygulanır.</span><span class="sxs-lookup"><span data-stu-id="96de0-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="96de0-125">Profili silme</span><span class="sxs-lookup"><span data-stu-id="96de0-125">Delete a profile</span></span>

1. <span data-ttu-id="96de0-126">**Windows'u Hazırla** sayfasında **Profiller** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="96de0-127">Bir cihaz adının yanındaki onay kutusuna tıklayın ve **Profil** bölmesinden **Profili sil** \> **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="96de0-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="96de0-128">Silinen profiller, atanmış oldukları cihazdan veya cihaz grubundan kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="96de0-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="96de0-129">Profili kaldırma</span><span class="sxs-lookup"><span data-stu-id="96de0-129">Remove a profile</span></span>

1. <span data-ttu-id="96de0-130">**Windows'u Hazırla** sayfasında **Cihazlar** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="96de0-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="96de0-131">Onay kutusunu aygıt adının yanındaki ve **Aygıt** Bölmesi'ni tıklatın, **Hiçbiri** **atanmadı profil** açılan listesinden seçin \> **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="96de0-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
