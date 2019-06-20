---
title: Ayarlama, genel bakış
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 iş kurma adımları genel bakış.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086410"
---
# <a name="overview-of-setup"></a><span data-ttu-id="ef1e6-103">Kurulum, genel bakış</span><span class="sxs-lookup"><span data-stu-id="ef1e6-103">Overview of setup</span></span>

<span data-ttu-id="ef1e6-104">Kurulum sihirbazındaki adımları ayarlamak çoğu yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="ef1e6-105">Adım 1: etki alanı ve kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="ef1e6-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="ef1e6-106">**[Etki alanınızın Ekle](set-up.md#add-your-domain-to-personalize-sign-in)** ( [kayıt](sign-up.md)sırasında etki alanı satın aldıysanız, bu adımı zaten yapılır.)</span><span class="sxs-lookup"><span data-stu-id="ef1e6-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="ef1e6-107">**Kullanıcı Ekle**.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-107">**Add users**.</span></span> <span data-ttu-id="ef1e6-108">Herhangi üç yoldan biriyle yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="ef1e6-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="ef1e6-109">[Sihirbaz](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="ef1e6-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="ef1e6-110">Eğer yerinde Active directory directory eşitlemesi [Azure AD Connect kullanarak kullanıcı eklemek](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) için kullanın.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="ef1e6-111">[Daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="ef1e6-112">2. adım: güvenlik ilkelerini ayarlama ve aygıtları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="ef1e6-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="ef1e6-113">Aygıt ve güvenlik ilkelerini yapılandırmak için [Kurulum Sihirbazı](set-up.md#set-up-security-policies-and-device-configurations) ' nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="ef1e6-114">Ayrıca daha ekleyebilir veya daha sonra [Yönetim Merkezi](view-policies-and-devices.md) ve [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="ef1e6-115">Kurulum Sihirbazı'ndaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek, güvenliğini artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="ef1e6-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="ef1e6-116">**E-posta zararlı yazılımlara karşı koruma**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-116">**Email malware protection**</span></span>
      - <span data-ttu-id="ef1e6-117">**Gelişmiş tehdit Koruması (ATP) güvenli bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="ef1e6-118">**ATP güvenli ekler**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="ef1e6-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="ef1e6-120">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="ef1e6-121">**Veri kaybını önleme (DLP)**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="ef1e6-122">**Azure bilgi koruma (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="ef1e6-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="ef1e6-123">Almak için bkz: [Gelişmiş güvenlik ilkelerini kurun](set-up-advanced-security.md)başladı.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="ef1e6-124">Ayrıca bkz: [Microsoft 365 işletmenizin güvenliğini sağlamak için üst 10 yolu](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) için bir yol haritası, en iyi güvenlik yöntemleri.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="ef1e6-125">Adım 3: Ayarlanır ve Windows 10 aygıtları yönetme</span><span class="sxs-lookup"><span data-stu-id="ef1e6-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="ef1e6-126">Windows 10 aygıt için Azure AD katıldığınızda, [Adım 2](#step-2-set-up-security-policies-and-configure-devices) ' de ayarladığınız ilkeleri uygulanan.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="ef1e6-127">Windows 10 Pro Microsoft 365 iş için bir [ön gereksinim](pre-requisites-for-data-protection.md) olmakla birlikte, Pro Windows 7, Windows 8 Pro veya Windows 8.1 Pro varsa, aboneliğiniz, [Windows 10 Pro yükseltmek](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)için hakkı verir.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="ef1e6-128">Windows 10 aygıtları ilkelerini yapılandırmak için [Kurulum Sihirbazı](set-up.md#set-up-security-policies-and-device-configurations) ' nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="ef1e6-129">Stes 4: Office 365 iş yükleme</span><span class="sxs-lookup"><span data-stu-id="ef1e6-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="ef1e6-130">[Kurulum Sihirbazı](set-up.md#deploy-office-365-client-apps)' nı kullanarak Windows aygıtlardan Office otomatik olarak yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="ef1e6-131">Otomatik olarak [Office yükleme](auto-install-or-uninstall-office.md) Yönetim Merkezi'nden.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="ef1e6-132">Kullanıcıların [Office uygulamaları yüklemek](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows ve aygıtlar için olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="ef1e6-133">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="ef1e6-133">Advanced</span></span>
- <span data-ttu-id="ef1e6-134">**Yeni aygıtları için AutoPilot kullanın**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="ef1e6-135">[Windows Autopilot](add-autopilot-devices-and-profile.md) otomatik olarak **Yeni** bir kullanıcı Windows 10 aygıtları önceden yapılandırmak için kullanabilirsiniz, ancak sizin için bunu yapmak için bir [ortak](https://www.microsoft.com/solution-providers/search) almak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="ef1e6-136">[Microsoft mağaza](https://go.microsoft.com/fwlink/?linkid=874598) ve yeni aygıtlar için satın bir bulut teknoloji uzmanı ayarlamak isteyin.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="ef1e6-137">**Şirket içi kaynaklara erişmek**</span><span class="sxs-lookup"><span data-stu-id="ef1e6-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="ef1e6-138">Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="ef1e6-139">Bunu ayarlamak için [Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış Windows 10 aygıtları etkinleştirme](manage-windows-devices.md) adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="ef1e6-140">Tercih edilen yöntem budur ve bu durumda aygıtları karma Azure adı verilen AD alanına bağlı aygıtlar.</span><span class="sxs-lookup"><span data-stu-id="ef1e6-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="ef1e6-141">Bazı içeren Active Directory yerinde kaynaklar (örneğin, dosya paylaşımları ve yazıcılar), bu kaynakların Azure AD alanına bağlı aygıtlara erişiminizi burada adımları izleyerek verebilirsiniz İşletmenizde yerel varsa: [erişim şirket içi kaynaklardan bir 365 işletmede Azure AD alanına bağlı aygıt](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="ef1e6-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  