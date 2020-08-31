---
title: Etki alanı kullanıcılarını Microsoft 365 ile eşitleme
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
description: Etki alanı denetimli kullanıcıları Microsoft 365 iş ile eşitleyin.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306459"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Etki alanı kullanıcılarını Microsoft 365 ile eşitleme

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin eşitlemeye hazırlanma 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory etki alanından eşitlemeden önce, [Microsoft 365 ile dizin eşitlemesi hazırlığı](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization)konusuna bakın. Özellikle:

   - Aşağıdaki öznitelikler için dizininizde hiçbir çoğaltma bulunmadığından emin olun: **posta**, **proxyAddresses**ve **userPrincipalName**. Bu değerlerin benzersiz olması ve tüm çoğaltmaların kaldırılması gerekir.
   
   - Her yerel kullanıcı hesabının **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz. Örneğin: *Mary@contoso. yerel* yerine *Mary.Shelley@contoso.com*
   
   - Active Directory etki *alanı,.* com veya. org gibi internet yönlendirilebilir soneki yerine *,.* *com* veya *. org*gibi yönlendirilemeyen bir sonek içinde sona erdiğinde, [Dizin eşitlemesi için yönlendirilemeyen bir etki ALANıNı hazırlama](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)başlığı altında açıklandığı gibi yerel kullanıcı hesaplarının UPN sonekini ayarlayın. 

Aşağıdaki dört (4) adımdaki **Run Idfıx** , şirket Içi Active Directory 'nin dır eşitlemesi için hazır olduğundan emin olur.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connect 'i yükleme ve yapılandırma

Kullanıcıları, grupları ve kişilerinizi yerel Active Directory 'den Azure Active Directory 'ye eşitlemek için Azure Active Directory Connect 'i yükleyin ve dizin eşitlemesini ayarlayın. 

 1. Yönetim merkezinde, sol gezintide <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Kurulum 'u** seçin.

 2. **Oturum açma ve güvenlik**altında, **kuruluşunuzun dizininden kullanıcıları Eşitle**altında **Görünüm** 'ü seçin.

 3. Kullanıcıları kuruluşunuzun **dizininden Eşitle** sayfasında **başlayın**'ı seçin.

 4. Dizin eşitlemeye hazırlanmak için ilk adım çalışma IdFix aracında.

 5. Sihirbazın adımlarını kullanarak Azure AD Connect 'i indirin ve etki alanı denetimli kullanıcılarınızı Microsoft 365 ile eşitlemek için kullanın.


Daha fazla bilgi edinmek için [Microsoft 365 için dizin eşitlemesini ayarlayın](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) .

Azure AD Connect için seçeneklerinizi yapılandırırken, **parola eşitleme**, **kesintisiz çoklu oturum açma**ve **parola geri yazma** özelliğini etkinleştirmenizi öneririz, bu da Microsoft 365 iş için desteklenmektedir.

> [!NOTE]
> Azure AD Connect 'teki denetim kutusunun ötesinde parola geri yazma için bazı ek adımlar vardır. Daha fazla bilgi [için bkz.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

Etki alanına bağlı Windows 10 cihazlarını da yönetmek istiyorsanız, karma Azure AD birleştirmeyi ayarlamak için [etki alanına bağlı Windows 10 cihazlarını Microsoft 365 Business Premium tarafından yönetilecek şekilde etkinleştirme](manage-windows-devices.md) konusuna bakın. 