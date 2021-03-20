---
title: Windows 10 cihazları için uygulama koruma ayarlarını düzenleme veya ayarlama
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Kullanıcılarınızı kişisel Windows 10 cihazlarında uygulama yönetimi ilkelerini oluşturma veya düzenlemeyi ve iş dosyalarını korumayı öğrenin.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912832"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="f2a86-103">Windows 10 cihazları için uygulama koruma ayarlarını ayarlama veya düzenleme</span><span class="sxs-lookup"><span data-stu-id="f2a86-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="f2a86-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="f2a86-105">Windows 10 için uygulama yönetimi ilkesi düzenleme</span><span class="sxs-lookup"><span data-stu-id="f2a86-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="f2a86-106">Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin:</span><span class="sxs-lookup"><span data-stu-id="f2a86-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="f2a86-107">Sol gezintide Cihaz **İlkeleri'ne** \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="f2a86-108">Var olan bir Windows uygulama ilkesi seçin ve ardından **Düzenle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="f2a86-109">Değiştirmek **istediğiniz** ayarın yanındaki Düzenle'yi ve ardından Kaydet'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="f2a86-110">Windows 10 için uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="f2a86-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="f2a86-111">Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2a86-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="f2a86-112">Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin:</span><span class="sxs-lookup"><span data-stu-id="f2a86-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="f2a86-113">Sol gezintide Cihaz **İlkeleri** \> **Ekle'yi** \> **seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="f2a86-114">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="f2a86-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="f2a86-115">**İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="f2a86-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="f2a86-116">Cihaz **türü altında,** Kişisel'i **veya Şirkete** **Ait'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="f2a86-117">**İş dosyalarını şifrele** seçeneği otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="f2a86-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="f2a86-118">Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="f2a86-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="f2a86-119">**Windows cihazlarda Verileri kurtar'ı genişletin.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="f2a86-120">Bu açmanizi **öneririz.**</span><span class="sxs-lookup"><span data-stu-id="f2a86-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="f2a86-121">Veri Kurtarma Aracısı sertifikasının bulunduğu konuma göz atmadan önce bir sertifika oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="f2a86-122">Yönergeler için, Şifreleme [Dosyası Sistemi (EFS)](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)Veri Kurtarma Aracısı (DRA) sertifikası oluşturma ve doğrulama.</span><span class="sxs-lookup"><span data-stu-id="f2a86-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="f2a86-123">Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="f2a86-124">Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="f2a86-125">Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="f2a86-126">Yönetici, dosyanın şifresini çözmek için Veri Kurtarma Aracısı (DRA) sertifikasını kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="f2a86-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="f2a86-128">Listelenen **tüm uygulamalardaki dosyaların** korun olduğundan emin olmak için ek etki alanları veya SharePoint Online konumları eklemek için Ek ağ ve bulut konumlarını koru'ya genişletin.</span><span class="sxs-lookup"><span data-stu-id="f2a86-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="f2a86-129">Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın.</span><span class="sxs-lookup"><span data-stu-id="f2a86-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="f2a86-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="f2a86-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="f2a86-133">Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="f2a86-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>