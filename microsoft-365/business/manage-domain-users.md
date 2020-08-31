---
title: Etki alanı kullanıcılarını Microsoft 365 ile eşitleme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Etki alanı denetimli kullanıcıları Microsoft 365 iş ile eşitleyin.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306459"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="275a7-103">Etki alanı kullanıcılarını Microsoft 365 ile eşitleme</span><span class="sxs-lookup"><span data-stu-id="275a7-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="275a7-104">1. Dizin eşitlemeye hazırlanma</span><span class="sxs-lookup"><span data-stu-id="275a7-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="275a7-105">Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory etki alanından eşitlemeden önce, [Microsoft 365 ile dizin eşitlemesi hazırlığı](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="275a7-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="275a7-106">Özellikle:</span><span class="sxs-lookup"><span data-stu-id="275a7-106">In particular:</span></span>

   - <span data-ttu-id="275a7-107">Aşağıdaki öznitelikler için dizininizde hiçbir çoğaltma bulunmadığından emin olun: **posta**, **proxyAddresses**ve **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="275a7-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="275a7-108">Bu değerlerin benzersiz olması ve tüm çoğaltmaların kaldırılması gerekir.</span><span class="sxs-lookup"><span data-stu-id="275a7-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="275a7-109">Her yerel kullanıcı hesabının **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="275a7-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="275a7-110">Örneğin: *Mary@contoso. yerel* yerine *Mary.Shelley@contoso.com*</span><span class="sxs-lookup"><span data-stu-id="275a7-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="275a7-111">Active Directory etki *alanı,.* com veya. org gibi internet yönlendirilebilir soneki yerine *,.* *com* veya *. org*gibi yönlendirilemeyen bir sonek içinde sona erdiğinde, [Dizin eşitlemesi için yönlendirilemeyen bir etki ALANıNı hazırlama](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)başlığı altında açıklandığı gibi yerel kullanıcı hesaplarının UPN sonekini ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="275a7-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="275a7-112">Aşağıdaki dört (4) adımdaki **Run Idfıx** , şirket Içi Active Directory 'nin dır eşitlemesi için hazır olduğundan emin olur.</span><span class="sxs-lookup"><span data-stu-id="275a7-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="275a7-113">2. Azure AD Connect 'i yükleme ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="275a7-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="275a7-114">Kullanıcıları, grupları ve kişilerinizi yerel Active Directory 'den Azure Active Directory 'ye eşitlemek için Azure Active Directory Connect 'i yükleyin ve dizin eşitlemesini ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="275a7-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="275a7-115">Yönetim merkezinde, sol gezintide <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Kurulum 'u** seçin.</span><span class="sxs-lookup"><span data-stu-id="275a7-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="275a7-116">**Oturum açma ve güvenlik**altında, **kuruluşunuzun dizininden kullanıcıları Eşitle**altında **Görünüm** 'ü seçin.</span><span class="sxs-lookup"><span data-stu-id="275a7-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="275a7-117">Kullanıcıları kuruluşunuzun **dizininden Eşitle** sayfasında **başlayın**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="275a7-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="275a7-118">Dizin eşitlemeye hazırlanmak için ilk adım çalışma IdFix aracında.</span><span class="sxs-lookup"><span data-stu-id="275a7-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="275a7-119">Sihirbazın adımlarını kullanarak Azure AD Connect 'i indirin ve etki alanı denetimli kullanıcılarınızı Microsoft 365 ile eşitlemek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="275a7-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="275a7-120">Daha fazla bilgi edinmek için [Microsoft 365 için dizin eşitlemesini ayarlayın](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .</span><span class="sxs-lookup"><span data-stu-id="275a7-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="275a7-121">Azure AD Connect için seçeneklerinizi yapılandırırken, **parola eşitleme**, **kesintisiz çoklu oturum açma**ve **parola geri yazma** özelliğini etkinleştirmenizi öneririz, bu da Microsoft 365 iş için desteklenmektedir.</span><span class="sxs-lookup"><span data-stu-id="275a7-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="275a7-122">Azure AD Connect 'teki denetim kutusunun ötesinde parola geri yazma için bazı ek adımlar vardır.</span><span class="sxs-lookup"><span data-stu-id="275a7-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="275a7-123">Daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="275a7-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="275a7-124">Etki alanına bağlı Windows 10 cihazlarını da yönetmek istiyorsanız, karma Azure AD birleştirmeyi ayarlamak için [etki alanına bağlı Windows 10 cihazlarını Microsoft 365 Business Premium tarafından yönetilecek şekilde etkinleştirme](manage-windows-devices.md) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="275a7-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 