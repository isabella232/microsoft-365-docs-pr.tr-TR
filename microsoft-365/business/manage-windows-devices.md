---
title: Etki alanına birleştirilmiş Windows 10 aygıtlarını iş için Microsoft 365 tarafından yönetilmesini etkinleştirin
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Microsoft 365'in yerel Active-Directory'ye katılan Windows 10 aygıtlarını yalnızca birkaç adımda nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471057"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Etki alanına bağlı Windows 10 cihazlarının Microsoft 365 Business Premium tarafından yönetilmesini etkinleştirme

Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.
Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz. Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.

Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacağına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin Senkronizasyonuna Hazırla 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden önce, [Office 365'e dizin eşitlemesi için hazırlayın'ı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin. Özellikle:

   - Aşağıdaki öznitelikler için dizininizde yineleme olmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**. Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz. Örneğin: *mary@contoso.yerel* yerine *mary.shelley@contoso.com*
   
   - Active Directory etki alanı *.com* veya *.org*gibi bir internet routable sonek yerine *.local* veya *.lan*gibi bir routable olmayan sonek biterse, önce yerel kullanıcı hesaplarının UPN sonekini [dizin eşitleme için routable olmayan bir etki alanı hazırlayın'da](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)açıklandığı gibi ayarlayın. 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connect'i yükleme ve yapılandırma

Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'i yükleyin ve dizin eşitlemesi ayarlayın. Bkz. Daha fazla bilgi edinmek [için Office 365 için dizin eşitlemesi ayarla.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

> [!NOTE]
> Adımlar, iş için Microsoft 365 için tam olarak aynıdır. 

Azure AD Connect seçeneklerinizi yapılandırırken, İş için Microsoft 365'te de desteklenen **Parola Eşitleme**, **Kesintisiz Tek Oturum**Açma ve parola **yazma** özelliğini etkinleştirmenizi öneririz.

> [!NOTE]
> Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır. Daha fazla bilgi için [bkz: Nasıl Yapılır: parola yazmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Karma Azure REKLAM Birleştirme'yi Yapılandırma

Windows 10 aygıtların Karma Azure AD'ye katılmasını etkinleştirmeden önce aşağıdaki ön koşulları yerine getirebildiğinizden emin olun:

   - Azure AD Connect'in en son sürümünü çalıştırıyorsunuz.

   - Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti. Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.

Karma Azure AD'nin katıldığı varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydetmek [için, Öğreticideki adımları izleyin: Yönetilen etki alanları için karma Azure Active Directory join'i yapılandırın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Bu karma, mevcut şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını ve bulutu hazır hale getirmesini sağlar.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Windows 10 için otomatik kaydı etkinleştirme

 Mobil aygıt yönetimi için Windows 10 aygıtlarını Intune'a otomatik olarak kaydetmek için Grup [İlkesi'ni kullanarak bir Windows 10 aygıtını otomatik olarak kaydedin'e](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)bakın. Grup İlkesi'ni yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için Etki Alanı Denetleyicinizde bu Grup İlkesi ayarını oluşturmak için Grup İlkesi Yönetim Konsolu ve ADMX şablonlarını kullanabilirsiniz.

## <a name="5-configure-seamless-single-sign-on"></a>5. Yapılandırılan Sorunsuz Tek İşaret-On

  Sorunsuz SSO, kullanıcıları kurumsal bilgisayarları kullanırken Microsoft 365 bulut kaynaklarına otomatik olarak imzalar. [Azure Active Directory Seamless Tek Oturum Açma: Hızlı başlangıç'ta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)açıklanan iki Grup İlkesi seçeneğinden birini dağıtmanız yeterlidir. **Grup İlkesi** seçeneği kullanıcıların ayarlarını değiştirmesine izin vermezken, **Grup İlkesi Tercihi** seçeneği değerleri ayarlar, aynı zamanda kullanıcı tarafından yapılandırılabilir bırakır.

## <a name="6-set-up-windows-hello-for-business"></a>6. İşletmeler için Windows Hello'yu ayarlama

 Windows Hello for Business, yerel bir bilgisayarda oturum açmak için parolaları güçlü iki faktörlü kimlik doğrulama (2FA) ile değiştirir. Bir faktör asimetrik anahtar çifti, diğeri ise aygıtınız destekliyorsa parmak izi veya yüz tanıma gibi bir PIN veya diğer yerel harekettir. Parolaları mümkün olduğunca 2FA ve Windows Hello for Business ile değiştirmenizi öneririz.

İşletmeler için Karma Windows Merhaba'yı yapılandırmak [için, İş Önkoşulları için Karma Anahtar güven Windows Hello'yu gözden geçirin.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs) Ardından, İş [için Karma Windows Merhaba'yı Yapılandır'daki](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)yönergeleri izleyin anahtar güven ayarları. 
