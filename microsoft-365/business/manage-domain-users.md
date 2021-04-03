---
title: Etki alanı kullanıcılarını Microsoft 365'e eşitleme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Etki alanı denetimli kullanıcıları Microsoft 365 İş ile eşitler.
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578417"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="a90c1-103">Etki alanı kullanıcılarını Microsoft 365'e eşitleme</span><span class="sxs-lookup"><span data-stu-id="a90c1-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="a90c1-104">1. Dizin Eşitlemesi için Hazırlanma</span><span class="sxs-lookup"><span data-stu-id="a90c1-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="a90c1-105">Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanı'nden eşitlemeden [önce, Microsoft 365'e dizin eşitlemesi için hazırlanma'ya bakabilirsiniz.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="a90c1-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="a90c1-106">Özellikle:</span><span class="sxs-lookup"><span data-stu-id="a90c1-106">In particular:</span></span>

   - <span data-ttu-id="a90c1-107">Dizinde şu öznitelikler için hiçbir yinelemenin var olmadığını emin olun: **posta,** **proxyAddresses** ve **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="a90c1-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="a90c1-108">Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="a90c1-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="a90c1-109">Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini lisanslı Microsoft 365 kullanıcıya karşılık gelen birincil e-posta adresiyle eş olacak şekilde yapılandırmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="a90c1-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="a90c1-110">Örneğin:  *mary.shelley@contoso.com.local yerine mary@contoso.*</span><span class="sxs-lookup"><span data-stu-id="a90c1-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="a90c1-111">Active Directory etki alanı *.com* veya *.org* gibi İnternet'e yönlendirilebilir bir sonek yerine *.local* veya *.lan* gibi yönlendirilebilir olmayan bir sonekle bitiyorsa, önce dizin eşitlemesi için yönlendirilebilir olmayan bir etki alanını hazırlama konusunda açıklandığı gibi yerel kullanıcı hesaplarının UPN soneki [ayarlayın.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="a90c1-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="a90c1-112">Aşağıdaki dördüncü adımda (4) **IdFix** Çalıştır, şirket içi Active Directory'nizin dizin eşitlemesi için hazır olduğundan da emin olur.</span><span class="sxs-lookup"><span data-stu-id="a90c1-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="a90c1-113">2. Azure AD Connect'i yükleme ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="a90c1-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="a90c1-114">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'ye eşitlemek için, Azure Active Directory Connect'i yükleyin ve dizin eşitlemesini ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a90c1-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="a90c1-115">Yönetim [merkezinde, sol](https://go.microsoft.com/fwlink/p/?linkid=2024339) **gezintide** Kurulum'u seçin.</span><span class="sxs-lookup"><span data-stu-id="a90c1-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="a90c1-116">Oturum **açma ve güvenlik altında, oturum** açma **kullanıcılarınızı** **eşitle'nin altında Görüntüle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="a90c1-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="a90c1-117">Kuruluş dizin **sayfasından Kullanıcıları eşitle'yi** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="a90c1-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="a90c1-118">Dizin eşitlemeye hazırlanmak için ilk adımda IdFix aracını çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="a90c1-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="a90c1-119">Azure AD Connect'i indirmek ve etki alanı denetimli kullanıcılarınızı Microsoft 365'e eşitlemek için sihirbaz adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="a90c1-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="a90c1-120">Daha [fazla bilgi edinmek için Bkz. Microsoft 365 için dizin](../enterprise/set-up-directory-synchronization.md) eşitlemesini ayarlama.</span><span class="sxs-lookup"><span data-stu-id="a90c1-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="a90c1-121">Azure AD Connect'e yönelik seçeneklerinizi yapılandırarak, Parola Eşitlemeyi, Sorunsuz Çoklu  Oturum Açma özelliğini ve ayrıca Microsoft 365 İş'te de desteklenen parola geri yazma özelliğini etkinleştirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="a90c1-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="a90c1-122">Azure AD Connect'te parola geri yazma için bazı ek adımlar vardır.</span><span class="sxs-lookup"><span data-stu-id="a90c1-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="a90c1-123">Daha fazla bilgi için bkz. [Nasıl yapılandırılır: parola geri yazma.](/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="a90c1-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="a90c1-124">Etki alanına katılmış Windows 10 cihazlarını da yönetmek için bkz. Etki alanına katılmış [Windows 10 cihazlarını Microsoft 365 Business Premium](manage-windows-devices.md) tarafından yönetecek şekilde etkinleştirme ve karma Azure AD Join ayarlama.</span><span class="sxs-lookup"><span data-stu-id="a90c1-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>