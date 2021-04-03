---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 cihazlarında Microsoft 365 İş Ekstra uygulama koruma ayarlarını doğrulayın ve kullanıcıların şirket verilerini kişisel dosyalara veya yönetilmeyen uygulamalara kopyalayamalarını doğrulayın.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579872"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="5a910-103">Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="5a910-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="5a910-104">Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="5a910-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="5a910-105">[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir.</span><span class="sxs-lookup"><span data-stu-id="5a910-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="5a910-106">Kullanıcıların şirket  verilerini kişisel dosyalara kopyalamasını engelle ayarını etkinleştirirseniz ve şirkete ait cihazlar için iş dosyalarını **OneDrive** İş ayarına kaydetmelerini zorlarsanız, Azure AD'ye bağlandıktan ve oturum açınktan sonra kullanıcının cihazında bunu kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5a910-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="5a910-107">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="5a910-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="5a910-108">Microsoft 365 İş Ekstra kimlik bilgileriyle oturum açın ve [Microsoft 365 İş](set-up-windows-devices.md)Ekstra kullanıcıları için Windows cihazlarını ayarlama konusunda açıklandığı gibi Azure AD'ye bağlanın, iş veya okul için **Windows** Ayarları Hesapları Erişimi'ne \>  \> gidin.</span><span class="sxs-lookup"><span data-stu-id="5a910-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="5a910-109">**\<tenant name\> Azure AD'ye Bağlan'ı** ve ardından Bilgi'yi **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5a910-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="5a910-111">Yönetilen **sayfasında,** aşağıdaki şekilde gösterilene benzer bir \<tenant name\> Yönetim Sunucusu Adresi **içeren** Bağlantı  bilgilerini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5a910-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="5a910-113">**Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramay işleminizi doğrulama**</span><span class="sxs-lookup"><span data-stu-id="5a910-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="5a910-114">Microsoft 365 İş Ekstra tarafından yüklenmiş olan Outlook 2016'ya açın.</span><span class="sxs-lookup"><span data-stu-id="5a910-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="5a910-115">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="5a910-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="5a910-116">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="5a910-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="5a910-117">Uygulamanın içeriğe erişe olmadığını haber alan bir hata alırsınız.</span><span class="sxs-lookup"><span data-stu-id="5a910-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="5a910-119">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5a910-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="5a910-120">Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama</span><span class="sxs-lookup"><span data-stu-id="5a910-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="5a910-121">**Bağlantı ayarlarını doğrulama**</span><span class="sxs-lookup"><span data-stu-id="5a910-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="5a910-122">Yerel kullanıcı olarak oturum açtığınız Windows 10 kişisel aygıtınızda, **Windows** Ayarları'na  gidin ve Hesaplar Erişimi'ne iş veya okul tıklayın \> **veya dokunun.**</span><span class="sxs-lookup"><span data-stu-id="5a910-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="5a910-123">**İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5a910-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="5a910-124">İş veya okul hesabı ayarla iletişim kutusunda Microsoft 365 İş Ekstra kimlik **bilgilerinizi** \> **girin.**</span><span class="sxs-lookup"><span data-stu-id="5a910-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="5a910-125">**İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="5a910-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![İş veya okul hesabı iletişim kutusunda Bilgi'ye tıklayın veya dokunun.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="5a910-127">Access **iş** veya okul sayfasında, aşağıdaki  şekilde gösterilene benzer bir **Yönetim** Sunucusu Adresi içeren ve içinde *wip* ve mam sözcükleri bulunan Bağlantı *bilgilerini* görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5a910-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="5a910-129">**Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramay işleminizi doğrulama**</span><span class="sxs-lookup"><span data-stu-id="5a910-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="5a910-130">Outlook 2016'yi açın, gerekirse Microsoft 365 İş Ekstra hesabını ekleyin ve Microsoft 365 İş Ekstra kimlik bilgilerinizle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5a910-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="5a910-131">Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="5a910-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="5a910-132">Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="5a910-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="5a910-133">Uygulama'nın içeriğe erişe olmadığını haber alan bir hata alırsınız.</span><span class="sxs-lookup"><span data-stu-id="5a910-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="5a910-135">Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5a910-135">You can, however, paste the same content into Word 2016.</span></span>
    

