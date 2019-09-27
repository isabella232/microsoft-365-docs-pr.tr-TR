---
title: Kuruluma genel bakış
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business için kurulum adımlarının genel görünümü.
ms.openlocfilehash: f156d236a783942ec06d457c9b7ca087d12d6f58
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288585"
---
# <a name="overview-of-setup"></a><span data-ttu-id="c0d90-103">Kuruluma genel bakış</span><span class="sxs-lookup"><span data-stu-id="c0d90-103">Overview of setup</span></span>

<span data-ttu-id="c0d90-104">Kurulum adımlarının çoğu kurulum sihirbazında yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="c0d90-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="c0d90-105">Adım 1: Etki alanınızı ve kullanıcılarınızı ekleyin</span><span class="sxs-lookup"><span data-stu-id="c0d90-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="c0d90-106">**[Etki alanınızı ekleyin](set-up.md#add-your-domain-to-personalize-sign-in)** [(kaydolma](sign-up.md)sırasında etki alanınızı satın aldıysanız, bu adım zaten tamamlanır.)</span><span class="sxs-lookup"><span data-stu-id="c0d90-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="c0d90-107">**Kullanıcı ekle.**</span><span class="sxs-lookup"><span data-stu-id="c0d90-107">**Add users**.</span></span> <span data-ttu-id="c0d90-108">Bunu üç şekilde yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c0d90-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="c0d90-109">[Büyücüde.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="c0d90-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="c0d90-110">Şirket içinde Etkin dizininiz varsa [Azure AD Connect'i kullanarak kullanıcıları eklemek](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) için dizin eşitlemesi kullanın.</span><span class="sxs-lookup"><span data-stu-id="c0d90-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="c0d90-111">Daha sonra yönetici merkezine [de kullanıcı ekleyebilirsiniz.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="c0d90-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="c0d90-112">Adım 2: Güvenlik ilkeleri ayarlama ve aygıtları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="c0d90-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="c0d90-113">Aygıt ve güvenlik ilkelerini yapılandırmak için [Kurulum sihirbazını](set-up.md#set-up-security-policies-and-device-configurations) kullanın.</span><span class="sxs-lookup"><span data-stu-id="c0d90-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="c0d90-114">Ayrıca daha fazla ekleyebilir veya daha sonra [yönetici merkezinde](view-policies-and-devices.md) ve [Intune portalında](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)bunları edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0d90-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="c0d90-115">Kurulum sihirbazındaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c0d90-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="c0d90-116">**Kötü amaçlı yazılımkoruması e-postayla gönder**</span><span class="sxs-lookup"><span data-stu-id="c0d90-116">**Email malware protection**</span></span>
      - <span data-ttu-id="c0d90-117">**Gelişmiş Tehdit Koruması (ATP) Güvenli bağlantılar**</span><span class="sxs-lookup"><span data-stu-id="c0d90-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="c0d90-118">**ATP Güvenli Ekler**</span><span class="sxs-lookup"><span data-stu-id="c0d90-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="c0d90-119">**ATP kimlik avı önleme**</span><span class="sxs-lookup"><span data-stu-id="c0d90-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="c0d90-120">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="c0d90-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="c0d90-121">**Veri Kaybı Önleme (DLP)**</span><span class="sxs-lookup"><span data-stu-id="c0d90-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="c0d90-122">**Azure Bilgi Koruması (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="c0d90-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="c0d90-123">Görmeye başlamak için [gelişmiş güvenlik ilkeleri ayarlayın.](set-up-advanced-security.md)</span><span class="sxs-lookup"><span data-stu-id="c0d90-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="c0d90-124">Microsoft [365 Business'ınızı](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) en iyi güvenlik uygulamalarının yol haritası için güvence altına almanın en iyi 10 yolunu da görün.</span><span class="sxs-lookup"><span data-stu-id="c0d90-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="c0d90-125">Adım 3: Windows 10 aygıtlarını ayarlama ve yönetme</span><span class="sxs-lookup"><span data-stu-id="c0d90-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="c0d90-126">Bir Windows 10 aygıtına Azure AD'ye katıldığınızda, [Adım 2'de](#step-2-set-up-security-policies-and-configure-devices) ayarladığınız ilkeler uygulanır.</span><span class="sxs-lookup"><span data-stu-id="c0d90-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="c0d90-127">Windows 10 Pro, Microsoft 365 Business için bir [ön koşuldur,](pre-requisites-for-data-protection.md) ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'nuz varsa, aboneliğiniz size [Windows 10 Pro'ya yükseltme](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)hakkı verir.</span><span class="sxs-lookup"><span data-stu-id="c0d90-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="c0d90-128">Windows 10 aygıtları için ilkeleri yapılandırmak için [kurulum sihirbazını](set-up.md#set-up-security-policies-and-device-configurations) kullanın.</span><span class="sxs-lookup"><span data-stu-id="c0d90-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="c0d90-129">Stes 4: Office 365 İş install</span><span class="sxs-lookup"><span data-stu-id="c0d90-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="c0d90-130">[Kurulum sihirbazını](set-up.md#deploy-office-365-client-apps)kullanarak Office'i Windows aygıtlarına otomatik olarak yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0d90-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="c0d90-131">Office'i yönetici merkezinden otomatik olarak [yükleyin.](auto-install-or-uninstall-office.md)</span><span class="sxs-lookup"><span data-stu-id="c0d90-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="c0d90-132">Kullanıcıların Windows ve aygıtlar için [Office uygulamalarını yüklemesine](https://docs.microsoft.com/office365/admin/setup/install-applications) izin verin.</span><span class="sxs-lookup"><span data-stu-id="c0d90-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="c0d90-133">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="c0d90-133">Advanced</span></span>
- <span data-ttu-id="c0d90-134">**Yeni aygıtlar kurmak için Otomatik Pilot'u kullanma**</span><span class="sxs-lookup"><span data-stu-id="c0d90-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="c0d90-135">Bir kullanıcı için **yeni** Windows 10 aygıtlarını otomatik olarak önceden yapılandırmak için [Windows Otomatik Pilot'u](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin için yapabilecek bir [iş ortağı](https://www.microsoft.com/solution-providers/search) bulmak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="c0d90-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="c0d90-136">Ayrıca [Microsoft Mağazası'na](https://go.microsoft.com/fwlink/?linkid=874598) gidip bir bulut teknolojisi uzmanından sizin için satın aldığınız yeni aygıtlar ayarlamasını isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0d90-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="c0d90-137">**Şirket içi kaynaklara erişim**</span><span class="sxs-lookup"><span data-stu-id="c0d90-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="c0d90-138">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0d90-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="c0d90-139">Bunu ayarlamak için [Microsoft 365 Business tarafından yönetilecek etki alanına birleştirilmiş Windows 10 aygıtlarını etkinleştir](manage-windows-devices.md) metodu adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="c0d90-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="c0d90-140">Bu tercih edilen yöntemdir ve bu durumdaki aygıtlar Karma Azure AD birleştirilmiş aygıtlar olarak adlandırılır.</span><span class="sxs-lookup"><span data-stu-id="c0d90-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="c0d90-141">İşletmenizde bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Etkin Dizin varsa, Azure AD'ye katılan aygıtlarınıza bu kaynaklara buradaki adımları izleyerek erişim sağlayabilirsiniz: [Şirket içi kaynaklara bir Microsoft 365 Business'ta Azure AD'ye bağlı aygıt.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="c0d90-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  