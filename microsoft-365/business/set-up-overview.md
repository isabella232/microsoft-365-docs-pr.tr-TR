---
title: Kuruluma genel bakış
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Aboneden etki alanı ve kullanıcı eklemeye, güvenlik ilkelerini ayarlamaya ve daha birçok işlemi yapmak için Microsoft 365 İş Ekstra'ya yönelik kurulum adımlarını öğrenin.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579944"
---
# <a name="overview-of-setup"></a>Kuruluma genel bakış

Microsoft 365 İş Ekstra kurulumu hakkında kısa bir video izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Kurulum adımlarının çoğu kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenir.

## <a name="step-1-add-your-domain-and-users"></a>1. Adım: Etki alanınızı ve kullanıcılarınızı ekleme

   - **[Etki alanınızı](set-up.md#add-your-domain-to-personalize-sign-in)** ekleyin (kayıt sırasında etki alanınızı [satın aldıysanız,](sign-up.md)bu adım zaten tamamdır.)

   - **Kullanıcı ekle 'yi seçin.** Kullanıcıları şu üç şekilden herhangi birini eklemenin yolları vardır:
        - Kılavuzlu [kurulumda.](set-up.md#add-users-in-the-wizard)
        - Şirket içi Active [directory'niz varsa, Azure AD Connect](../enterprise/set-up-directory-synchronization.md) kullanarak kullanıcıları eklemek için dizin eşitlemesini kullanın.
        - Kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de ebilirsiniz.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. Adım: Güvenlik ilkelerini ayarlama ve cihazları yapılandırma 

  - Cihaz ilkelerini [yapılandırmak için](set-up.md#protect-your-organization) kılavuzlu kurulumu kullanın. 
  - Ayrıca, daha sonra yönetim merkezinde ve Intune [portalında](view-policies-and-devices.md) daha fazla ekleyebilir veya [bunları düzenleyebilirsiniz.](/intune/tutorial-walkthrough-intune-portal)
  - Kurulum sihirbazı ayrıca temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.
  
  Kurulum sihirbazında güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:

- **E-posta kötü amaçlı yazılıma karşı koruma**
- **Office 365 için Defender'da kimlik avı önleme**
- **Exchange Online Arşivleme**
- **Azure Information Protection (Plan1**)

Başlamak için tehdit [korumasını artırmaya bakın](increase-threat-protection.md) [ve uyumluluk özelliklerini ayarlayın.](set-up-compliance.md)

En iyi [güvenlik uygulamalarının yol haritası için Microsoft 365 İş Ekstra'nızı](/office365/admin/security-and-compliance/secure-your-business-data) güvenli hale etmenin en iyi 10 yolunu da inceleyebilirsiniz.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. Adım: Windows 10 cihazlarını ayarlama ve yönetme

Rehberli kurulumu tamamlandıktan sonra, organizasyonınızdaki tüm Windows 10 bilgisayarlarını korumak istediğinizden emin olun.
  
- Windows 10 Pro, Microsoft 365 İş Ekstra'nın önkoşullarıdır, ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'nız varsa, aboneliğiniz [size Windows 10 Pro'ya](./upgrade-to-windows-pro-creators-update.md)yükseltme hakkı sağlar. [](pre-requisites-for-data-protection.md)
- Windows [10 cihazlarına yönelik](secure-win-10-pcs.md) ilkeleri ayarlamak için güvenli Windows 10 bilgisayarlarında adımları izleyin.

Bir Windows 10 cihazına Azure AD'ye katılsanız, Windows 10 bilgisayarlar için ayarınızdaki ilkeler bu cihaza uygulanır. Daha fazla bilgi için bkz. [Microsoft 365 kullanıcıları](set-up-windows-devices.md)için Windows cihazlarını ayarlama.

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. Adım: Microsoft 365 İş Uygulamalarını yükleme
- Kurulum sihirbazını kullanarak Windows cihazlarına Office'i otomatik [olarak yükleyebilirsiniz.](set-up.md#deploy-office-365-client-apps)
- Kullanıcıların Windows [ve cihazlar için Office](/office365/admin/setup/install-applications) uygulamalarını yüklemesine izin verin.
     
## <a name="advanced"></a>Gelişmiş
- **Yeni cihazları ayarlamak için Autopilot'a kullanma**
            
     Yeni Windows 10 cihazlarını bir  kullanıcı için otomatik olarak önceden yapılandırmak için [Windows Autopilot'u](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin için yapacak bir iş ortağını almak daha kolay olabilir. [](https://www.microsoft.com/solution-providers/search) Ayrıca Microsoft [Store'a gidip](https://go.microsoft.com/fwlink/?linkid=874598)bir bulut teknolojisi uzmanının satın aldığınız yeni cihazları ayarlamalarını da sebilirsiniz.

- **Şirket içi kaynaklara erişme**

     - Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 İş Ekstra'nın ayarlamasını yaparken, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz. Bu ayarı yapmak [için etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş Ekstra](manage-windows-devices.md) tarafından yönetilsin. Tercih edilen yöntem budur ve bu durumdaki cihazlar Karma Azure AD'ye katılmış cihazlar olarak adlandırılan cihazlar.

    - İşletmenizin bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'si varsa, Azure AD'ye katılmış cihazlarınıza şu adımları takip edin: [Microsoft 365 Business Premium'da Azure AD'ye](access-resources.md)katılmış bir cihazdan şirket içi kaynaklara erişme.

## <a name="see-also"></a>Ayrıca bk.

[İş için Microsoft 365 eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)