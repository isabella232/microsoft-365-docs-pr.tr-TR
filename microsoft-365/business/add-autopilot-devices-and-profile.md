---
title: AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: İşletmeniz için yeni Windows 10 aygıtları kurmak için Windows AutoPilot kullanmayı öğrenin.
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660699"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="0f33f-103">AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.</span><span class="sxs-lookup"><span data-stu-id="0f33f-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="0f33f-104">Windows AutoPilot, çalışanlarınıza vermediğiniz sürece bunlar üretken kullanılmak üzere hazır olacak şekilde işletmeniz için **Yeni** Windows 10 aygıtları belirlemek için kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0f33f-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="0f33f-105">Cihaz gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="0f33f-105">Device requirements</span></span>

<span data-ttu-id="0f33f-106">Cihazların şu gereksinimleri karşılaması gerekir:</span><span class="sxs-lookup"><span data-stu-id="0f33f-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="0f33f-107">Windows 10, sürüm 1703 veya üstü.</span><span class="sxs-lookup"><span data-stu-id="0f33f-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="0f33f-108">Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.</span><span class="sxs-lookup"><span data-stu-id="0f33f-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="0f33f-109">Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma</span><span class="sxs-lookup"><span data-stu-id="0f33f-109">Use the setup guide to create devices and profiles</span></span>

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="0f33f-111">Henüz cihaz grubu veya profil oluşturmadıysanız başlamanın en iyi yolu adım adım kılavuzu kullanmaktır. Bununla birlikte, kılavuzu kullanmadan da [cihaz ekleyebilir](create-and-edit-autopilot-devices.md) ve bu cihazlara [profil atayabilirsiniz](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="0f33f-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="0f33f-112">Yönetim merkezinde mi <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="0f33f-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="0f33f-113">**Aygıtlar** üzerinde sol nav seçin \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="0f33f-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![Yönetim Merkezi'nde aygıtları ve AutoPilot seçin.](media/AutoPilot.png)
  
2. <span data-ttu-id="0f33f-115">**AutoPilot** sayfasında **Kılavuzu Başlat**' a dokunun veya tıklatın.</span><span class="sxs-lookup"><span data-stu-id="0f33f-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="0f33f-p101">**Cihaz listesiyle .csv dosyası yükleme** sayfasında, .CSV dosyanızın hazır bulunduğu konuma gidin ve sonra **Aç** \> **İleri**'yi seçin. Dosyada üç üst bilgi olmalıdır:</span><span class="sxs-lookup"><span data-stu-id="0f33f-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="0f33f-119">A sütunu: Cihaz Seri Numarası</span><span class="sxs-lookup"><span data-stu-id="0f33f-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="0f33f-120">B sütunu: Windows Ürün Kimliği</span><span class="sxs-lookup"><span data-stu-id="0f33f-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="0f33f-121">C sütunu: Donanım Numarası</span><span class="sxs-lookup"><span data-stu-id="0f33f-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="0f33f-122">Bu bilgileri donanım satıcınızdan edinebilir veya CSV dosyasını oluşturmak için [Get-WindowsAutoPilotInfo PowerShell betiğini](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0f33f-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="0f33f-p102">Daha fazla bilgi için bkz. [Cihaz listesi CSV dosyası](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). **Cihaz listesiyle .csv dosyası yükleme** sayfasında bir örnek dosya da indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0f33f-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="0f33f-p103">**Profil atama** sayfasında mevcut bir profili seçebilir veya yeni bir profil oluşturabilirsiniz. Henüz profiliniz yoksa yenisini oluşturmanız istenir.</span><span class="sxs-lookup"><span data-stu-id="0f33f-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="0f33f-127">Profil, tek bir cihaza veya bir cihaz grubuna uygulanabilen ayarlar koleksiyonudur.</span><span class="sxs-lookup"><span data-stu-id="0f33f-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="0f33f-p104">Varsayılan özellikler gereklidir ve otomatik olarak ayarlanır. Varsayılan özellikler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="0f33f-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="0f33f-130">Cortana, OneDrive ve OEM kaydı atlanır.</span><span class="sxs-lookup"><span data-stu-id="0f33f-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="0f33f-131">Şirketinizin markasıyla oturum açma deneyimi oluşturma.</span><span class="sxs-lookup"><span data-stu-id="0f33f-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="0f33f-132">Cihazlarınız Azure Active Directory hesaplarına bağlanır ve Microsoft 365 İş tarafından yönetilmek üzere otomatik olarak kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="0f33f-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="0f33f-133">Daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="0f33f-133">For more information, see</span></span>
    
    <span data-ttu-id="0f33f-134">[AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="0f33f-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="0f33f-135">Diğer ayarlar, **Gizlilik ayarlarını atla** ve **Kullanıcının yerel yönetici olmasına izin verme** şeklindedir. Varsayılan olarak ikisi de **Kapalı** durumdadır.</span><span class="sxs-lookup"><span data-stu-id="0f33f-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="0f33f-136">**İleri**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="0f33f-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="0f33f-p105">**Hepsi bu kadar** sayfası oluşturduğunuz (veya seçtiğiniz) profilin, cihaz listesini yükleyerek oluşturduğunuz cihaz grubuna uygulanacağı anlamına gelir. Cihaz kullanıcıları bir daha oturum açtığında bu ayarlar geçerli olur. **Kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="0f33f-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    