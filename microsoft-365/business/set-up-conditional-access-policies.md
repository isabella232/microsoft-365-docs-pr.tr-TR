---
title: Microsoft 365 kampanyaları için koşullu erişim ilkeleri ayarlama
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
description: Microsoft 365 Kampanyaları için koşullu erişim ilkeleri nasıl ayarlayabilirsiniz öğrenin.
ms.openlocfilehash: 614e3a6e13a14114f40ecf87bf936d4165744503
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982391"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="d5a40-103">Koşullu erişim ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="d5a40-103">Set up conditional access policies</span></span>

<span data-ttu-id="d5a40-104">[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri, yedek ek güvenlik ekler.</span><span class="sxs-lookup"><span data-stu-id="d5a40-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="d5a40-105">Microsoft, tüm müşteriler için önerilen bir temel koşullu erişim ilkeleri kümesi sağlar.</span><span class="sxs-lookup"><span data-stu-id="d5a40-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="d5a40-106">Temel ilkeler, kuruluşların birçok yaygın saldırıya karşı korunmasına yardımcı olan önceden tanımlanmış ilkeler kümesidir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="d5a40-107">Bu yaygın saldırılar parola püskürtme, yeniden oynatma ve kimlik avı içerebilir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="d5a40-108">Bu ilkeler, belirli koşullar yerine getirildiğinde yöneticilerin ve kullanıcıların ikinci bir kimlik doğrulama biçimi (çok faktörlü kimlik doğrulama veya MFA olarak adlandırılır) girmesini gerektirir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="d5a40-109">Örneğin, bir kullanıcı farklı bir ülkeden oturum veriyorsa, oturum açma riskli kabul edilebilir ve kullanıcının ek bir kimlik doğrulama biçimi sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="d5a40-110">Şu anda, temel ilkeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="d5a40-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="d5a40-111">**Yöneticiler için MFA gerektirir** — Genel yönetici de dahil olmak üzere en ayrıcalıklı yönetici rolleri için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="d5a40-112">**Son kullanıcı koruması** — Yalnızca oturum açma riskli olduğunda kullanıcılar için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="d5a40-113">**Eski kimlik doğrulamayı engelleyin** — Eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli, kimlik doğrulama protokolleri kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="d5a40-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="d5a40-114">Bu eski uygulamalar koşullu erişim ilkelerini atlayabilir ve ortamınıza yetkisiz erişim elde edebilir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="d5a40-115">Bu ilke, koşullu erişimi desteklemeyen istemcilerin erişimini engeller.</span><span class="sxs-lookup"><span data-stu-id="d5a40-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="d5a40-116">**Hizmet Yönetimi için MFA Gerektirir** — Azure portalı (temel ilkeleri yapılandırdığınız yer) dahil olmak üzere yönetim araçlarına erişmek için çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="d5a40-117">Microsoft, bu temel ilkelerin tümünün etkinleştirilmesini önerir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="d5a40-118">Bu ilkeler etkinleştirildikten sonra, yöneticilerden ve kullanıcılardan Azure Multii-Factor kimlik doğrulaması için kaydolması istenir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="d5a40-119">Bu ilkeler hakkında daha fazla bilgi için [temel ilkeler nelerdir?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="d5a40-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="d5a40-120">Temel ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="d5a40-120">Set up baseline policies</span></span>

1. <span data-ttu-id="d5a40-121">Azure [portalına](https://portal.azure.com)gidin ve ardından **Azure Etkin Dizin** \> **Koşullu Erişim'e**gidin.</span><span class="sxs-lookup"><span data-stu-id="d5a40-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="d5a40-122">Temel ilkeler sayfada listelenir.</span><span class="sxs-lookup"><span data-stu-id="d5a40-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="d5a40-123">![Koşullu erişim için temel ilkeleri listeleyen sayfa.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="d5a40-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="d5a40-124">Her ilke için aşağıdaki özel yönergeye bakın:</span><span class="sxs-lookup"><span data-stu-id="d5a40-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="d5a40-125">Yöneticiler için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="d5a40-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="d5a40-126">Kullanıcılar için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="d5a40-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="d5a40-127">Eski kimlik doğrulamasını engelleme</span><span class="sxs-lookup"><span data-stu-id="d5a40-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="d5a40-128">Hizmet yönetimi için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="d5a40-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="d5a40-129">Onaylı istemci uygulamaları gerektirmek gibi birçok ek ilke ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d5a40-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="d5a40-130">Daha fazla bilgi için [Koşullu Erişim Belgelerine](https://docs.microsoft.com/azure/active-directory/conditional-access/) bakın.</span><span class="sxs-lookup"><span data-stu-id="d5a40-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>