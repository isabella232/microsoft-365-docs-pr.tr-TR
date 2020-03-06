---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 cihazlarında Microsoft 365 İş uygulaması koruma ayarlarını doğrulayın ve kullanıcıların şirket verilerini kişisel dosyalara veya yönetilmeyen uygulamalara kopyalayamayacağını doğrulayın.
ms.openlocfilehash: 4d3d7e950311ac32606e700ebb35bf026ae091cc
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550007"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="1f16f-103">Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="1f16f-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="1f16f-104">Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="1f16f-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="1f16f-105">[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir.</span><span class="sxs-lookup"><span data-stu-id="1f16f-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="1f16f-106">Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını Engelley'i **açtıysanız** ve iş dosyalarını şirkete ait cihazlar için İş için **OneDrive'a kaydetmeye zorladıysanız,** azure AD'ye bağlanıp oturum açtıktan sonra bunu kullanıcının aygıtında denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f16f-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="1f16f-107">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="1f16f-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="1f16f-p102">[Microsoft 365 İş kullanıcıları için Windows cihazlarını ayarlama](set-up-windows-devices.md) konusunda açıklandığı gibi Microsoft 365 İş kimlik bilgileriyle oturum açtıktan ve Azure AD'ye bağlandıktan sonra, **Windows Ayarları** \> **Hesaplar** \> **İş yeri veya okula eriş** seçeneğine gidin. **Bağlanılan \<kiracı adı\> Azure AD**'yi seçin ve sonra da **Bilgi**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="1f16f-111">\<Kiracı\> adı tarafından **yönetilen** sayfada, aşağıdaki şekilde gösterildiği gibi bir Yönetim **Sunucusu Adresi** içeren Bağlantı **bilgilerini** görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f16f-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="1f16f-113">**Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramayacağınızı doğrulayın**</span><span class="sxs-lookup"><span data-stu-id="1f16f-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="1f16f-114">Microsoft 365 İş tarafından yüklenmiş olan Outlook 2016'yı açın.</span><span class="sxs-lookup"><span data-stu-id="1f16f-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="1f16f-115">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="1f16f-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="1f16f-116">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="1f16f-117">Uygulamanın içeriğe erişemediğini belirten bir hata alırsınız.</span><span class="sxs-lookup"><span data-stu-id="1f16f-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="1f16f-119">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f16f-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="1f16f-120">Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="1f16f-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="1f16f-121">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="1f16f-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="1f16f-122">Yerel bir kullanıcı olarak oturum açtığınız Windows 10 kişisel cihazınızda **Windows Ayarları'na**gidin ve **HesaplarA** \> **Erişim çalışmasına veya okuluna**tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="1f16f-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="1f16f-123">**İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="1f16f-124">**İş yeri veya okul hesabı oluştur iletişim kutusu** \> **Oturum aç** için Microsoft 365 İş kimlik bilgilerinizi girin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="1f16f-125">**İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![İş veya okul hesabı iletişim kutusundaKi Bilgiler'i tıklatın veya dokunun.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="1f16f-127">Access **çalışmasında veya okul** sayfasında, aşağıdaki şekilde gösterildiği gibi bir **Yönetim Sunucusu Adresi** içeren ve içindeki *silme* ve *mam* sözcülerini içeren **Bağlantı bilgilerini** görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f16f-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="1f16f-129">**Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramayacağınızı doğrulayın**</span><span class="sxs-lookup"><span data-stu-id="1f16f-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="1f16f-130">Outlook 2016'yı açın, gerekirse Microsoft 365 İş hesabınızı ekleyin ve Microsoft 365 İş kimlik bilgilerinizle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="1f16f-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="1f16f-131">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="1f16f-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="1f16f-132">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="1f16f-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="1f16f-133">App'in içeriğe erişemediğini belirten bir hata alırsınız.</span><span class="sxs-lookup"><span data-stu-id="1f16f-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="1f16f-135">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1f16f-135">You can, however, paste the same content into Word 2016.</span></span>
    

