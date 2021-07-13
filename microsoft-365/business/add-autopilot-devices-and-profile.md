---
title: AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: AutoPilot'Windows kullanabileceğiniz ve iş için Windows 10 kullanıma hazır olacak şekilde yeni cihaz ayarlamayı öğrenin.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393449"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="6de5d-103">AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.</span><span class="sxs-lookup"><span data-stu-id="6de5d-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="6de5d-104">Windows AutoPilot Windows 10 u kullanarak  işletmenize uygun yeni cihaz ve cihazları çalışanlarınıza verirken kullanıma hazır hale kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="6de5d-105">Cihaz gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="6de5d-105">Device requirements</span></span>

<span data-ttu-id="6de5d-106">Cihazlar şu gereksinimleri karşılamalıdır:</span><span class="sxs-lookup"><span data-stu-id="6de5d-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="6de5d-107">Windows 10, sürüm 1703 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="6de5d-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="6de5d-108">Henüz ilk ve en son Windows yeni cihazlar</span><span class="sxs-lookup"><span data-stu-id="6de5d-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="6de5d-109">Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma</span><span class="sxs-lookup"><span data-stu-id="6de5d-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="6de5d-110">Henüz cihaz grupları veya profil oluşturmadıysanız, başlamanın en iyi yolu adım adım kılavuzu kullanmaktır.</span><span class="sxs-lookup"><span data-stu-id="6de5d-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="6de5d-111">Ayrıca, kılavuzu [kullanmadan](create-and-edit-autopilot-devices.md) [cihazlar ekleyebilir ve](create-and-edit-autopilot-profiles.md) onlara profil atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="6de5d-112">yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin.</span><span class="sxs-lookup"><span data-stu-id="6de5d-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="6de5d-113">Sol gezinti bölmesinde Cihazlar  \> **AutoPilot'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="6de5d-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Yönetim merkezinde cihazlar'ı ve ardından AutoPilot'ı seçin.](../media/AutoPilot.png)
  
2. <span data-ttu-id="6de5d-115">**AutoPilot sayfasında Kılavuzu** başlat'a tıklayın **veya dokunun.**</span><span class="sxs-lookup"><span data-stu-id="6de5d-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="6de5d-117">Cihaz **Upload .csv listesinin bulunduğu dosyada,** dosyanın hazır bulunduğu konuma gidin ve .CSV **Aç'ı** \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="6de5d-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="6de5d-118">Dosyada üç üst bilgi olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="6de5d-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="6de5d-119">A sütunu: Cihaz Seri Numarası</span><span class="sxs-lookup"><span data-stu-id="6de5d-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="6de5d-120">B sütunu: Windows Ürün Kimliği</span><span class="sxs-lookup"><span data-stu-id="6de5d-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="6de5d-121">C sütunu: Donanım Numarası</span><span class="sxs-lookup"><span data-stu-id="6de5d-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="6de5d-122">Bu bilgileri donanım satıcıdan edinebilirsiniz veya CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) betiği kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="6de5d-p103">Daha fazla bilgi için bkz. [Cihaz listesi CSV dosyası](../admin/misc/device-list.md). **Cihaz listesiyle .csv dosyası yükleme** sayfasında bir örnek dosya da indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6de5d-125">Bu betikte, müşterinin cihazı AutoPilot'a kaydetmesi için gereken özellikleri almak Windows kullanılır.</span><span class="sxs-lookup"><span data-stu-id="6de5d-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="6de5d-126">Sonuçta elde edilen CSV dosyasının BIR Windows Ürün Kimliği (PKID) değeri toplamamalerinin normal olduğunu, çünkü bir cihazı kaydetmek için bu değerin gerekli olmadığını ve PKID'nin CSV çıktısinde NULL olması tamamen sorun olmadığını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="6de5d-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="6de5d-127">Yalnızca seri numarası ve donanım karması doldurulur.</span><span class="sxs-lookup"><span data-stu-id="6de5d-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="6de5d-128">Profil **atama sayfasında** mevcut bir profili seçebilirsiniz veya yeni bir profil oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="6de5d-129">Henüz bir tane yoksa, oluşturmak için bir hesap oluşturmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="6de5d-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="6de5d-130">Profil, tek bir cihaza veya bir cihaz grubuna uygulanabilen ayarlar koleksiyonudur.</span><span class="sxs-lookup"><span data-stu-id="6de5d-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="6de5d-131">Varsayılan özellikler gereklidir ve otomatik olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="6de5d-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="6de5d-132">Varsayılan özellikler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="6de5d-132">The default features are:</span></span>
    
    - <span data-ttu-id="6de5d-133">OEM Cortana, OneDrive kaydı atlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6de5d-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="6de5d-134">Şirketinizin markasıyla oturum açma deneyimi oluşturma.</span><span class="sxs-lookup"><span data-stu-id="6de5d-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="6de5d-135">Bağlan hesaplarınıza Azure Active Directory ve sizin tarafından yönetilleri için otomatik olarak Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="6de5d-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="6de5d-136">Daha fazla bilgi için [bkz. AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="6de5d-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="6de5d-137">Diğer ayarlar, **Gizlilik ayarlarını atla** ve **Kullanıcının yerel yönetici olmasına izin verme** şeklindedir. Varsayılan olarak ikisi de **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="6de5d-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="6de5d-138">**İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6de5d-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="6de5d-139">**Hepsi bu kadar,** oluşturduğunuz (veya seçtiğiniz) profilin, cihaz listesini yükerek oluşturduğunuz cihaz grubuna uygulanıyor olduğu gösterir.</span><span class="sxs-lookup"><span data-stu-id="6de5d-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="6de5d-140">Ayarlar, cihaz kullanıcıları bir sonraki oturum açmada etkili olur.</span><span class="sxs-lookup"><span data-stu-id="6de5d-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="6de5d-141">**Kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6de5d-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="6de5d-142">İlgili içerik</span><span class="sxs-lookup"><span data-stu-id="6de5d-142">Related content</span></span>

<span data-ttu-id="6de5d-143">[AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md) (makale)</span><span class="sxs-lookup"><span data-stu-id="6de5d-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="6de5d-144">[Cihazlarınızı ve uygulama verilerinizi koruma seçenekleri](../admin/devices/choose-device-security.md) (makale)</span><span class="sxs-lookup"><span data-stu-id="6de5d-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>
