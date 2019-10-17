---
title: Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Microsoft 365'in yerel AD'yi korumak için Windows 10 aygıtlarını nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 392c57a7350a901c1481be632e880cc9fcaa6140
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575988"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme

Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.
Bunu ayarlamak için Karma **Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz. Bunlar, hem şirket içi Active Dizininize hem de Azure Etkin Dizininize katılan aygıtlardır.

Aşağıdaki video, aşağıdaki adımlarda da ayrıntılı olarak ayrıntılı olarak açıklanan en yaygın senaryo için bu ayarlama adımları ayrıntıları.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Dizin Senkronizasyonuna Hazırla 

Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden önce, [Office 365'e dizin eşitlemesi için hazırlayın'ı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin. Özellikle:

   - Aşağıdaki öznitelikler için dizininizde yineleme bulunmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**. Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğinin lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırılmasını öneririz. Örneğin *mary@contoso.local* yerine *mary.shelley@contoso.com*
   
   - Active Directory etki alanı *.com* veya *.org*gibi bir internet routable sonek yerine *.local* veya *.lan*gibi bir routable olmayan sonek biterse, ilk olarak açıklandığı gibi yerel kullanıcı hesaplarının UPN soneki ayarlamanız gerekir [Dizin eşitleme için routable olmayan bir etki alanı hazırlayın.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Azure AD Connect'i yükleme ve yapılandırma

Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'i yükleyin ve dizin eşitlemesi ayarlayın. Bkz. Daha fazla bilgi edinmek [için Office 365 için dizin eşitlemesi ayarla.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> Adımlar Microsoft 365 Business için tam olarak aynıdır. 

Azure AD Connect seçeneklerinizi yapılandırırken, **Parola Senkronizasyonu** ve **Sorunsuz Tek Oturum**Açma özelliğinin yanı sıra Microsoft 365 Business'ta da desteklenen parola **yazma** özelliğini etkinleştirmenizi öneririz.

> [!NOTE]
> Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır. Daha fazla bilgi için [bkz: Nasıl Yapılır: parola yazmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Karma Azure REKLAM Birleştirme'yi Yapılandırma

Windows 10 aygıtlarını Karma Azure AD olarak etkinleştirmeden önce aşağıdaki ön koşulları yerine getirebildiğinizden emin olmalısınız:

   - Azure AD bağlantısının en son sürümünü çalıştırıyorsunuz.

   - Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti. Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.

Karma Azure AD'nin katıldığı varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydetmek [için, Öğreticideki adımları izleyin: Yönetilen etki alanları için karma Azure Active Directory join'i yapılandırın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Bu, varolan şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını sağlar ve bulutları hazır hale getirecektir.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Windows 10 için otomatik kaydı etkinleştirme

 Mobil aygıt yönetimi için Windows 10 aygıtlarını Intune'a otomatik olarak kaydetmek için Grup [İlkesi'ni kullanarak bir Windows 10 aygıtını otomatik olarak kaydedin'e](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)bakın. Grup İlkesi'ni yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için Grup İlkesi Yönetim Konsolu ve ADMX şablonlarını kullanarak Etki Alanı Denetleyicinizde bu grup ilkesi ayarını oluşturabilirsiniz.

## <a name="5-configure-seamless-single-sign-on"></a>5. Yapılandırılan Sorunsuz Tek İşaret-On

  Sorunsuz SSO, kullanıcıları kurumsal bilgisayarları kullandıklarında Microsoft 365 bulut kaynaklarında otomatik olarak oturum alacaktır. [Azure Active Directory Seamless Tek Oturum Açma: Hızlı başlangıç'ta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)açıklanan iki Grup İlkesi seçeneğinden birini dağıtmanız yeterlidir. **Grup İlkesi** seçeneği kullanıcıların ayarlarını değiştirmesine izin vermezken, **Grup İlkesi Tercihi** seçeneği değerleri ayarlar, aynı zamanda kullanıcı tarafından yapılandırılabilir bırakır.

## <a name="6-set-up-windows-hello-for-business"></a>6. İşletmeler için Windows Hello'yu ayarlama

 Windows Hello for Business, yerel bir bilgisayarda oturum açmak için parolaları güçlü iki faktörlü kimlik doğrulama (2FA) ile değiştirir. Bir faktör asimetrik anahtar çifti, diğeri ise aygıtınız destekliyorsa parmak izi veya yüz tanıma gibi bir PIN veya diğer yerel harekettir. Parolaları mümkün olduğunca 2FA ve Windows Hello for Business ile değiştirmenizi öneririz.

İşletmeler için Karma Windows Merhaba'yı yapılandırmak [için, İş Önkoşulları için Karma Anahtar güven Windows Hello'yu gözden geçirin.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs) Ardından, İş [için Karma Windows Merhaba'yı Yapılandır'daki](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)yönergeleri izleyin anahtar güven ayarları. 
