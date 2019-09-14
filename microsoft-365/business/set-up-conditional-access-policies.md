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
# <a name="set-up-conditional-access-policies"></a>Koşullu erişim ilkeleri ayarlama

[Koşullu erişim](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ilkeleri, yedek ek güvenlik ekler. Microsoft, tüm müşteriler için önerilen bir temel koşullu erişim ilkeleri kümesi sağlar. Temel ilkeler, kuruluşların birçok yaygın saldırıya karşı korunmasına yardımcı olan önceden tanımlanmış ilkeler kümesidir. Bu yaygın saldırılar parola püskürtme, yeniden oynatma ve kimlik avı içerebilir.

Bu ilkeler, belirli koşullar yerine getirildiğinde yöneticilerin ve kullanıcıların ikinci bir kimlik doğrulama biçimi (çok faktörlü kimlik doğrulama veya MFA olarak adlandırılır) girmesini gerektirir. Örneğin, bir kullanıcı farklı bir ülkeden oturum veriyorsa, oturum açma riskli kabul edilebilir ve kullanıcının ek bir kimlik doğrulama biçimi sağlaması gerekir. 

Şu anda, temel ilkeler şunlardır:
- **Yöneticiler için MFA gerektirir** — Genel yönetici de dahil olmak üzere en ayrıcalıklı yönetici rolleri için çok faktörlü kimlik doğrulaması gerektirir.
- **Son kullanıcı koruması** — Yalnızca oturum açma riskli olduğunda kullanıcılar için çok faktörlü kimlik doğrulaması gerektirir. 
- **Eski kimlik doğrulamayı engelleyin** — Eski istemci uygulamaları ve bazı yeni uygulamalar daha yeni, daha güvenli, kimlik doğrulama protokolleri kullanmaz. Bu eski uygulamalar koşullu erişim ilkelerini atlayabilir ve ortamınıza yetkisiz erişim elde edebilir. Bu ilke, koşullu erişimi desteklemeyen istemcilerin erişimini engeller. 
- **Hizmet Yönetimi için MFA Gerektirir** — Azure portalı (temel ilkeleri yapılandırdığınız yer) dahil olmak üzere yönetim araçlarına erişmek için çok faktörlü kimlik doğrulama gerektirir. 

Microsoft, bu temel ilkelerin tümünün etkinleştirilmesini önerir. Bu ilkeler etkinleştirildikten sonra, yöneticilerden ve kullanıcılardan Azure Multii-Factor kimlik doğrulaması için kaydolması istenir.

Bu ilkeler hakkında daha fazla bilgi için [temel ilkeler nelerdir?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Temel ilkeleri ayarlama

1. Azure [portalına](https://portal.azure.com)gidin ve ardından **Azure Etkin Dizin** \> **Koşullu Erişim'e**gidin.
    
    Temel ilkeler sayfada listelenir. <br/> <br/>
    ![Koşullu erişim için temel ilkeleri listeleyen sayfa.](media/baslinepolicies.png)
1. Her ilke için aşağıdaki özel yönergeye bakın:

  - [Yöneticiler için MFA gerektirir](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Kullanıcılar için MFA gerektirir](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Eski kimlik doğrulamasını engelleme](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Hizmet yönetimi için MFA gerektirir](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Onaylı istemci uygulamaları gerektirmek gibi birçok ek ilke ayarlayabilirsiniz. Daha fazla bilgi için [Koşullu Erişim Belgelerine](https://docs.microsoft.com/azure/active-directory/conditional-access/) bakın.