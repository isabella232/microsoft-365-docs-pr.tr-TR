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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business Premium için abone olmaktan etki alanı ve kullanıcı eklemeye, güvenlik ilkeleri ayarlamaya ve daha fazlasına kadar kurulum adımlarını öğrenin.
ms.openlocfilehash: 8b26d423d4f62ee8f9ea4a61eb8f7efa72ee26cb
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633365"
---
# <a name="overview-of-setup"></a><span data-ttu-id="daa60-103">Kuruluma genel bakış</span><span class="sxs-lookup"><span data-stu-id="daa60-103">Overview of setup</span></span>

<span data-ttu-id="daa60-104">Microsoft 365 Business Premium kurulumu hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="daa60-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="daa60-105">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).  </span><span class="sxs-lookup"><span data-stu-id="daa60-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="daa60-106">Kurulum adımlarının çoğu kurulum sihirbazında yapılabilir, ancak diğer seçenekler de listelenir.</span><span class="sxs-lookup"><span data-stu-id="daa60-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="daa60-107">Adım 1: Etki alanınızı ve kullanıcılarınızı ekleyin</span><span class="sxs-lookup"><span data-stu-id="daa60-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="daa60-108">**[Etki alanınızı ekleyin](set-up.md#add-your-domain-to-personalize-sign-in)** [(kaydolma](sign-up.md)sırasında etki alanınızı satın aldıysanız, bu adım zaten tamamlanır.)</span><span class="sxs-lookup"><span data-stu-id="daa60-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="daa60-109">**Kullanıcı ekle.**</span><span class="sxs-lookup"><span data-stu-id="daa60-109">**Add users**.</span></span> <span data-ttu-id="daa60-110">Kullanıcıları üç şekilde ekleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="daa60-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="daa60-111">[Büyücüde.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="daa60-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="daa60-112">Şirket içinde Etkin dizininiz varsa [Azure AD Connect'i kullanarak kullanıcıları eklemek](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) için dizin eşitlemesi kullanın.</span><span class="sxs-lookup"><span data-stu-id="daa60-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="daa60-113">Daha sonra yönetici merkezine [de kullanıcı ekleyebilirsiniz.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="daa60-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="daa60-114">Adım 2: Güvenlik ilkeleri ayarlama ve aygıtları yapılandırma</span><span class="sxs-lookup"><span data-stu-id="daa60-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="daa60-115">Aygıt ilkelerini yapılandırmak için [Kurulum sihirbazını](set-up.md#protect-your-organization) kullanın.</span><span class="sxs-lookup"><span data-stu-id="daa60-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="daa60-116">Ayrıca daha fazla ekleyebilir veya daha sonra [yönetici merkezinde](view-policies-and-devices.md) ve [Intune portalında](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)bunları edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="daa60-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="daa60-117">Kurulum sihirbazı ayrıca temel tehdit koruması ve veri kaybıönleme ayarlarını da ayarlar.</span><span class="sxs-lookup"><span data-stu-id="daa60-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="daa60-118">Kurulum sihirbazındaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="daa60-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="daa60-119">**Kötü amaçlı yazılımkoruması e-postayla gönder**</span><span class="sxs-lookup"><span data-stu-id="daa60-119">**Email malware protection**</span></span>
- <span data-ttu-id="daa60-120">**ATP kimlik avı önleme**</span><span class="sxs-lookup"><span data-stu-id="daa60-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="daa60-121">**Exchange Online Arşivleme**</span><span class="sxs-lookup"><span data-stu-id="daa60-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="daa60-122">**Azure Bilgi Koruması (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="daa60-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="daa60-123">Başlamak için [tehdit korumasını artırın](increase-threat-protection.md) ve [uyumluluk özelliklerini ayarlayın.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="daa60-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="daa60-124">Microsoft [365 Business Premium'unuzu](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) en iyi güvenlik uygulamalarının yol haritası için güvence altına almanın en iyi 10 yolunu da görün.</span><span class="sxs-lookup"><span data-stu-id="daa60-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="daa60-125">Adım 3: Windows 10 aygıtlarını ayarlama ve yönetme</span><span class="sxs-lookup"><span data-stu-id="daa60-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="daa60-126">Kurulum sihirbazını çalıştırdıktan sonra, kuruluşunuzdaki tüm Windwos 10 bilgisayarlarını çalıştırmak isteyeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="daa60-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="daa60-127">Windows 10 Pro, Microsoft 365 Business Premium için bir [ön koşuldur,](pre-requisites-for-data-protection.md) ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'nuz varsa, aboneliğiniz size [Windows 10 Pro'ya yükseltme](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)hakkı verir.</span><span class="sxs-lookup"><span data-stu-id="daa60-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="daa60-128">Windows 10 aygıtları için ilkeler ayarlamak için [güvenli Windows 10 bilgisayarlarındaki](secure-win-10-pcs.md) adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="daa60-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="daa60-129">Bir Windows 10 aygıtına Azure AD'ye katıldığınızda, Windows 10 bilgisayarlar için belirlediğiniz ilkeler uygulanır.</span><span class="sxs-lookup"><span data-stu-id="daa60-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="daa60-130">Daha fazla bilgi için [bkz.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="daa60-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="daa60-131">Adım 4: İşletmeler için Microsoft 365 Uygulamalarını yükleyin</span><span class="sxs-lookup"><span data-stu-id="daa60-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="daa60-132">[Kurulum sihirbazını](set-up.md#deploy-office-365-client-apps)kullanarak Office'i Windows aygıtlarına otomatik olarak yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="daa60-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="daa60-133">Kullanıcıların Windows ve aygıtlar için [Office uygulamalarını yüklemesine](https://docs.microsoft.com/office365/admin/setup/install-applications) izin verin.</span><span class="sxs-lookup"><span data-stu-id="daa60-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="daa60-134">Gelişmiş</span><span class="sxs-lookup"><span data-stu-id="daa60-134">Advanced</span></span>
- <span data-ttu-id="daa60-135">**Yeni aygıtlar kurmak için Otomatik Pilot'u kullanma**</span><span class="sxs-lookup"><span data-stu-id="daa60-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="daa60-136">Bir kullanıcı için **yeni** Windows 10 aygıtlarını otomatik olarak önceden yapılandırmak için [Windows Otomatik Pilot'u](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin için yapabilecek bir [iş ortağı](https://www.microsoft.com/solution-providers/search) bulmak daha kolay olabilir.</span><span class="sxs-lookup"><span data-stu-id="daa60-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="daa60-137">Microsoft [Mağazası'na](https://go.microsoft.com/fwlink/?linkid=874598)da gidebilir ve bir bulut teknolojisi uzmanından satın aldığınız yeni aygıtlar ayarlamasını isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="daa60-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="daa60-138">**Şirket içi kaynaklara erişim**</span><span class="sxs-lookup"><span data-stu-id="daa60-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="daa60-139">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="daa60-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="daa60-140">Bunu ayarlamak için [Microsoft 365 Business Premium tarafından yönetilecek etki alanına birleştirilmiş Windows 10 aygıtlarını etkinleştirme](manage-windows-devices.md) adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="daa60-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="daa60-141">Bu tercih edilen yöntemdir ve bu durumdaki aygıtlar Karma Azure AD birleştirilmiş aygıtlar olarak adlandırılır.</span><span class="sxs-lookup"><span data-stu-id="daa60-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="daa60-142">İşletmenizde bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Etkin Dizin varsa, Azure AD'ye katılan aygıtlarınıza buradaki adımları izleyerek bu kaynaklara erişim sağlayabilirsiniz: [Microsoft 365 Business Premium'daki Azure AD'ye bağlı bir aygıttan şirket içi kaynaklara erişin.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="daa60-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="daa60-143">Ayrıca bkz.</span><span class="sxs-lookup"><span data-stu-id="daa60-143">See also</span></span>

[<span data-ttu-id="daa60-144">İş eğitimi videoları için Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="daa60-144">Microsoft 365 for business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
