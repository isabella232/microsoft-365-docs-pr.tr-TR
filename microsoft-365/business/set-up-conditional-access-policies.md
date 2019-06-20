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
# <a name="set-up-conditional-access-policies"></a>Koşullu erişim ilkelerini kurun

[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri substancial ek güvenlik ekleyin. Microsoft, tüm müşteriler için önerilen temel koşullu erişim ilkeleri kümesi sağlar. Temel ilkeleri kuruluşlar birçok ortak saldırılara karşı korunmasına yardımcı olmak önceden tanımlanan ilkeler bir kümesidir. Bu ortak saldırıları parola sprey, replay ve kimlik avı dahil edebilirsiniz.

Bu ilkeler Yöneticiler ve kullanıcıların ikinci bir form kimlik doğrulaması (çok faktörlü kimlik doğrulama veya MFA denir) girmesini gerektiren zaman koşullar. Örneğin, bir kullanıcı farklı bir ülkeden oturum açma, oturum riskli olarak kabul edilebilir ve kullanıcı başka bir kimlik doğrulama biçimi sağlamanız gerekir. 

Şu anda, temel ilkeleri şunlardır:
- **Yöneticileri için MFA gerektirir** — genel yönetici de dahil olmak üzere en yüksek ayrıcalıklı yönetici rolleri çok faktörlü kimlik doğrulama gerektirir.
- **Son kullanıcı koruması** — bir işareti de risklidir yalnızca kullanıcılar için çok faktörlü kimlik doğrulama gerektirir. 
- **Eski kimlik bloğunu** — eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli kimlik doğrulama protokollerini kullanma. Bu eski uygulamaların, koşullu erişim ilkelerini devre dışı bırakabilir ve ortamınızı yetkisiz erişim. Bu ilke erişimi engeller koşullu erişim desteklemeyen istemcilerden gelen. 
- **Servis Yönetimi için gerekli MFA** — erişim için yönetim araçlarını (Burada yapılandırdığınız temel ilkeleri) Azure portal dahil olmak üzere, çok faktörlü kimlik doğrulama gerektirir. 

Microsoft, bu temel ilkelerini etkinleştir önerir. Bu ilkeler etkinleştirildikten sonra Yöneticiler ve kullanıcılar Azure Multii faktörlü kimlik doğrulama için kaydetmek için istenir.

Bu ilkeler hakkında daha fazla bilgi için bkz: [temel ilkeleri nelerdir](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Temel ilkelerini kurun

1. [Azure portalı](https://portal.azure.com)' na gidin ve sonra **Active Directory Azure** gidin \> **Koşullu erişim**.
    
    Temel ilkeleri sayfasında listelenir. <br/> <br/>
    ![Koşullu erişim için temel ilkelerini listeler sayfası.](media/baslinepolicies.png)
1. Her ilke için aşağıdaki özel yönergelere bakın:

  - [MFA Yöneticiler için gerektirir.](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire MFA kullanıcılar için](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blok eski kimlik doğrulaması](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [MFA Hizmeti Yönetimi için gerekli](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Onaylanmış istemci uygulamaları gerektiren gibi birçok ek ilkeler ayarlayabilirsiniz. Daha fazla bilgi için [Koşullu erişim belgelerine](https://docs.microsoft.com/azure/active-directory/conditional-access/) bakın.