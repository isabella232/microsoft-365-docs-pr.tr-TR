---
title: Microsoft 365 kampanyaları için koşullu erişim ilkeleri ayarlama
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Önemli ölçüde ek güvenlik eklemek için Microsoft 365 Kampanyaları için koşullu erişim ilkeleri nasıl ayarlayabilirsiniz öğrenin.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470657"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="05f81-103">Koşullu erişim ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="05f81-103">Set up conditional access policies</span></span>

<span data-ttu-id="05f81-104">Bu makale Microsoft 365 Business Premium için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="05f81-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="05f81-105">[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri önemli ölçüde ek güvenlik ekler.</span><span class="sxs-lookup"><span data-stu-id="05f81-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="05f81-106">Microsoft, tüm müşteriler için önerilen bir temel koşullu erişim ilkeleri kümesi sağlar.</span><span class="sxs-lookup"><span data-stu-id="05f81-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="05f81-107">Temel ilkeler, kuruluşların birçok yaygın saldırıya karşı korunmasına yardımcı olan önceden tanımlanmış ilkeler kümesidir.</span><span class="sxs-lookup"><span data-stu-id="05f81-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="05f81-108">Bu yaygın saldırılar parola püskürtme, yeniden oynatma ve kimlik avı içerebilir.</span><span class="sxs-lookup"><span data-stu-id="05f81-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="05f81-109">Bu ilkeler, belirli koşullar yerine getirildiğinde yöneticilerin ve kullanıcıların ikinci bir kimlik doğrulama biçimi (çok faktörlü kimlik doğrulama veya MFA olarak adlandırılır) girmesini gerektirir.</span><span class="sxs-lookup"><span data-stu-id="05f81-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="05f81-110">Örneğin, bir kullanıcı farklı bir ülkeden oturum veriyorsa, oturum açma riskli kabul edilebilir ve kullanıcının ek bir kimlik doğrulama biçimi sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="05f81-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="05f81-111">Şu anda, temel ilkeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="05f81-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="05f81-112">Yöneticiler için **MFA gerektirir** &ndash; Genel yönetici de dahil olmak üzere en ayrıcalıklı yönetici rolleri için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="05f81-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="05f81-113">**Son kullanıcı koruması** &ndash; Yalnızca oturum açma riskli olduğunda kullanıcılar için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="05f81-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="05f81-114">**Eski kimlik doğrulamasını** &ndash; engelleme Eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli, kimlik doğrulama protokolleri kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="05f81-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="05f81-115">Bu eski uygulamalar koşullu erişim ilkelerini atlayabilir ve ortamınıza yetkisiz erişim elde edebilir.</span><span class="sxs-lookup"><span data-stu-id="05f81-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="05f81-116">Bu ilke, koşullu erişimi desteklemeyen istemcilerin erişimini engeller.</span><span class="sxs-lookup"><span data-stu-id="05f81-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="05f81-117">**Hizmet Yönetimi** &ndash; için MFA Gerektirir Azure portalı (temel ilkeleri yapılandırdığınız yer) dahil olmak üzere yönetim araçlarına erişmek için çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="05f81-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="05f81-118">Microsoft, bu temel ilkelerin tümünün etkinleştirilmesini önerir.</span><span class="sxs-lookup"><span data-stu-id="05f81-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="05f81-119">Bu ilkeler etkinleştirildikten sonra, yöneticilerden ve kullanıcılardan Azure Multii-Factor kimlik doğrulaması için kaydolması istenir.</span><span class="sxs-lookup"><span data-stu-id="05f81-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="05f81-120">Bu ilkeler hakkında daha fazla bilgi için [temel ilkeler nelerdir?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="05f81-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="05f81-121">Temel ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="05f81-121">Set up baseline policies</span></span>

1. <span data-ttu-id="05f81-122">Azure [portalına](https://portal.azure.com)gidin ve ardından **Azure Etkin Dizin** \> **Koşullu Erişim'e**gidin.</span><span class="sxs-lookup"><span data-stu-id="05f81-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="05f81-123">Temel ilkeler sayfada listelenir.</span><span class="sxs-lookup"><span data-stu-id="05f81-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="05f81-124">![Koşullu erişim için temel ilkeleri listeleyen sayfa.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="05f81-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="05f81-125">Her ilke için aşağıdaki özel yönergeye bakın:</span><span class="sxs-lookup"><span data-stu-id="05f81-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="05f81-126">Yöneticiler için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="05f81-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="05f81-127">Kullanıcılar için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="05f81-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="05f81-128">Eski kimlik doğrulamasını engelleme</span><span class="sxs-lookup"><span data-stu-id="05f81-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="05f81-129">Hizmet yönetimi için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="05f81-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="05f81-130">Onaylı istemci uygulamaları gerektirmek gibi birçok ek ilke ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="05f81-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="05f81-131">Daha fazla bilgi için [Koşullu Erişim Belgeleri'ne](https://docs.microsoft.com/azure/active-directory/conditional-access/)bakın.</span><span class="sxs-lookup"><span data-stu-id="05f81-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
