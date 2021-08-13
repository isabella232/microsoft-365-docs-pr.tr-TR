---
title: Etki alanı kullanıcılarını eşitlemek Microsoft 365
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
description: Etki alanı denetimli kullanıcıları iş için Microsoft 365 eşitleme.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809322"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Etki alanı kullanıcılarını eşitlemek Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin Eşitlemesi'ne Hazırlanma 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki [](../enterprise/prepare-for-directory-synchronization.md)Alanı'Microsoft 365. Özellikle:

   - Dizinde şu öznitelikler için yinelenen değerler **(mail,** **proxyAddresses** ve **userPrincipalName)** olduğundan emin olun. Bu değerlerin benzersiz olması ve tüm yinelenenlerin kaldırılması gerekir.
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini, lisanslı kullanıcıya karşılık gelen birincil e-posta adresiyle eşecek şekilde Microsoft 365 öneririz. Örneğin:  *mary.shelley@contoso.com.local yerine mary@contoso.*
   
   - Active Directory etki alanı *.com* veya *.org* gibi İnternet'e yönlendirilebilir bir sonek yerine *.local* veya *.lan* gibi yönlendirilebilir olmayan bir sonek ile bitiyorsa, öncelikle Dizin eşitlemesi için yönlendirilebilir olmayan bir etki alanını hazırlama konusunda açıklandığı gibi yerel kullanıcı hesaplarının UPN soneki [ayarlayın.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Aşağıdaki dört. adımda (4) **IdFix'i** çalıştır, şirket içi Active Directory'nizin dizin eşitlemeye hazır olduğundan da emin olur.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD E-postalarını yükleme ve Bağlan

Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den başka bir Azure Active Directory eşitlemek için Azure Active Directory Bağlan eşitlemesini yükleyin ve ayarlayın. 

 1. Yönetim [merkezinde, sol](https://go.microsoft.com/fwlink/p/?linkid=2024339) **gezintiden** Kurulum'u seçin.

 2. Oturum **açma ve güvenlik altında,** Kullanıcıların kuruluş **dizininden** **eşitle'nin altında Görüntüle'yi seçin.**

 3. Kuruluş **dizinden kullanıcıları eşitle sayfasında,** **Başla'ya tıklayın.**

 4. İlk adımda, IdFix aracını çalıştırarak Dizin eşitlemeye hazırlanmak için.

 5. Azure AD E-posta aboneliğini indirmek Bağlan sihirbaz adımlarını izleyin ve bu adımları kullanarak etki alanı denetimli kullanıcılarınızı eşitlemek Microsoft 365.


Daha [fazla bilgi edinmek için bkz. Microsoft 365](../enterprise/set-up-directory-synchronization.md) eşitlemeyi ayarlama.

Azure AD Bağlan için seçeneklerinizi yapılandırken, Parola Eşitlemesi **,** Sorunsuz Çoklu Oturum Açma  ve aynı zamanda işletmeler için Microsoft 365'de de desteklenen parola geri yazma özelliğini etkinleştirmenizi öneririz. 

> [!NOTE]
> Azure AD'de parola geri yazma adımları, Azure AD'de onay kutusunun Bağlan. Daha fazla bilgi için [bkz. Nasıl yapılandırılır: parola geri yazma.](/azure/active-directory/authentication/howto-sspr-writeback) 

Etki alanına katılmış cihazları da Windows 10, karma bir Azure AD Join ayarlamak için bkz. Etki alanına katılmış [Windows 10](manage-windows-devices.md) cihazlarının Microsoft 365 İş Ekstra tarafından yönetillerini etkinleştirme.