---
title: Microsoft 365 kampanyalar için koşullu erişim ilkeleri ayarlama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
description: Koşullu erişim ilkelerini kurmak için Microsoft 365 Kampanyalar öğrenin.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086419"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="08fdb-103">Koşullu erişim ilkelerini kurun</span><span class="sxs-lookup"><span data-stu-id="08fdb-103">Set up conditional access policies</span></span>

<span data-ttu-id="08fdb-104">[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri substancial ek güvenlik ekleyin.</span><span class="sxs-lookup"><span data-stu-id="08fdb-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="08fdb-105">Microsoft, tüm müşteriler için önerilen temel koşullu erişim ilkeleri kümesi sağlar.</span><span class="sxs-lookup"><span data-stu-id="08fdb-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="08fdb-106">Temel ilkeleri kuruluşlar birçok ortak saldırılara karşı korunmasına yardımcı olmak önceden tanımlanan ilkeler bir kümesidir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="08fdb-107">Bu ortak saldırıları parola sprey, replay ve kimlik avı dahil edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="08fdb-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="08fdb-108">Bu ilkeler Yöneticiler ve kullanıcıların ikinci bir form kimlik doğrulaması (çok faktörlü kimlik doğrulama veya MFA denir) girmesini gerektiren zaman koşullar.</span><span class="sxs-lookup"><span data-stu-id="08fdb-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="08fdb-109">Örneğin, bir kullanıcı farklı bir ülkeden oturum açma, oturum riskli olarak kabul edilebilir ve kullanıcı başka bir kimlik doğrulama biçimi sağlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="08fdb-110">Şu anda, temel ilkeleri şunlardır:</span><span class="sxs-lookup"><span data-stu-id="08fdb-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="08fdb-111">**Yöneticileri için MFA gerektirir** — genel yönetici de dahil olmak üzere en yüksek ayrıcalıklı yönetici rolleri çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="08fdb-112">**Son kullanıcı koruması** — bir işareti de risklidir yalnızca kullanıcılar için çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="08fdb-113">**Eski kimlik bloğunu** — eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli kimlik doğrulama protokollerini kullanma.</span><span class="sxs-lookup"><span data-stu-id="08fdb-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="08fdb-114">Bu eski uygulamaların, koşullu erişim ilkelerini devre dışı bırakabilir ve ortamınızı yetkisiz erişim.</span><span class="sxs-lookup"><span data-stu-id="08fdb-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="08fdb-115">Bu ilke erişimi engeller koşullu erişim desteklemeyen istemcilerden gelen.</span><span class="sxs-lookup"><span data-stu-id="08fdb-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="08fdb-116">**Servis Yönetimi için gerekli MFA** — erişim için yönetim araçlarını (Burada yapılandırdığınız temel ilkeleri) Azure portal dahil olmak üzere, çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="08fdb-117">Microsoft, bu temel ilkelerini etkinleştir önerir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="08fdb-118">Bu ilkeler etkinleştirildikten sonra Yöneticiler ve kullanıcılar Azure Multii faktörlü kimlik doğrulama için kaydetmek için istenir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="08fdb-119">Bu ilkeler hakkında daha fazla bilgi için bkz: [temel ilkeleri nelerdir](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="08fdb-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="08fdb-120">Temel ilkelerini kurun</span><span class="sxs-lookup"><span data-stu-id="08fdb-120">Set up baseline policies</span></span>

1. <span data-ttu-id="08fdb-121">[Azure portalı](https://portal.azure.com)' na gidin ve sonra **Active Directory Azure** gidin \> **Koşullu erişim**.</span><span class="sxs-lookup"><span data-stu-id="08fdb-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="08fdb-122">Temel ilkeleri sayfasında listelenir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="08fdb-123">![Koşullu erişim için temel ilkelerini listeler sayfası.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="08fdb-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="08fdb-124">Her ilke için aşağıdaki özel yönergelere bakın:</span><span class="sxs-lookup"><span data-stu-id="08fdb-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="08fdb-125">MFA Yöneticiler için gerektirir.</span><span class="sxs-lookup"><span data-stu-id="08fdb-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="08fdb-126">Reequire MFA kullanıcılar için</span><span class="sxs-lookup"><span data-stu-id="08fdb-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="08fdb-127">Blok eski kimlik doğrulaması</span><span class="sxs-lookup"><span data-stu-id="08fdb-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="08fdb-128">MFA Hizmeti Yönetimi için gerekli</span><span class="sxs-lookup"><span data-stu-id="08fdb-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="08fdb-129">Onaylanmış istemci uygulamaları gerektiren gibi birçok ek ilkeler ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="08fdb-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="08fdb-130">Daha fazla bilgi için [Koşullu erişim belgelerine](https://docs.microsoft.com/azure/active-directory/conditional-access/) bakın.</span><span class="sxs-lookup"><span data-stu-id="08fdb-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>