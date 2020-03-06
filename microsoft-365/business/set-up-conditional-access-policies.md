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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
description: Önemli ölçüde ek güvenlik eklemek için Microsoft 365 Kampanyaları için koşullu erişim ilkeleri nasıl ayarlayabilirsiniz öğrenin.
ms.openlocfilehash: be3ca0da3d27e3ec49f1227e4482cfd7fcaae8cb
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550087"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="fabd5-103">Koşullu erişim ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="fabd5-103">Set up conditional access policies</span></span>

<span data-ttu-id="fabd5-104">[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri önemli ölçüde ek güvenlik ekler.</span><span class="sxs-lookup"><span data-stu-id="fabd5-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="fabd5-105">Microsoft, tüm müşteriler için önerilen bir temel koşullu erişim ilkeleri kümesi sağlar.</span><span class="sxs-lookup"><span data-stu-id="fabd5-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="fabd5-106">Temel ilkeler, kuruluşların birçok yaygın saldırıya karşı korunmasına yardımcı olan önceden tanımlanmış ilkeler kümesidir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="fabd5-107">Bu yaygın saldırılar parola püskürtme, yeniden oynatma ve kimlik avı içerebilir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="fabd5-108">Bu ilkeler, belirli koşullar yerine getirildiğinde yöneticilerin ve kullanıcıların ikinci bir kimlik doğrulama biçimi (çok faktörlü kimlik doğrulama veya MFA olarak adlandırılır) girmesini gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="fabd5-109">Örneğin, bir kullanıcı farklı bir ülkeden oturum veriyorsa, oturum açma riskli kabul edilebilir ve kullanıcının ek bir kimlik doğrulama biçimi sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="fabd5-110">Şu anda, temel ilkeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="fabd5-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="fabd5-111">**Yöneticiler için MFA'yı zorunlu kılması,** &ndash; genel yönetici de dahil olmak üzere en ayrıcalıklı yönetici rolleri için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="fabd5-112">**Son kullanıcı koruması** &ndash; Yalnızca oturum açma riskli olduğunda kullanıcılar için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="fabd5-113">**Eski kimlik doğrulamayı** &ndash; engelleyin Eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli, kimlik doğrulama protokolleri kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="fabd5-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="fabd5-114">Bu eski uygulamalar koşullu erişim ilkelerini atlayabilir ve ortamınıza yetkisiz erişim elde edebilir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="fabd5-115">Bu ilke, koşullu erişimi desteklemeyen istemcilerin erişimini engeller.</span><span class="sxs-lookup"><span data-stu-id="fabd5-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="fabd5-116">**Hizmet Yönetimi** &ndash; için MFA'yı zorunlu kılması Azure portalı (temel ilkeleri yapılandırdığınız yer) dahil olmak üzere yönetim araçlarına erişmek için çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="fabd5-117">Microsoft, bu temel ilkelerin tümünün etkinleştirilmesini önerir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="fabd5-118">Bu ilkeler etkinleştirildikten sonra, yöneticilerden ve kullanıcılardan Azure Multii-Factor kimlik doğrulaması için kaydolması istenir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="fabd5-119">Bu ilkeler hakkında daha fazla bilgi için [temel ilkeler nelerdir?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="fabd5-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="fabd5-120">Temel ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="fabd5-120">Set up baseline policies</span></span>

1. <span data-ttu-id="fabd5-121">Azure [portalına](https://portal.azure.com)gidin ve ardından **Azure Etkin Dizin** \> **Koşullu Erişim'e**gidin.</span><span class="sxs-lookup"><span data-stu-id="fabd5-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="fabd5-122">Temel ilkeler sayfada listelenir.</span><span class="sxs-lookup"><span data-stu-id="fabd5-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="fabd5-123">![Koşullu erişim için temel ilkeleri listeleyen sayfa.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="fabd5-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="fabd5-124">Her ilke için aşağıdaki özel yönergeye bakın:</span><span class="sxs-lookup"><span data-stu-id="fabd5-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="fabd5-125">Yöneticiler için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="fabd5-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="fabd5-126">Kullanıcılar için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="fabd5-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="fabd5-127">Eski kimlik doğrulamasını engelleme</span><span class="sxs-lookup"><span data-stu-id="fabd5-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="fabd5-128">Hizmet yönetimi için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="fabd5-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="fabd5-129">Onaylı istemci uygulamaları gerektirmek gibi birçok ek ilke ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fabd5-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="fabd5-130">Daha fazla bilgi için [Koşullu Erişim Belgeleri'ne](https://docs.microsoft.com/azure/active-directory/conditional-access/)bakın.</span><span class="sxs-lookup"><span data-stu-id="fabd5-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
