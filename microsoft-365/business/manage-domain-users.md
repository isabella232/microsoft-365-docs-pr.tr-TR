---
title: Etki alanı kullanıcılarını Microsoft 365'e eşitleme
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
description: Etki alanı denetimli kullanıcıları Microsoft 365 İş ile eşitler.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913264"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Etki alanı kullanıcılarını Microsoft 365'e eşitleme

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin Eşitlemesi için Hazırlanma 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanı'nden eşitlemeden [önce, Microsoft 365'e dizin eşitlemesi için hazırlanma'ya bakabilirsiniz.](../enterprise/prepare-for-directory-synchronization.md) Özellikle:

   - Dizinde şu öznitelikler için hiçbir yinelemenin mevcut olmadığını emin olun: **posta,** **proxyAddresses** ve **userPrincipalName**. Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini lisanslı Microsoft 365 kullanıcıya karşılık gelen birincil e-posta adresiyle eş olacak şekilde yapılandırmanızı öneririz. Örneğin:  *mary.shelley@contoso.com.local yerine mary@contoso.*
   
   - Active Directory etki alanı *.com* veya *.org* gibi İnternet'e yönlendirilebilir bir sonek yerine *.local* veya *.lan* gibi yönlendirilebilir olmayan bir sonekle bitiyorsa, önce dizin eşitlemesi için yönlendirilebilir olmayan bir etki alanını hazırlama konusunda açıklandığı gibi yerel kullanıcı hesaplarının UPN soneki [ayarlayın.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

Aşağıdaki dördüncü adımda (4) **IdFix** Çalıştır, şirket içi Active Directory'nizin dizin eşitlemesi için hazır olduğundan da emin olur.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connect'i yükleme ve yapılandırma

Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'ye eşitlemek için, Azure Active Directory Connect'i yükleyin ve dizin eşitlemesini ayarlayın. 

 1. Yönetim [merkezinde, sol](https://go.microsoft.com/fwlink/p/?linkid=2024339) **gezintide** Kurulum'u seçin.

 2. Oturum **açma ve güvenlik altında, oturum** açma **kullanıcılarınızı** **eşitle'nin altında Görüntüle'yi seçin.**

 3. Kuruluş dizin **sayfasından Kullanıcıları eşitle'yi** **seçin.**

 4. Dizin eşitlemeye hazırlanmak için ilk adımda IdFix aracını çalıştırın.

 5. Azure AD Connect'i indirmek ve etki alanı denetimli kullanıcılarınızı Microsoft 365'e eşitlemek için sihirbaz adımlarını izleyin.


Daha [fazla bilgi edinmek için Bkz. Microsoft 365 için dizin](../enterprise/set-up-directory-synchronization.md) eşitlemesini ayarlama.

Azure AD Connect'e yönelik seçeneklerinizi yapılandırken, Microsoft 365 İş'te de desteklenen Parola Eşitlemesi, Sorunsuz Çoklu Oturum Açma ve parola geri yazma özelliğini etkinleştirmenizi öneririz. 

> [!NOTE]
> Azure AD Connect'te parola geri yazma için bazı ek adımlar vardır. Daha fazla bilgi için bkz. [Nasıl yapılandırılır: parola geri yazma.](/azure/active-directory/authentication/howto-sspr-writeback) 

Etki alanına katılmış Windows 10 cihazlarını da yönetmek için bkz. Etki alanına katılmış [Windows 10 cihazlarını Microsoft 365 Business Premium](manage-windows-devices.md) tarafından yönetecek şekilde etkinleştirme ve karma Azure AD Join ayarlama.