---
title: Kuruluma genel bakış
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Aboneden etki alanı ve kullanıcı eklemeye, güvenlik ilkelerini ayarlamaya ve daha birçok işlemi yapmak için Microsoft 365 İş Ekstra'ya yönelik kurulum adımlarını öğrenin.
ms.openlocfilehash: 9d92aefb3b5666bb7c2fd2e13c9a00f074f107a7
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912500"
---
# <a name="overview-of-setup"></a><span data-ttu-id="65bd6-103">Kuruluma genel bakış</span><span class="sxs-lookup"><span data-stu-id="65bd6-103">Overview of setup</span></span>

<span data-ttu-id="65bd6-104">Microsoft 365 İş Ekstra kurulumu hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="65bd6-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="65bd6-105">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="65bd6-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="65bd6-106">Kurulum adımlarının çoğu kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="65bd6-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="65bd6-107">1. Adım: Etki alanınızı ve kullanıcılarınızı ekleme</span><span class="sxs-lookup"><span data-stu-id="65bd6-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="65bd6-108">**[Etki alanınızı](set-up.md#add-your-domain-to-personalize-sign-in)** ekleyin (kayıt sırasında etki alanınızı [satın aldıysanız,](sign-up.md)bu adım zaten tamamdır.)</span><span class="sxs-lookup"><span data-stu-id="65bd6-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="65bd6-109">**Kullanıcı ekle 'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="65bd6-109">**Add users**.</span></span> <span data-ttu-id="65bd6-110">Kullanıcıları şu üç şekilden herhangi birini eklemenin yolları vardır:</span><span class="sxs-lookup"><span data-stu-id="65bd6-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="65bd6-111">Kılavuzlu [kurulumda.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="65bd6-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="65bd6-112">Şirket içi Active [directory'niz varsa, Azure AD Connect](../enterprise/set-up-directory-synchronization.md) kullanarak kullanıcıları eklemek için dizin eşitlemesini kullanın.</span><span class="sxs-lookup"><span data-stu-id="65bd6-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="65bd6-113">Kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de ebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd6-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="65bd6-114">2. Adım: Güvenlik ilkelerini ayarlama ve cihazları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="65bd6-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="65bd6-115">Cihaz ilkelerini [yapılandırmak için](set-up.md#protect-your-organization) kılavuzlu kurulumu kullanın.</span><span class="sxs-lookup"><span data-stu-id="65bd6-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="65bd6-116">Ayrıca, daha sonra yönetim merkezinde ve Intune [portalında](view-policies-and-devices.md) daha fazla ekleyebilir veya [bunları düzenleyebilirsiniz.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="65bd6-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="65bd6-117">Kurulum sihirbazı ayrıca temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.</span><span class="sxs-lookup"><span data-stu-id="65bd6-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="65bd6-118">Kurulum sihirbazında güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="65bd6-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="65bd6-119">**E-posta kötü amaçlı yazılıma karşı koruma**</span><span class="sxs-lookup"><span data-stu-id="65bd6-119">**Email malware protection**</span></span>
- <span data-ttu-id="65bd6-120">**Office 365 için Defender'da kimlik avı önleme**</span><span class="sxs-lookup"><span data-stu-id="65bd6-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="65bd6-121">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="65bd6-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="65bd6-122">**Azure Information Protection (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="65bd6-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="65bd6-123">Başlamak için tehdit [korumasını artırmaya bakın](increase-threat-protection.md) [ve uyumluluk özelliklerini ayarlayın.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="65bd6-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="65bd6-124">En iyi [güvenlik uygulamalarının yol haritası için Microsoft 365 İş Ekstra'nızı](/office365/admin/security-and-compliance/secure-your-business-data) güvenli hale etmenin en iyi 10 yolunu da inceleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd6-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="65bd6-125">3. Adım: Windows 10 cihazlarını ayarlama ve yönetme</span><span class="sxs-lookup"><span data-stu-id="65bd6-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="65bd6-126">Rehberli kurulumu tamamlandıktan sonra, organizasyonınızdaki tüm Windows 10 bilgisayarlarını korumak istediğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="65bd6-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="65bd6-127">Windows 10 Pro, Microsoft 365 İş Ekstra'nın önkoşullarıdır, ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'nız varsa, aboneliğiniz [size Windows 10 Pro'ya](./upgrade-to-windows-pro-creators-update.md)yükseltme hakkı sağlar. [](pre-requisites-for-data-protection.md)</span><span class="sxs-lookup"><span data-stu-id="65bd6-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="65bd6-128">Windows [10 cihazlarına yönelik](secure-win-10-pcs.md) ilkeleri ayarlamak için güvenli Windows 10 bilgisayarlarında adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="65bd6-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="65bd6-129">Bir Windows 10 cihazına Azure AD'ye katılsanız, Windows 10 bilgisayarlar için ayarınızdaki ilkeler bu cihaza uygulanır.</span><span class="sxs-lookup"><span data-stu-id="65bd6-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="65bd6-130">Daha fazla bilgi için bkz. [Microsoft 365 kullanıcıları](set-up-windows-devices.md)için Windows cihazlarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="65bd6-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="65bd6-131">4. Adım: Microsoft 365 İş Uygulamalarını yükleme</span><span class="sxs-lookup"><span data-stu-id="65bd6-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="65bd6-132">Kurulum sihirbazını kullanarak Windows cihazlarına Office'i otomatik [olarak yükleyebilirsiniz.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="65bd6-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="65bd6-133">Kullanıcıların Windows [ve cihazlar için Office](/office365/admin/setup/install-applications) uygulamalarını yüklemesine izin verin.</span><span class="sxs-lookup"><span data-stu-id="65bd6-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="65bd6-134">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="65bd6-134">Advanced</span></span>
- <span data-ttu-id="65bd6-135">**Yeni cihazları ayarlamak için Autopilot'a kullanma**</span><span class="sxs-lookup"><span data-stu-id="65bd6-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="65bd6-136">Kullanıcının yeni Windows 10 cihazlarını  otomatik olarak önceden yapılandırmak için [Windows Autopilot'u](add-autopilot-devices-and-profile.md) [](https://www.microsoft.com/solution-providers/search) kullanabilirsiniz, ancak bunu sizin için yapacak bir iş ortağını almak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="65bd6-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="65bd6-137">Ayrıca Microsoft [Store'a gidip](https://go.microsoft.com/fwlink/?linkid=874598)bir bulut teknolojisi uzmanının satın aldığınız yeni cihazları ayarlamalarını da sebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd6-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="65bd6-138">**Şirket içi kaynaklara erişme**</span><span class="sxs-lookup"><span data-stu-id="65bd6-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="65bd6-139">Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 İş Ekstra'nın ayarlamasını yaparken, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="65bd6-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="65bd6-140">Bu ayarı yapmak [için etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş Ekstra](manage-windows-devices.md) tarafından yönetilsin.</span><span class="sxs-lookup"><span data-stu-id="65bd6-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="65bd6-141">Tercih edilen yöntem budur ve bu durumdaki cihazlar Karma Azure AD'ye katılmış cihazlar olarak adlandırılan cihazlar.</span><span class="sxs-lookup"><span data-stu-id="65bd6-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="65bd6-142">İşletmenizin bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'si varsa, Azure AD'ye katılmış cihazlarınıza şu adımları takip edin: [Microsoft 365 Business Premium'da Azure AD'ye](access-resources.md)katılmış bir cihazdan şirket içi kaynaklara erişme.</span><span class="sxs-lookup"><span data-stu-id="65bd6-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="65bd6-143">Ayrıca bkz.</span><span class="sxs-lookup"><span data-stu-id="65bd6-143">See also</span></span>

[<span data-ttu-id="65bd6-144">İş için Microsoft 365 eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="65bd6-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)