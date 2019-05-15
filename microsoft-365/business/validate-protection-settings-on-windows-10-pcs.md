---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 aygıtları'nda bulunan Microsoft 365 iş app koruma ayarlarını doğrulamak öğrenin.
ms.openlocfilehash: 7710accf9a3cd1db788dd5215ab6d7bbb97e48a6
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074390"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="d5c85-103">Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="d5c85-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="d5c85-104">Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="d5c85-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="d5c85-p101">[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir. Şirkete ait cihazlar için **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamalarını engelle ve iş dosyalarını OneDrive İş'e kaydetmelerini zorla** ayarını **Açık** duruma getirdiyseniz, kullanıcılar Azure AD'ye bağlanıp oturum açtıktan sonra bunu kullanıcının cihazında denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5c85-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="d5c85-107">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="d5c85-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="d5c85-p102">[Microsoft 365 İş kullanıcıları için Windows cihazlarını ayarlama](set-up-windows-devices.md) konusunda açıklandığı gibi Microsoft 365 İş kimlik bilgileriyle oturum açtıktan ve Azure AD'ye bağlandıktan sonra, **Windows Ayarları** \> **Hesaplar** \> **İş yeri veya okula eriş** seçeneğine gidin. **Bağlanılan \<kiracı adı\> Azure AD**'yi seçin ve sonra da **Bilgi**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="d5c85-111">**Yöneten** \<kiracı adı\> sayfasında, aşağıdaki şekilde gösterilene benzer bir **Yönetim Sunucusu Adresi** içeren **Bağlantı bilgileri** kutusunu görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5c85-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="d5c85-113">**Şirket verilerini yönetilmeyen bir uygulamaya yapıştıramadığınızı doğrulama**</span><span class="sxs-lookup"><span data-stu-id="d5c85-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="d5c85-114">Microsoft 365 İş tarafından yüklenmiş olan Outlook 2016'yı açın.</span><span class="sxs-lookup"><span data-stu-id="d5c85-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="d5c85-115">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="d5c85-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="d5c85-116">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="d5c85-117">Uygulama içeriğe erişemiyor hatasını alırsınız.</span><span class="sxs-lookup"><span data-stu-id="d5c85-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="d5c85-119">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5c85-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="d5c85-120">Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="d5c85-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="d5c85-121">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="d5c85-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="d5c85-122">Yerel kullanıcı olarak oturum açtığınız Windows 10 kişisel cihazınızda **Windows Ayarları**'na gidin ve **Hesaplar** \> **İş yeri veya okula eriş**'e tıklayın veya dokunun.</span><span class="sxs-lookup"><span data-stu-id="d5c85-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="d5c85-123">**İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="d5c85-124">**İş yeri veya okul hesabı oluştur iletişim kutusu** \> **Oturum aç** için Microsoft 365 İş kimlik bilgilerinizi girin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="d5c85-125">**İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="d5c85-127">**İş yeri veya okula eriş** sayfasında, aşağıdaki şekilde gösterilene benzeyen ve içinde  **wip**  ile  **mam**  sözcükleri bulunan bir *Yönetim Sunucusu Adresi*'nin yer aldığı *Bağlantı bilgileri* kutusunu görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5c85-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="d5c85-129">**Şirket verilerini yönetilmeyen bir uygulamaya yapıştıramadığınızı doğrulama**</span><span class="sxs-lookup"><span data-stu-id="d5c85-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="d5c85-130">Outlook 2016'yı açın, gerekirse Microsoft 365 İş hesabınızı ekleyin ve Microsoft 365 İş kimlik bilgilerinizle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="d5c85-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="d5c85-131">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="d5c85-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="d5c85-132">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="d5c85-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="d5c85-133">Uygulama içeriğe erişemiyor hatasını alırsınız.</span><span class="sxs-lookup"><span data-stu-id="d5c85-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="d5c85-135">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5c85-135">You can, however, paste the same content into Word 2016.</span></span>
    

