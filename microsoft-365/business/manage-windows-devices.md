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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Microsoft 365'in yerel AD'yi korumak için Windows 10 aygıtlarını nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068115"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme

Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz. Bunu, önce Active Directory ile senkronize ederek, ardından Windows 10 aygıtlarını Azure AD'ye kaydederek ve Microsoft 365 Business tarafından mobil cihaz yönetimine kaydederek ayarlayabilirsiniz.
Aşağıdaki video, bunu en yaygın senaryo için nasıl ayarlayabilmek için gereken adımları ayrıntılarıyla açıklar.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Microsoft 365 Business tarafından yönetilecek etki alanı birleştirilmiş aygıtları ayarlama

Kurum içi Active Directory'ye ek olarak Azure Active Directory tarafından sağlanan özelliklerden yararlanacak şekilde kuruluşunuzun etki alanına katılan aygıtlarını ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz. Bunlar, hem şirket içi Active Dizininize hem de Azure Etkin Dizininize katılan aygıtlardır. Karma Azure AD birleştirilmiş aygıtlar Microsoft 365 Business tarafından korunabilir ve yönetilebilir. 
  
Windows 10 cihazlarınızı Karma Azure AD'nin Microsoft 365 Business tarafından birleştirilmiş ve yönetildiği yapmak için aşağıdaki adımları tamamlayın.
  
1. **Dizin Eşitlemesi için hazırlanın**: Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden [önce, Office 365'e dizin eşitlemesi için hazırla'yı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin. Özellikle:

   - Aşağıdaki öznitelikler için dizininizde yineleme bulunmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**. Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır...
   
   - Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğinin lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırılmasını önerdik. Örneğin **mary@contoso.local** yerine **mary.shelley@contoso.com**
   
   - Active Directory etki alanı **.com** veya **.org**gibi bir internet routable sonek yerine **.local** veya **.lan**gibi bir routable olmayan sonek biterse, ilk olarak açıklandığı gibi yerel kullanıcı hesaplarının UPN soneki ayarlamanız gerekir [Dizin eşitleme için routable olmayan bir etki alanı hazırlayın.](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization) 

2. **Azure AD Bağlantısını yükleme ve yapılandırma**: Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'ten Dizin eşitleme sihirbazını çalıştırın. Bkz. Daha fazla bilgi edinmek [için Office 365 için dizin eşitlemesi ayarla.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)
    
    > [!NOTE]
    > Adımlar Microsoft 365 Business için tam olarak aynıdır. 
    
Azure AD Connect seçeneklerinizi yapılandırırken, **Parola Senkronizasyonu** ve **Sorunsuz Tek Oturum**Açma özelliğinin yanı sıra Microsoft 365 Business'ta da desteklenen parola **yazma** özelliğini etkinleştirmenizi öneririz.

> [!NOTE]
> Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır. Nasıl [Yapılır'a bakın: parola yazmayı yapılandırma](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Karma Azure REKLAM Birleştirme'yi Yapılandırın**: Windows 10 aygıtların Karma Azure AD'ye katılmasını etkinleştirmeden önce aşağıdaki ön koşulları yerine getirebildiğinizden emin olmalısınız:

   - Azure AD bağlantısının en son sürümünü çalıştırıyorsunuz.

   - Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti. Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.

Karma Azure AD'nin katıldığı varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydetmek [için, Öğreticideki adımları izleyin: Yönetilen etki alanları için karma Azure Active Directory join'i yapılandırın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Bu, varolan şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını sağlar ve bulutları hazır hale getirecektir.
    
4. **Windows 10 için otomatik kaydı etkinleştirin**: Mobil aygıt yönetimi için Windows 10 aygıtlarını Intune'da otomatik olarak kaydetmek için Grup [İlkesi'ni kullanarak otomatik olarak bir Windows 10 aygıtı kaydedin'e](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)bakın. Grup İlkesi'ni yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için Grup İlkesi Yönetim Konsolu ve ADMX şablonlarını kullanarak Etki Alanı Denetleyicinizde bu grup ilkesi ayarını oluşturabilirsiniz.

5. **Yapılandın Sorunsuz Tek Oturum Açma**: Sorunsuz SSO, kullanıcıları kurumsal bilgisayarları kullandıklarında Otomatik olarak Microsoft 365 bulut kaynaklarına oturum alacaktır. [Azure Active Directory Seamless Tek Oturum Açma: Hızlı başlangıç'ta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)açıklanan iki Grup İlkesi seçeneğinden birini dağıtmanız yeterlidir. **Grup İlkesi** seçeneği kullanıcıların ayarlarını değiştirmesine izin vermezken, **Grup İlkesi Tercihi** seçeneği değerleri ayarlar, aynı zamanda kullanıcı tarafından yapılandırılabilir bırakır.

6. **Windows Hello for Business**'ı ayarlama : Windows Hello for Business, parolaları yerel bir bilgisayarda oturum açmak için güçlü iki faktörlü kimlik doğrulama (2FA) ile değiştirir. Bir faktör asimetrik anahtar çifti, diğeri ise aygıtınız destekliyorsa parmak izi veya yüz tanıma gibi bir PIN veya diğer yerel harekettir. Parolaları mümkün olduğunca 2FA ve Windows Hello for Business ile değiştirmenizi tavsiye ettik.

İşletmeler için Karma Windows Merhaba'yı yapılandırmak [için, İş Önkoşulları için Karma Anahtar güven Windows Hello'yu gözden geçirin.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs) Ardından, İş [için Karma Windows Merhaba'yı yapılandırma yönergelerini](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)izleyin anahtar güven ayarları. 
