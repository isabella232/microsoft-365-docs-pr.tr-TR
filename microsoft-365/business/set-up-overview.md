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
description: Microsoft 365 Business Premium için kurulum adımlarını, abone olmak, etki alanı ve kullanıcıları eklemeye, güvenlik ilkelerini ayarlamayı ve daha fazlasını öğrenin.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842140"
---
# <a name="overview-of-setup"></a><span data-ttu-id="28984-103">Kuruluma genel bakış</span><span class="sxs-lookup"><span data-stu-id="28984-103">Overview of setup</span></span>

<span data-ttu-id="28984-104">Microsoft 365 Business Premium kurulumu hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="28984-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="28984-105">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="28984-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="28984-106">Kurulum adımlarının çoğu Kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="28984-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="28984-107">Adım 1: etki alanınızı ve kullanıcılarınızı ekleme</span><span class="sxs-lookup"><span data-stu-id="28984-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="28984-108">**[Etki alanınızı ekleyin](set-up.md#add-your-domain-to-personalize-sign-in)** ( [kaydolma](sign-up.md)sırasında etki alanınızı satın aldıysanız, bu adım zaten yapılır.)</span><span class="sxs-lookup"><span data-stu-id="28984-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="28984-109">**Kullanıcıları ekleyin**.</span><span class="sxs-lookup"><span data-stu-id="28984-109">**Add users**.</span></span> <span data-ttu-id="28984-110">Kullanıcıları üç şekilde ekleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="28984-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="28984-111">[Kılavuzlu kurulumda](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="28984-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="28984-112">Şirket içi Active Directory 'niz varsa [Azure AD Connect 'i kullanarak kullanıcıları eklemek](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) için dizin eşitlemesi kullanın.</span><span class="sxs-lookup"><span data-stu-id="28984-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="28984-113">Ayrıca, [daha sonra Yönetim merkezinde kullanıcı ekleyebilirsiniz](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="28984-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="28984-114">Adım 2: güvenlik ilkelerini ayarlama ve cihazları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="28984-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="28984-115">Cihaz ilkelerini yapılandırmak için [Kılavuzlu kurulumu](set-up.md#protect-your-organization) kullanın.</span><span class="sxs-lookup"><span data-stu-id="28984-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="28984-116">Ayrıca, daha sonra [Yönetim merkezinde](view-policies-and-devices.md) ve [Intune portalında](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)daha fazla ekleyebilir veya düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="28984-117">Kurulum Sihirbazı ayrıca temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.</span><span class="sxs-lookup"><span data-stu-id="28984-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="28984-118">Kurulum sihirbazındaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="28984-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="28984-119">**Eposta koruması**</span><span class="sxs-lookup"><span data-stu-id="28984-119">**Email malware protection**</span></span>
- <span data-ttu-id="28984-120">**Office 365 Defender 'da kimlik avını önleme**</span><span class="sxs-lookup"><span data-stu-id="28984-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="28984-121">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="28984-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="28984-122">**Azure bilgi koruması (Plan1** )</span><span class="sxs-lookup"><span data-stu-id="28984-122">**Azure Information Protection (Plan1** )</span></span>

<span data-ttu-id="28984-123">Başlamak için [tehdit korumasını arttırın](increase-threat-protection.md) ve [uyumluluk özelliklerini ayarlayın](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="28984-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="28984-124">[Microsoft 365 Iş ekstra için güvenli](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) bir yol haritası-en iyi güvenlik uygulamaları</span><span class="sxs-lookup"><span data-stu-id="28984-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="28984-125">Adım 3: Windows 10 cihazlarını ayarlama ve yönetme</span><span class="sxs-lookup"><span data-stu-id="28984-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="28984-126">Kılavuzlu kurulumu tamamladıktan sonra, kuruluşunuzdaki tüm Windows 10 bilgisayarlarını korumanız gerekecektir.</span><span class="sxs-lookup"><span data-stu-id="28984-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="28984-127">Windows 10 Pro, Microsoft 365 Business Premium için bir [önkoşuldur](pre-requisites-for-data-protection.md) , ancak Windows 7 Pro, Windows 8 Pro veya Windows 8,1 Pro kullanıyorsanız, aboneliğiniz [Windows 10 Pro 'ya yükseltme](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)yapmanız aboneliğiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="28984-128">Windows 10 cihazlarında ilkeler ayarlamak için [Windows 10 bilgisayarlarında güvenli](secure-win-10-pcs.md) olan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="28984-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="28984-129">Windows 10 bilgisayarlarında bir Windows 10 aygıtına katıldığınızda, Windows 10 bilgisayarlarında ayarladığınız ilkeler buna uygulanır.</span><span class="sxs-lookup"><span data-stu-id="28984-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="28984-130">Daha fazla bilgi için bkz: [Microsoft 365 kullanıcıları Için Windows cihazları ayarlama](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="28984-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="28984-131">Adım 4: işletmeler için Microsoft 365 uygulamalarını yükleme</span><span class="sxs-lookup"><span data-stu-id="28984-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="28984-132">[Kurulum sihirbazını](set-up.md#deploy-office-365-client-apps)kullanarak Windows cihazlarında Office 'i otomatik olarak yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="28984-133">Kullanıcıların Windows için [Office uygulamalarını](https://docs.microsoft.com/office365/admin/setup/install-applications) ve aygıtlarını yüklemesini sağlayın.</span><span class="sxs-lookup"><span data-stu-id="28984-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="28984-134">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="28984-134">Advanced</span></span>
- <span data-ttu-id="28984-135">**Yeni cihazları ayarlamak için Autopilot 'ı kullanma**</span><span class="sxs-lookup"><span data-stu-id="28984-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="28984-136">[Windows Autopilot](add-autopilot-devices-and-profile.md) 'ı kullanarak bir kullanıcı için **Yeni** Windows 10 cihazlarını otomatik olarak yapılandırabilirsiniz, ancak bunu sizin için yapabileceği bir [iş ortağı](https://www.microsoft.com/solution-providers/search) almanız daha kolaydır.</span><span class="sxs-lookup"><span data-stu-id="28984-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="28984-137">Ayrıca, [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)'a gidebilir ve bir bulut teknoloji uzmanından satın aldığınız yeni cihazları kurulumunu isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="28984-138">**Şirket içi kaynaklara erişme**</span><span class="sxs-lookup"><span data-stu-id="28984-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="28984-139">Kuruluşunuzda Windows Server Active Directory 'yi şirket içinde kullanıyorsanız, Microsoft 365 Iş ekstra 'ı, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürmeye devam ederken Windows 10 aygıtlarınızı korumak için ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="28984-140">Bu ayarı ayarlamak için [etki alanı odaklı Windows 10 aygıtlarının Microsoft 365 Iş ekstra tarafından yönetilmesini sağlama](manage-windows-devices.md) konusundaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="28984-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="28984-141">Bu tercih edilen yöntemdir ve bu durumdaki cihazlar karma Azure AD birleştirilmiş cihazları olarak adlandırılır.</span><span class="sxs-lookup"><span data-stu-id="28984-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="28984-142">İşletmenizde bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory varsa, buradaki adımları izleyerek Azure AD-birleştirilmiş cihazlarınıza bu kaynaklara erişim sağlayabilirsiniz: [Microsoft 365 Business Premium 'Da Azure AD 'a katılmış cihazından şirket içi kaynaklara erişim](access-resources.md)sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28984-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="28984-143">Ayrıca bkz.</span><span class="sxs-lookup"><span data-stu-id="28984-143">See also</span></span>

[<span data-ttu-id="28984-144">Microsoft 365 iş eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="28984-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
