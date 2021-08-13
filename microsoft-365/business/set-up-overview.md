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
description: Abone Microsoft 365 İş Ekstra, etki alanı ve kullanıcı eklemeye, güvenlik ilkelerini ayarlamaya ve daha fazlası için kurulum adımlarını öğrenin.
ms.openlocfilehash: 7c09dca354781bf92f6bbecca0f3fb9875fb654515fe35c2f96cc780a894a764
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803232"
---
# <a name="overview-of-setup"></a>Kuruluma genel bakış

Kurulum hakkında kısa bir Microsoft 365 İş Ekstra izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](../business-video/index.yml).

Kurulum adımlarının çoğu kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenmiştir.

## <a name="step-1-add-your-domain-and-users"></a>1. Adım: Etki alanınızı ve kullanıcılarınızı ekleme

   - **[Etki alanınızı](set-up.md#add-your-domain-to-personalize-sign-in)** ekleyin (etki alanınızı kaydol sırasında [satın aldıysanız,](sign-up.md)bu adım zaten bitti.)

   - **Kullanıcı ekle 'yi seçin.** Kullanıcıları şu üç şekilde ebilirsiniz:
        - Kılavuzlu [kurulumda](set-up.md#add-users-in-the-wizard).
        - Şirket içi Active [directory'niz varsa, Azure AD Bağlan](../enterprise/set-up-directory-synchronization.md) kullanarak kullanıcıları eklemek için dizin eşitlemesini kullanın.
        - Kullanıcıları daha [sonra yönetim merkezinden](../admin/add-users/add-users.md) de eklemeniz gerekir.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. Adım: Güvenlik ilkelerini ayarlama ve cihazları yapılandırma 

  - Cihaz ilkelerini [yapılandırmak için](set-up.md#protect-your-organization) kılavuzlu kurulumu kullanın. 
  - Ayrıca daha sonra yönetim merkezinde ve Intune [portalında](view-policies-and-devices.md) daha fazla ekleyebilir veya [bunları düzenleyebilirsiniz.](/intune/tutorial-walkthrough-intune-portal)
  - Kurulum sihirbazı, temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.
  
  Kurulum sihirbazında güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:

- **E-posta kötü amaçlı yazılıma karşı koruma**
- **Kimlik avı için Defender'da kimlik Office 365**
- **Exchange Online Arşivleme**
- **Azure Information Protection (Plan1)**

Bunun için bkz. [tehdit korumasını artırma](increase-threat-protection.md) [ve uyumluluk özelliklerini ayarlama.](set-up-compliance.md)

Ayrıca, en iyi güvenlik uygulamalarının yol haritası için Microsoft 365 İş Ekstra en iyi [10](/office365/admin/security-and-compliance/secure-your-business-data) güvenlik yolunu da inceleyebilirsiniz.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. Adım: Cihazlarınızı ayarlama Windows 10 yönetme

Rehberli kurulumu tamamlandıktan sonra, tüm bilgisayarlarınızı ve Windows 10 korumanız gerekir.
  
- Windows 10 Pro, Microsoft 365 İş Ekstra'in [](pre-requisites-for-data-protection.md) önkoşullarıdır, ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'niz varsa, aboneliğiniz size Windows 10 Pro yükseltme [hakkı Windows 10 Pro.](./upgrade-to-windows-pro-creators-update.md)
- Mobil cihazlara yönelik [ilkeleri Windows 10 için güvenli](secure-win-10-pcs.md) bilgisayarlardaki Windows 10 izleyin.

bir Windows 10 Azure AD'ye katılsanız, bu cihaza Windows 10 ilkeler uygulanır. Daha fazla bilgi için [bkz. Windows için cihaz Microsoft 365 ayarlama](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. Adım: Yükleme İş için Microsoft 365 Uygulamaları
- Kurulum sihirbazını Office bilgisayarınıza Windows bilgisayarınıza otomatik [olarak yükleyebilirsiniz.](set-up.md#deploy-office-365-client-apps)
- Kullanıcıların [e-Office cihazlar için](/office365/admin/setup/install-applications) Windows uygulamaları yüklemesine izin verin.
     
## <a name="advanced"></a>Gelişmiş
- **Yeni cihazları ayarlamak için AutoPilot'i kullanma**
            
     Bir kullanıcının yeni Windows cihazlarını otomatik olarak  Windows 10 için [AutoPilot'a](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin [](https://www.microsoft.com/solution-providers/search) için yapacak bir iş ortağını almak daha kolay olabilir. Ayrıca Microsoft Store ['a](https://go.microsoft.com/fwlink/?linkid=874598)gidebilir ve bir bulut teknolojisi uzmanının satın aldığınız yeni cihazları ayarlamalarını sorabilirsiniz.

- **Şirket içi access kaynakları**

     - Kuruluşta şirket Windows Server Active Directory kullanıyorsa, Microsoft 365 İş Ekstra cihazlarınızı korumak için Windows 10 ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi korumaya devam etmek için Windows 10'i kurabilirsiniz. Bu özelliği ayarlamak [için Etki alanına katılmış Windows 10 cihazlarını bu cihazlar](manage-windows-devices.md) tarafından Microsoft 365 İş Ekstra adımlarını izleyin. Bu tercih edilen yöntemdir ve bu durumdaki cihazlar Karma Azure AD'ye katılmış cihazlar olarak adlandırılan cihazlar.

    - İşletmenizin bazı şirket içi kaynakları (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory'niz varsa, Azure AD'ye katılmış cihazlarınıza şu adımları takip edin: [Microsoft 365 İş Ekstra'te Azure AD'ye](access-resources.md)katılmış bir cihazdan şirket içi kaynaklara erişme .

## <a name="related-content"></a>İlgili içerik

[Microsoft 365 eğitim videoları için giriş](../business-video/index.yml) (bağlantı sayfası)