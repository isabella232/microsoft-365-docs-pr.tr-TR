---
title: Etki alanı kullanıcılarını Microsoft 365 ile senkronize etme
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
description: Etki alanı denetimli kullanıcıları iş için Microsoft 365 ile senkronize edin.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081931"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="39b55-103">Etki alanı kullanıcılarını Microsoft 365 ile senkronize etme</span><span class="sxs-lookup"><span data-stu-id="39b55-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="39b55-104">1. Dizin Senkronizasyonuna Hazırla</span><span class="sxs-lookup"><span data-stu-id="39b55-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="39b55-105">Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden önce, [Microsoft 365'e dizin eşitlemesi için hazırlayın'ı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="39b55-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="39b55-106">Özellikle:</span><span class="sxs-lookup"><span data-stu-id="39b55-106">In particular:</span></span>

   - <span data-ttu-id="39b55-107">Aşağıdaki öznitelikler için dizininizde yineleme olmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="39b55-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="39b55-108">Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="39b55-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="39b55-109">Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="39b55-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="39b55-110">Örneğin: *mary@contoso.yerel* yerine *mary.shelley@contoso.com*</span><span class="sxs-lookup"><span data-stu-id="39b55-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="39b55-111">Active Directory etki alanı *.com* veya *.org*gibi bir internet routable sonek yerine *.local* veya *.lan*gibi bir routable olmayan sonek biterse, önce yerel kullanıcı hesaplarının UPN sonekini [dizin eşitleme için routable olmayan bir etki alanı hazırlayın'da](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)açıklandığı gibi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="39b55-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="39b55-112">Aşağıdaki adım dört (4) adımdaki **Run IdFix,** şirket içi Active Directory'nizin dir senkronizasyonuna hazır olduğundan da emin olacaktır.</span><span class="sxs-lookup"><span data-stu-id="39b55-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="39b55-113">2. Azure AD Connect'i yükleme ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="39b55-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="39b55-114">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'i yükleyin ve dizin eşitlemesi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="39b55-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="39b55-115"><a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>Sol daki **Kurulum'u** seçin'deki yönetici merkezinde.</span><span class="sxs-lookup"><span data-stu-id="39b55-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="39b55-116">**Oturum Açma ve güvenlik**altında, org **dizininizdeki Eşitleme kullanıcıları**altında **Görüntüle'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="39b55-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="39b55-117">**Org'unuzun dizin sayfasındaki Eşitleme kullanıcıları** üzerinde **Başlat'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="39b55-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="39b55-118">İlk adımda Dizin eşitleme için hazırlamak için IdFix aracı çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="39b55-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="39b55-119">Azure AD Connect'i indirmek ve etki alanı denetimindeki kullanıcılarınızı Microsoft 365 ile senkronize etmek için kullanmak için sihirbaz adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="39b55-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="39b55-120">Bkz. Daha fazla bilgi edinmek [için Microsoft 365 için dizin eşitlemesi ayarla.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="39b55-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="39b55-121">Azure AD Connect seçeneklerinizi yapılandırırken, İş için Microsoft 365'te de desteklenen **Parola Eşitleme**, **Kesintisiz Tek Oturum**Açma ve parola **yazma** özelliğini etkinleştirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="39b55-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="39b55-122">Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır.</span><span class="sxs-lookup"><span data-stu-id="39b55-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="39b55-123">Daha fazla bilgi için [bkz: Nasıl Yapılır: parola yazmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="39b55-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="39b55-124">Etki alanına bağlı Windows 10 aygıtlarını da yönetmek istiyorsanız, [bkz.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="39b55-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 