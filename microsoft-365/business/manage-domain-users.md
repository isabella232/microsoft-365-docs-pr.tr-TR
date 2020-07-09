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
# <a name="synchronize-domain-users-to-microsoft-365"></a>Etki alanı kullanıcılarını Microsoft 365 ile senkronize etme

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin Senkronizasyonuna Hazırla 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden önce, [Microsoft 365'e dizin eşitlemesi için hazırlayın'ı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin. Özellikle:

   - Aşağıdaki öznitelikler için dizininizde yineleme olmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**. Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz. Örneğin: *mary@contoso.yerel* yerine *mary.shelley@contoso.com*
   
   - Active Directory etki alanı *.com* veya *.org*gibi bir internet routable sonek yerine *.local* veya *.lan*gibi bir routable olmayan sonek biterse, önce yerel kullanıcı hesaplarının UPN sonekini [dizin eşitleme için routable olmayan bir etki alanı hazırlayın'da](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)açıklandığı gibi ayarlayın. 

Aşağıdaki adım dört (4) adımdaki **Run IdFix,** şirket içi Active Directory'nizin dir senkronizasyonuna hazır olduğundan da emin olacaktır.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connect'i yükleme ve yapılandırma

Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'i yükleyin ve dizin eşitlemesi ayarlayın. 

 1. <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>Sol daki **Kurulum'u** seçin'deki yönetici merkezinde.

 2. **Oturum Açma ve güvenlik**altında, org **dizininizdeki Eşitleme kullanıcıları**altında **Görüntüle'yi** seçin.

 3. **Org'unuzun dizin sayfasındaki Eşitleme kullanıcıları** üzerinde **Başlat'ı**seçin.

 4. İlk adımda Dizin eşitleme için hazırlamak için IdFix aracı çalıştırın.

 5. Azure AD Connect'i indirmek ve etki alanı denetimindeki kullanıcılarınızı Microsoft 365 ile senkronize etmek için kullanmak için sihirbaz adımlarını izleyin.


Bkz. Daha fazla bilgi edinmek [için Microsoft 365 için dizin eşitlemesi ayarla.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

Azure AD Connect seçeneklerinizi yapılandırırken, İş için Microsoft 365'te de desteklenen **Parola Eşitleme**, **Kesintisiz Tek Oturum**Açma ve parola **yazma** özelliğini etkinleştirmenizi öneririz.

> [!NOTE]
> Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır. Daha fazla bilgi için [bkz: Nasıl Yapılır: parola yazmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

Etki alanına bağlı Windows 10 aygıtlarını da yönetmek istiyorsanız, [bkz.](manage-windows-devices.md) 