---
title: Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlama
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Merkezi yönetim ve güvenlik denetimlerini etkinleştiren Microsoft 365 Business Premium kullanıcıları için Windows 10 Pro çalıştıran Windows aygıtlarını nasıl ayarlayabilirsiniz öğrenin.
ms.openlocfilehash: 85ac3c964792a132d5699703e543289020e38f57
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785862"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="2339c-103">Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlama</span><span class="sxs-lookup"><span data-stu-id="2339c-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="2339c-104">Microsoft 365 Business Premium kullanıcıları için Windows aygıtları kurmak için ön koşullar</span><span class="sxs-lookup"><span data-stu-id="2339c-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="2339c-105">Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlamadan önce, tüm Windows aygıtlarının Windows 10 Pro, sürüm 1703 (Creators Update) çalıştırdığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="2339c-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="2339c-106">Windows 10 Pro, Windows 10 Pro'yu tamamlayan ve Microsoft 365 Business Premium'un merkezi yönetim ve güvenlik denetimlerini etkinleştiren bir dizi bulut hizmeti ve aygıt yönetimi özelliği olan Windows 10 Business'ı dağıtmak için bir ön koşuldur.</span><span class="sxs-lookup"><span data-stu-id="2339c-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="2339c-107">Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro çalıştıran Windows aygıtlarınız varsa, Microsoft 365 Business Premium aboneliğiniz size Windows 10 yükseltmesi hakkı verir.</span><span class="sxs-lookup"><span data-stu-id="2339c-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="2339c-108">Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltme hakkında daha fazla bilgi için bu konudaki adımları izleyin: [Windows cihazları Windows Pro Creators Update sürümüne yükseltme](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="2339c-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="2339c-109">Bkz. Yükseltmeye sahip olduğunuzu doğrulamak veya yükseltmenin çalıştığından emin olmak için [aygıtın Azure AD'ye bağlı olduğunu doğrulayın.](#verify-the-device-is-connected-to-azure-ad)</span><span class="sxs-lookup"><span data-stu-id="2339c-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="2339c-110">Windows'u Microsoft 365'e bağlama hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="2339c-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="2339c-111">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="2339c-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="2339c-112">Kuruluşunuzun Azure AD'sine Windows 10 cihazlarını ekleme</span><span class="sxs-lookup"><span data-stu-id="2339c-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="2339c-113">Kuruluşunuzdaki tüm Windows aygıtları Windows 10 Pro Creators Update'e yükseltilmiş sa veya Windows 10 Pro Creators Update'i zaten çalıştırıyorsa, bu aygıtları kuruluşunuzun Azure Etkin Dizini'ne katılabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2339c-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="2339c-114">Aygıtlar birleştikten sonra, Microsoft 365 Business Premium aboneliğinizin bir parçası olan Windows 10 Business'a otomatik olarak yükseltilir.</span><span class="sxs-lookup"><span data-stu-id="2339c-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="2339c-115">Yeni yükseltilmiş veya yeni bir Windows 10 Pro cihaz için</span><span class="sxs-lookup"><span data-stu-id="2339c-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="2339c-116">Windows 10 Pro Creators Update çalıştıran yeni bir cihaz için ya da Windows 10 Pro Creators Update sürümüne yükseltilmiş ancak Windows 10 cihaz kurulumu henüz tamamlanmamış bir cihaz için bu adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2339c-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="2339c-117">**Nasıl ayarlamak istersiniz?** sayfasına gelene kadar Windows 10 cihaz kurulumu adımlarını tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="2339c-119">Burada, **bir kuruluş için ayarla'yı** seçin ve ardından Microsoft 365 Business Premium için kullanıcı adınızı ve parolanızı girin.</span><span class="sxs-lookup"><span data-stu-id="2339c-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="2339c-120">Windows 10 cihazı kurulumunu tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="2339c-121">Once you're done, the user will be connected to your organization's Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2339c-121">Once you're done, the user will be connected to your organization's Azure AD.</span></span> <span data-ttu-id="2339c-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span><span class="sxs-lookup"><span data-stu-id="2339c-122">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="2339c-123">Önceden ayarlanmış ve Windows 10 Pro çalıştıran bir cihaz için</span><span class="sxs-lookup"><span data-stu-id="2339c-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="2339c-124">**Kullanıcıları Azure AD'ye bağlama:**</span><span class="sxs-lookup"><span data-stu-id="2339c-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="2339c-125">Kullanıcınızın Windows 10 Pro sürüm 1703 (Creators Update) (bkz. [önkoşullar](pre-requisites-for-data-protection.md)) çalıştıran Windows bilgisayarında, Windows logosuna ve ardından Ayarlar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="2339c-127">**Ayarlar**'da **Hesaplar**'a gidin.</span><span class="sxs-lookup"><span data-stu-id="2339c-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="2339c-129">**Bilgileriniz** sayfasında **İş yeri veya okula erişim** \> **Bağlan**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="2339c-131">**İş veya okul hesabı ayarlama** iletişim kutusunda **Diğer eylemler**'in altında **Bu cihazı Azure Active Directory'ye ekleyin**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="2339c-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="2339c-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="2339c-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="2339c-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="2339c-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="2339c-136">Bunun **kuruluş sayfanız olduğundan emin olun,** bilgilerin doğru olduğundan emin olun ve **Katıl'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2339c-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="2339c-137">On the **You're all set!**</span><span class="sxs-lookup"><span data-stu-id="2339c-137">On the **You're all set!**</span></span> <span data-ttu-id="2339c-138">page, click **Done**.</span><span class="sxs-lookup"><span data-stu-id="2339c-138">page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="2339c-140">OneDrive İş'e dosya yüklediyseniz, bunları tekrar eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="2339c-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="2339c-141">Profili ve dosyaları geçirmek için bir üçüncü taraf aracı kullandıysanız, bunları yeni profille de eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="2339c-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="2339c-142">Cihazın Azure AD'ye bağlı olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="2339c-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="2339c-143">**Eşitleme**durumunuzu doğrulamak için Ayarlar'daki **Access çalışmasında veya okul** sayfasında , Bilgi ve Bağlantı kesme düğmelerini ortaya çıkarmak için _ _ alanına **Bağlı'yı** \<organization name\> **Info** tıklatın. **Disconnect**</span><span class="sxs-lookup"><span data-stu-id="2339c-143">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="2339c-144">Eşitleme durumunuzu görmek için **Bilgi**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-144">Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="2339c-145">En son mobil cihaz yönetimi ilkelerini bilgisayara aktarmak için, Eşitleme durumu sayfasında Eşitle'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="2339c-146">Microsoft 365 Business Premium hesabını kullanmaya başlamak için Windows **Start** düğmesine gidin, geçerli hesap resminize sağ tıklayın ve ardından **hesabı değiştirin.**</span><span class="sxs-lookup"><span data-stu-id="2339c-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="2339c-147">Kurumsal e-postanız ve parolanızla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="2339c-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="2339c-149">Cihazın Windows 10 Business'a yükseltildiğini doğrulama</span><span class="sxs-lookup"><span data-stu-id="2339c-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="2339c-150">Azure AD'nizin Windows 10'a katıldığını doğrulayın, Microsoft 365 Business Premium aboneliğinizin bir parçası olarak Windows 10 Business'a yükseltildi.</span><span class="sxs-lookup"><span data-stu-id="2339c-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="2339c-151">**Ayarlar** \> **Sistem** \> **Hakkında**'ya gidin.</span><span class="sxs-lookup"><span data-stu-id="2339c-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="2339c-152">**Sürüm** bölümünde **Windows 10 Business** ifadesinin bulunduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="2339c-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="2339c-154">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="2339c-154">Next steps</span></span>

<span data-ttu-id="2339c-155">Mobil cihazlarınızı ayarlamak için bkz: [Microsoft 365 Business Premium kullanıcıları için mobil cihazlar ayarla](set-up-mobile-devices.md), Cihaz koruma veya uygulama koruma ilkeleri ayarlamak [için, iş için Microsoft 365'i yönet'e](manage.md)bakın.</span><span class="sxs-lookup"><span data-stu-id="2339c-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="2339c-156">Microsoft 365 Business Premium'u kurma ve kullanma hakkında daha fazla şey için</span><span class="sxs-lookup"><span data-stu-id="2339c-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="2339c-157">İş eğitimi videoları için Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2339c-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
