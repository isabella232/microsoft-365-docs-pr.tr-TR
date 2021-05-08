---
title: Kuruluma genel bakış
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Abone Microsoft 365 İş Ekstra, etki alanı ve kullanıcı eklemeye, güvenlik ilkelerini ayarlamaya ve daha fazlası için kurulum adımlarını öğrenin.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245074"
---
# <a name="overview-of-setup"></a><span data-ttu-id="895a5-103">Kuruluma genel bakış</span><span class="sxs-lookup"><span data-stu-id="895a5-103">Overview of setup</span></span>

<span data-ttu-id="895a5-104">Kurulum hakkında kısa bir Microsoft 365 İş Ekstra izleyin.</span><span class="sxs-lookup"><span data-stu-id="895a5-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="895a5-105">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="895a5-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>

<span data-ttu-id="895a5-106">Kurulum adımlarının çoğu kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenmiştir.</span><span class="sxs-lookup"><span data-stu-id="895a5-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="895a5-107">1. Adım: Etki alanınızı ve kullanıcılarınızı ekleme</span><span class="sxs-lookup"><span data-stu-id="895a5-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="895a5-108">**[Etki alanınızı](set-up.md#add-your-domain-to-personalize-sign-in)** ekleyin (etki alanınızı kaydol sırasında [satın aldıysanız,](sign-up.md)bu adım zaten bitti.)</span><span class="sxs-lookup"><span data-stu-id="895a5-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="895a5-109">**Kullanıcı ekle 'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="895a5-109">**Add users**.</span></span> <span data-ttu-id="895a5-110">Kullanıcıları şu üç şekilde ebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="895a5-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="895a5-111">Kılavuzlu [kurulumda](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="895a5-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="895a5-112">Şirket içi Active [directory'niz varsa, Azure AD Bağlan](../enterprise/set-up-directory-synchronization.md) kullanarak kullanıcıları eklemek için dizin eşitlemesini kullanın.</span><span class="sxs-lookup"><span data-stu-id="895a5-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="895a5-113">Kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="895a5-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="895a5-114">2. Adım: Güvenlik ilkelerini ayarlama ve cihazları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="895a5-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="895a5-115">Cihaz ilkelerini [yapılandırmak için](set-up.md#protect-your-organization) kılavuzlu kurulumu kullanın.</span><span class="sxs-lookup"><span data-stu-id="895a5-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="895a5-116">Ayrıca daha sonra yönetim merkezinde ve Intune [portalında](view-policies-and-devices.md) daha fazla ekleyebilir veya [bunları düzenleyebilirsiniz.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="895a5-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="895a5-117">Kurulum sihirbazı, temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.</span><span class="sxs-lookup"><span data-stu-id="895a5-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="895a5-118">Kurulum sihirbazında güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="895a5-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="895a5-119">**E-posta kötü amaçlı yazılıma karşı koruma**</span><span class="sxs-lookup"><span data-stu-id="895a5-119">**Email malware protection**</span></span>
- <span data-ttu-id="895a5-120">**Kimlik avı için Defender'da kimlik Office 365**</span><span class="sxs-lookup"><span data-stu-id="895a5-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="895a5-121">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="895a5-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="895a5-122">**Azure Information Protection (Plan1)**</span><span class="sxs-lookup"><span data-stu-id="895a5-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="895a5-123">Bunun için bkz. [tehdit korumasını artırma](increase-threat-protection.md) [ve uyumluluk özelliklerini ayarlama.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="895a5-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="895a5-124">Ayrıca, en iyi güvenlik uygulamalarının yol haritası için Microsoft 365 İş Ekstra en iyi [10](/office365/admin/security-and-compliance/secure-your-business-data) güvenlik yolunu da inceleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="895a5-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="895a5-125">3. Adım: Cihazlarınızı ayarlama Windows 10 yönetme</span><span class="sxs-lookup"><span data-stu-id="895a5-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="895a5-126">Rehberli kurulumu tamamlandıktan sonra, tüm bilgisayarlarınızı ve Windows 10 korumanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="895a5-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="895a5-127">Windows 10 Pro, Microsoft 365 İş Ekstra'in [](pre-requisites-for-data-protection.md) önkoşullarıdır, ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'niz varsa, aboneliğiniz size Windows 10 Pro yükseltme [hakkı Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="895a5-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="895a5-128">Mobil cihazlara yönelik [ilkeleri Windows 10 için güvenli](secure-win-10-pcs.md) bilgisayarlardaki Windows 10 izleyin.</span><span class="sxs-lookup"><span data-stu-id="895a5-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="895a5-129">bir Windows 10 Azure AD'ye katılsanız, bu cihaza Windows 10 ilkeler uygulanır.</span><span class="sxs-lookup"><span data-stu-id="895a5-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="895a5-130">Daha fazla bilgi için [bkz. Windows için cihaz Microsoft 365 ayarlama](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="895a5-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="895a5-131">4. Adım: Yükleme İş için Microsoft 365 Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="895a5-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="895a5-132">Kurulum sihirbazını Office bilgisayarınıza Windows bilgisayarınıza otomatik [olarak yükleyebilirsiniz.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="895a5-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="895a5-133">Kullanıcıların [e-Office cihazlar için](/office365/admin/setup/install-applications) Windows uygulamaları yüklemesine izin verin.</span><span class="sxs-lookup"><span data-stu-id="895a5-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="895a5-134">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="895a5-134">Advanced</span></span>
- <span data-ttu-id="895a5-135">**Yeni cihazları ayarlamak için AutoPilot'i kullanma**</span><span class="sxs-lookup"><span data-stu-id="895a5-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="895a5-136">Bir kullanıcının yeni Windows cihazlarını otomatik olarak  Windows 10 için [AutoPilot'a](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin [](https://www.microsoft.com/solution-providers/search) için yapacak bir iş ortağını almak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="895a5-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="895a5-137">Ayrıca Microsoft Store ['a](https://go.microsoft.com/fwlink/?linkid=874598)gidebilir ve bir bulut teknolojisi uzmanının satın aldığınız yeni cihazları ayarlamalarını sorabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="895a5-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="895a5-138">**Şirket içi access kaynakları**</span><span class="sxs-lookup"><span data-stu-id="895a5-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="895a5-139">Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Microsoft 365 İş Ekstra cihazlarınızı korumak için Windows 10'i kurabilirsiniz ve bu sırada yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="895a5-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="895a5-140">Bu özelliği ayarlamak [için Etki alanına katılmış Windows 10 cihazlarını bu cihazlar](manage-windows-devices.md) tarafından Microsoft 365 İş Ekstra adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="895a5-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="895a5-141">Bu tercih edilen yöntemdir ve bu durumdaki cihazlar Karma Azure AD'ye katılmış cihazlar olarak adlandırılan cihazlar.</span><span class="sxs-lookup"><span data-stu-id="895a5-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="895a5-142">İşletmenizin bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'niz varsa, Azure AD'ye katılmış cihazlarınıza şu adımları takip edin: [Microsoft 365 İş Ekstra'te Azure AD'ye](access-resources.md)katılmış bir cihazdan şirket içi kaynaklara erişme .</span><span class="sxs-lookup"><span data-stu-id="895a5-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="related-content"></a><span data-ttu-id="895a5-143">İlgili içerik</span><span class="sxs-lookup"><span data-stu-id="895a5-143">Related content</span></span>

<span data-ttu-id="895a5-144">[Microsoft 365 eğitim videoları için giriş](../business-video/index.yml) (bağlantı sayfası)</span><span class="sxs-lookup"><span data-stu-id="895a5-144">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>