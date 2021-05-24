---
title: Mobil Windows cihazları Microsoft 365 İş Ekstra ayarlama
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Kullanıcı Windows çalışan Windows 10 Pro cihazlarını Microsoft 365 İş Ekstra ve merkezi yönetim ve güvenlik denetimlerini etkinleştirebilirsiniz.
ms.openlocfilehash: 3d32a033a1a1c89d7d4d557cea6a28e24543ab2c
ms.sourcegitcommit: b0d3abbccf4dd37e32d69664d3ebc9ab8dea760d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/21/2021
ms.locfileid: "52594031"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="6b8b0-103">Mobil Windows cihazları Microsoft 365 İş Ekstra ayarlama</span><span class="sxs-lookup"><span data-stu-id="6b8b0-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="6b8b0-104">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="6b8b0-104">Before you begin</span></span>

<span data-ttu-id="6b8b0-105">Microsoft 365 İş Ekstra için Windows cihazları ayarlamadan önce tüm Windows 1703 sürümü (Creators Update) Windows 10 Pro çalıştıran cihazlardan emin olun.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="6b8b0-106">Windows 10 Pro, Windows 10 Business'i tamamlayıcı nitelikte olan ve Windows 10 Pro'un merkezi yönetim ve güvenlik denetimlerini etkinleştiren bulut hizmetleri ve cihaz yönetimi özellikleri kümesi olan Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="6b8b0-107">Windows 7 Windows, Pro, Windows 8 Pro veya Windows 8.1 Pro çalıştıran Microsoft 365 İş Ekstra cihazlarınız varsa, Microsoft 365 İş Ekstra aboneliğiniz size Windows 10 verir.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="6b8b0-108">Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltme hakkında daha fazla bilgi için bu konudaki adımları izleyin: [Windows cihazları Windows Pro Creators Update sürümüne yükseltme](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="6b8b0-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="6b8b0-109">Yükseltmeye [sahip olduğunuzdan emin olmak veya yükseltmenin](#verify-the-device-is-connected-to-azure-ad) çalıştığını doğrulamak için bkz. Cihazın Azure AD'ye bağlı olduğunu doğrulama.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="6b8b0-110">E-Windows'i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="6b8b0-111">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="6b8b0-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="6b8b0-112">Kuruluşunuzun Azure AD'sine Windows 10 cihazlarını ekleme</span><span class="sxs-lookup"><span data-stu-id="6b8b0-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="6b8b0-113">Tüm Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltildikten sonra veya Windows 10 Pro Creators Update'i zaten çalıştırıyorsa, bu cihazları kuruluş kuruluşlarının Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="6b8b0-114">Cihazlar katıldıktan sonra, otomatik olarak Microsoft 365 İş Ekstra aboneliğinizin bir parçası olan Windows 10 Business'e Microsoft 365 İş Ekstra yükseltilir.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="6b8b0-115">Yeni yükseltilmiş veya yeni bir Windows 10 Pro cihaz için</span><span class="sxs-lookup"><span data-stu-id="6b8b0-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="6b8b0-116">Windows 10 Pro Creators Update çalıştıran yeni bir cihaz için ya da Windows 10 Pro Creators Update sürümüne yükseltilmiş ancak Windows 10 cihaz kurulumu henüz tamamlanmamış bir cihaz için bu adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="6b8b0-117">**Nasıl ayarlamak istersiniz?** sayfasına gelene kadar Windows 10 cihaz kurulumu adımlarını tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="6b8b0-119">Burada, Kuruluş **için ayarla'ya tıklayın** ve kuruluş için kullanıcı adınızı ve parolanızı Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="6b8b0-120">Windows 10 cihazı kurulumunu tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="6b8b0-p103">İşiniz bittiğinde kullanıcı, kuruluşunuzun Azure AD'sine bağlanmış olur. Emin olmak için bkz. [Cihazın Azure AD'ye bağlı olduğunu doğrulama](#verify-the-device-is-connected-to-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="6b8b0-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="6b8b0-123">Önceden ayarlanmış ve Windows 10 Pro çalıştıran bir cihaz için</span><span class="sxs-lookup"><span data-stu-id="6b8b0-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="6b8b0-124">**Kullanıcıları Azure AD'ye bağlama:**</span><span class="sxs-lookup"><span data-stu-id="6b8b0-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="6b8b0-125">Kullanıcınızın Windows 10 Pro sürüm 1703 (Creators Update) (bkz. [önkoşullar](pre-requisites-for-data-protection.md)) çalıştıran Windows bilgisayarında, Windows logosuna ve ardından Ayarlar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="6b8b0-127">**Ayarlar**'da **Hesaplar**'a gidin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="6b8b0-129">**Bilgileriniz** sayfasında **İş yeri veya okula erişim** \> **Bağlan**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="6b8b0-131">**İş veya okul hesabı ayarlama** iletişim kutusunda **Diğer eylemler**'in altında **Bu cihazı Azure Active Directory'ye ekleyin**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="6b8b0-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="6b8b0-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="6b8b0-136">Bunun **sizin kuruluş bağlantınız olduğundan emin olun** sayfasında, bilgilerin doğru olduğundan emin olun ve Katıl'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="6b8b0-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="6b8b0-137">**Hazırsınız!**</span><span class="sxs-lookup"><span data-stu-id="6b8b0-137">On the **You're all set!**</span></span> <span data-ttu-id="6b8b0-138">page, chosse **Done .**</span><span class="sxs-lookup"><span data-stu-id="6b8b0-138">page, chosse **Done**.</span></span>
  
   ![Bunun sizin kuruluş ekranınız olduğundan emin olun ekranında Katıl'ı seçin](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="6b8b0-140">OneDrive İş'e dosya yüklediyseniz, bunları tekrar eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="6b8b0-141">Profil ve dosyaları geçirmek için üçüncü taraf bir araç kullandıysanız, bu dosyaları da yeni profile eşitlenin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="6b8b0-142">Cihazın Azure AD'ye bağlı olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="6b8b0-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="6b8b0-143">Eşitlemenizin durumunu doğrulamak için, Ayarlar'daki İş veya okula **erişim** sayfasında **Bağlı** _ _ alanı öğesini seçerek Bilgi ve Bağlantıyı Kes \<organization name\> düğmelerini **gösterebilirsiniz.** </span><span class="sxs-lookup"><span data-stu-id="6b8b0-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="6b8b0-144">Eşitlemenizin **durumunu** almak için Bilgi'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="6b8b0-145">En son **mobil cihaz yönetim** ilkelerini bilgisayara **almak** için Eşitleme durumu sayfasında Eşitle'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="6b8b0-146">Microsoft 365 İş Ekstra kullanmaya başlamak için, Başlangıç Windows gidin, geçerli  hesap resminize sağ tıklayın ve Ardından Hesap **değiştir'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="6b8b0-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="6b8b0-147">Kurumsal e-postanız ve parolanızla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="6b8b0-149">Pc'nin Şu sürüme yükseltildikten Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="6b8b0-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="6b8b0-150">Azure AD'ye katılmış Windows 10 cihazlarınızı Windows 10 Business aboneliğinizin bir parçası olarak Microsoft 365 İş Ekstra doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="6b8b0-151">**Ayarlar** \> **Sistem** \> **Hakkında**'ya gidin.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="6b8b0-152">**Sürüm** bölümünde **Windows 10 Business** ifadesinin bulunduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="6b8b0-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="6b8b0-154">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="6b8b0-154">Next steps</span></span>

<span data-ttu-id="6b8b0-155">Mobil cihazlarınızı ayarlamak için bkz. Microsoft 365 İş Ekstra kullanıcıları için mobil cihazları ayarlama [,](set-up-mobile-devices.md)Cihaz koruma veya uygulama koruma ilkelerini ayarlamak için bkz. [Microsoft 365 yönetme](manage.md).</span><span class="sxs-lookup"><span data-stu-id="6b8b0-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="related-content"></a><span data-ttu-id="6b8b0-156">İlgili içerik</span><span class="sxs-lookup"><span data-stu-id="6b8b0-156">Related content</span></span>

<span data-ttu-id="6b8b0-157">[Microsoft 365 eğitim videoları için giriş](../business-video/index.yml) (bağlantı sayfası)</span><span class="sxs-lookup"><span data-stu-id="6b8b0-157">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
