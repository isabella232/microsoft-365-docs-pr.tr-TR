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
search.appverid:
- BCS160
- MET150
- MOE150
description: Önemli ölçüde ek güvenlik eklemek için Microsoft 365 Kampanyaları için koşullu erişim ilkeleri nasıl ayarlayabilirsiniz öğrenin.
ms.openlocfilehash: 26fadecc69486d7931dac069d8f53061592f397f
ms.sourcegitcommit: e525bcf073a61e1350484719a0c3ceb6ff0d8db1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2020
ms.locfileid: "43153776"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="79796-103">Koşullu Erişim ilkelerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="79796-103">Set up Conditional Access policies</span></span>

<span data-ttu-id="79796-104">[Koşullu Erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri önemli ölçüde ek güvenlik ekler.</span><span class="sxs-lookup"><span data-stu-id="79796-104">[Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="79796-105">Microsoft, tüm müşteriler için önerilen bir temel Koşullu Erişim ilkeleri kümesi sağlar.</span><span class="sxs-lookup"><span data-stu-id="79796-105">Microsoft provides a set of baseline Conditional Access policies that are recommended for all customers.</span></span> <span data-ttu-id="79796-106">Temel ilkeler, kuruluşların birçok yaygın saldırıya karşı korunmasına yardımcı olan önceden tanımlanmış ilkeler kümesidir.</span><span class="sxs-lookup"><span data-stu-id="79796-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="79796-107">Bu yaygın saldırılar parola püskürtme, yeniden oynatma ve kimlik avı içerebilir.</span><span class="sxs-lookup"><span data-stu-id="79796-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="79796-108">Bu ilkeler, belirli koşullar yerine getirildiğinde yöneticilerin ve kullanıcıların ikinci bir kimlik doğrulama biçimi (çok faktörlü kimlik doğrulama veya MFA olarak adlandırılır) girmesini gerektirir.</span><span class="sxs-lookup"><span data-stu-id="79796-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="79796-109">Örneğin, bir kullanıcı farklı bir ülkeden oturum veriyorsa, oturum açma riskli kabul edilebilir ve kullanıcının ek bir kimlik doğrulama biçimi sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="79796-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="79796-110">Şu anda, temel ilkeler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="79796-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="79796-111">**Yöneticiler için MFA'yı zorunlu kılması,** &ndash; genel yönetici de dahil olmak üzere en ayrıcalıklı yönetici rolleri için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="79796-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="79796-112">**Son kullanıcı koruması** &ndash; Yalnızca oturum açma riskli olduğunda kullanıcılar için çok faktörlü kimlik doğrulaması gerektirir.</span><span class="sxs-lookup"><span data-stu-id="79796-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="79796-113">**Eski kimlik doğrulamayı** &ndash; engelleyin Eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli, kimlik doğrulama protokolleri kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="79796-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="79796-114">Bu eski uygulamalar Koşullu Erişim ilkelerini atlayabilir ve ortamınıza yetkisiz erişim sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="79796-114">These older apps can bypass Conditional Access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="79796-115">Bu ilke, Koşullu Erişimi desteklemeyen istemcilerin erişimini engeller.</span><span class="sxs-lookup"><span data-stu-id="79796-115">This policy blocks access from clients that don't support Conditional Access.</span></span> 
- <span data-ttu-id="79796-116">**Hizmet Yönetimi** &ndash; için MFA'yı zorunlu kılması Azure portalı (temel ilkeleri yapılandırdığınız yer) dahil olmak üzere yönetim araçlarına erişmek için çok faktörlü kimlik doğrulama gerektirir.</span><span class="sxs-lookup"><span data-stu-id="79796-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="79796-117">Microsoft, bu temel ilkelerin tümünün etkinleştirilmesini önerir.</span><span class="sxs-lookup"><span data-stu-id="79796-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="79796-118">Bu ilkeler etkinleştirildikten sonra, yöneticilerden ve kullanıcılardan Azure Multii-Factor kimlik doğrulaması için kaydolması istenir.</span><span class="sxs-lookup"><span data-stu-id="79796-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="79796-119">Bu ilkeler hakkında daha fazla bilgi için [temel ilkeler nelerdir?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="79796-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="79796-120">Temel ilkeleri ayarlama</span><span class="sxs-lookup"><span data-stu-id="79796-120">Set up baseline policies</span></span>

1. <span data-ttu-id="79796-121">Azure [portalına](https://portal.azure.com)gidin ve ardından **Azure Etkin Dizin** \> **Koşullu Erişim'e**gidin.</span><span class="sxs-lookup"><span data-stu-id="79796-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="79796-122">Temel ilkeler sayfada listelenir.</span><span class="sxs-lookup"><span data-stu-id="79796-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="79796-123">![Koşullu Erişim için temel ilkeleri listeleyen sayfa.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="79796-123">![Page that lists baseline policies for Conditional Access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="79796-124">Her ilke için aşağıdaki özel yönergeye bakın:</span><span class="sxs-lookup"><span data-stu-id="79796-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="79796-125">Yöneticiler için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="79796-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="79796-126">Kullanıcılar için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="79796-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="79796-127">Eski kimlik doğrulamasını engelleme</span><span class="sxs-lookup"><span data-stu-id="79796-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="79796-128">Hizmet yönetimi için MFA gerektirir</span><span class="sxs-lookup"><span data-stu-id="79796-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="79796-129">Onaylı istemci uygulamaları gerektirmek gibi birçok ek ilke ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="79796-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="79796-130">Daha fazla bilgi için [Koşullu Erişim Belgeleri'ne](https://docs.microsoft.com/azure/active-directory/conditional-access/)bakın.</span><span class="sxs-lookup"><span data-stu-id="79796-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
