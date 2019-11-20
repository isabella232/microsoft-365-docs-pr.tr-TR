---
title: Microsoft 365 Business kullanıcıları için Windows cihazlarını ayarlama
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
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Microsoft 365 Business kullanıcıları için Windows 10 Pro çalıştıran Windows aygıtlarını nasıl ayarlayabilirsiniz öğrenin. '
ms.openlocfilehash: f929c64b00e4ebf24e9f82fcfea433119abf2f1c
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718889"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="38378-103">Microsoft 365 Business kullanıcıları için Windows cihazlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="38378-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38378-104">Önkoşullar</span><span class="sxs-lookup"><span data-stu-id="38378-104">Prerequisites</span></span>

<span data-ttu-id="38378-p101">Microsoft 365 Business kullanıcıları için Windows cihazları ayarlamadan önce, tüm Windows cihazların Windows 10 Pro sürüm 1703 (Creators Update) çalıştırdığından emin olun. Windows 10 Pro'yu tamamlayıcı nitelikte bir bulut hizmetleri ve cihaz yönetimi kümesi olan ve Microsoft 365 Business'ın güvenlik denetimlerine ve merkezi olarak yönetilmesine olanak sağlayan Windows 10 Business'in dağıtımı için gerekli önkoşullardan biri Windows 10 Pro'dur.</span><span class="sxs-lookup"><span data-stu-id="38378-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="38378-107">Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro çalıştıran Windows cihazlarınız varsa, Microsoft 365 Business aboneliğiniz size bir Windows 10 yükseltmesi hakkı tanır.</span><span class="sxs-lookup"><span data-stu-id="38378-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="38378-108">Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltme hakkında daha fazla bilgi için bu konudaki adımları izleyin: [Windows cihazları Windows Pro Creators Update sürümüne yükseltme](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="38378-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="38378-109">Bkz. Yükseltmeye sahip olduğunuzu doğrulamak veya yükseltmenin çalıştığından emin olmak için [aygıtın Azure AD'ye bağlı olduğunu doğrulayın.](#verify-the-device-is-connected-to-azure-ad)</span><span class="sxs-lookup"><span data-stu-id="38378-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span> 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="38378-110">Kuruluşunuzun Azure AD'sine Windows 10 cihazlarını ekleme</span><span class="sxs-lookup"><span data-stu-id="38378-110">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="38378-111">Kuruluşunuzdaki tüm Windows aygıtları Windows 10 Pro Creators Update'e yükseltilmiş sa veya Windows 10 Pro Creators Update'i zaten çalıştırıyorsa, bu aygıtları kuruluşunuzun Azure Etkin Dizini'ne katılabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="38378-111">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="38378-112">Aygıtlar birleştikten sonra, Microsoft 365 Business aboneliğinizin bir parçası olan Windows 10 Business'a otomatik olarak yükseltilir.</span><span class="sxs-lookup"><span data-stu-id="38378-112">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="38378-113">Yeni yükseltilmiş veya yeni bir Windows 10 Pro cihaz için</span><span class="sxs-lookup"><span data-stu-id="38378-113">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="38378-114">Windows 10 Pro Creators Update çalıştıran yeni bir cihaz için ya da Windows 10 Pro Creators Update sürümüne yükseltilmiş ancak Windows 10 cihaz kurulumu henüz tamamlanmamış bir cihaz için bu adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="38378-114">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="38378-115">**Nasıl ayarlamak istersiniz?** sayfasına gelene kadar Windows 10 cihaz kurulumu adımlarını tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="38378-115">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="38378-117">Burada **Kuruluş için ayarlama**'yı seçin ve ardından Microsoft 365 Business kullanıcı adınızı ve parolanızı girin.</span><span class="sxs-lookup"><span data-stu-id="38378-117">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="38378-118">Windows 10 cihazı kurulumunu tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="38378-118">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="38378-p103">İşiniz bittiğinde kullanıcı, kuruluşunuzun Azure AD'sine bağlanmış olur. Emin olmak için bkz. [Cihazın Azure AD'ye bağlı olduğunu doğrulama](#verify-the-device-is-connected-to-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="38378-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="38378-121">Önceden ayarlanmış ve Windows 10 Pro çalıştıran bir cihaz için</span><span class="sxs-lookup"><span data-stu-id="38378-121">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="38378-122">**Kullanıcıları Azure AD'ye bağlama:**</span><span class="sxs-lookup"><span data-stu-id="38378-122">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="38378-123">Kullanıcınızın Windows 10 Pro sürüm 1703 (Creators Update) (bkz. [önkoşullar](pre-requisites-for-data-protection.md)) çalıştıran Windows bilgisayarında, Windows logosuna ve ardından Ayarlar simgesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="38378-123">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="38378-125">**Ayarlar**'da **Hesaplar**'a gidin.</span><span class="sxs-lookup"><span data-stu-id="38378-125">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="38378-127">**Bilgileriniz** sayfasında **İş yeri veya okula erişim** \> **Bağlan**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="38378-127">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="38378-129">**İş veya okul hesabı ayarlama** iletişim kutusunda **Diğer eylemler**'in altında **Bu cihazı Azure Active Directory'ye ekleyin**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="38378-129">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="38378-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="38378-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="38378-132">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="38378-132">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="38378-134">Bunun **kuruluş sayfanız olduğundan emin olun,** bilgilerin doğru olduğundan emin olun ve **Katıl'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="38378-134">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="38378-p104">**Hazırsınız!** sayfasında **Bitti**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="38378-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="38378-138">OneDrive İş'e dosya yüklediyseniz, bunları tekrar eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="38378-138">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="38378-139">Profili ve dosyaları geçirmek için bir üçüncü taraf aracı kullandıysanız, bunları yeni profille de eşitleyin.</span><span class="sxs-lookup"><span data-stu-id="38378-139">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="38378-140">Cihazın Azure AD'ye bağlı olduğunu doğrulama</span><span class="sxs-lookup"><span data-stu-id="38378-140">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="38378-p106">Eşitleme durumunuzu doğrulamak için, **Ayarlar**'daki **İş yeri veya okula erişim** sayfasında **Bağlanılan yer** _ \<organization name\> _ alanına tıklayarak **Bilgi** ve **Bağlantıyı kes** düğmelerini görüntüleyin. Eşitleme durumunuzu görmek için **Bilgi**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="38378-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="38378-143">En son mobil cihaz yönetimi ilkelerini bilgisayara aktarmak için, Eşitleme durumu sayfasında Eşitle'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="38378-143">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="38378-144">Microsoft 365 Business hesabını kullanmaya başlamak için Windows **Başlat** düğmesine gidin, geçerli hesap resminize sağ tıklayın ve ardından **hesabı değiştirin.**</span><span class="sxs-lookup"><span data-stu-id="38378-144">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="38378-145">Kurumsal e-postanız ve parolanızla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="38378-145">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="38378-147">Cihazın Windows 10 Business'a yükseltildiğini doğrulama</span><span class="sxs-lookup"><span data-stu-id="38378-147">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="38378-148">Azure AD'ye eklenmiş Windows 10 cihazlarınızın, Microsoft 365 Business aboneliğinize dahil olan Windows 10 Business'a yükseltildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="38378-148">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="38378-149">**Ayarlar** \> **Sistem** \> **Hakkında**'ya gidin.</span><span class="sxs-lookup"><span data-stu-id="38378-149">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="38378-150">**Sürüm** bölümünde **Windows 10 Business** ifadesinin bulunduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="38378-150">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="38378-152">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="38378-152">Next steps</span></span>

<span data-ttu-id="38378-153">Mobil cihazlarınızı ayarlamak için [Microsoft 365 Business kullanıcıları için mobil cihazları ayarlama](set-up-mobile-devices.md) bölümüne, cihaz koruma veya uygulama koruma ilkelerini ayarlamak içinse [Microsoft 365 Business yönetimi](manage.md) bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="38378-153">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
