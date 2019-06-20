---
title: Ayarlama, genel bakış
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 iş kurma adımları genel bakış.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086410"
---
# <a name="overview-of-setup"></a>Kurulum, genel bakış

Kurulum sihirbazındaki adımları ayarlamak çoğu yapılabilir, ancak diğer seçenekler de listelenir.


## <a name="step-1-add-your-domain-and-users"></a>Adım 1: etki alanı ve kullanıcı ekleme

   - **[Etki alanınızın Ekle](set-up.md#add-your-domain-to-personalize-sign-in)** ( [kayıt](sign-up.md)sırasında etki alanı satın aldıysanız, bu adımı zaten yapılır.)

    - **Kullanıcı Ekle**. Herhangi üç yoldan biriyle yapabilirsiniz:
        - [Sihirbaz](set-up.md#add-users-in-the-wizard).
        - Eğer yerinde Active directory directory eşitlemesi [Azure AD Connect kullanarak kullanıcı eklemek](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) için kullanın.
        - [Daha sonra kullanıcılar eklemek](add-users-m365b.md) Yönetim Merkezi'nde de kullanabilirsiniz.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. adım: güvenlik ilkelerini ayarlama ve aygıtları yapılandırma 

  - Aygıt ve güvenlik ilkelerini yapılandırmak için [Kurulum Sihirbazı](set-up.md#set-up-security-policies-and-device-configurations) ' nı kullanın. 
  - Ayrıca daha ekleyebilir veya daha sonra [Yönetim Merkezi](view-policies-and-devices.md) ve [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)düzenleyin.
  - Kurulum Sihirbazı'ndaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek, güvenliğini artırabilirsiniz:

      - **E-posta zararlı yazılımlara karşı koruma**
      - **Gelişmiş tehdit Koruması (ATP) güvenli bağlantılar**
      - **ATP güvenli ekler**
      - **ATP anti-phishing**
      - **Exchange Online Arşivleme**
      - **Veri kaybını önleme (DLP)**
      - **Azure bilgi koruma (Plan1**)

          Almak için bkz: [Gelişmiş güvenlik ilkelerini kurun](set-up-advanced-security.md)başladı.

        Ayrıca bkz: [Microsoft 365 işletmenizin güvenliğini sağlamak için üst 10 yolu](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) için bir yol haritası, en iyi güvenlik yöntemleri.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Adım 3: Ayarlanır ve Windows 10 aygıtları yönetme

   Windows 10 aygıt için Azure AD katıldığınızda, [Adım 2](#step-2-set-up-security-policies-and-configure-devices) ' de ayarladığınız ilkeleri uygulanan.

   - Windows 10 Pro Microsoft 365 iş için bir [ön gereksinim](pre-requisites-for-data-protection.md) olmakla birlikte, Pro Windows 7, Windows 8 Pro veya Windows 8.1 Pro varsa, aboneliğiniz, [Windows 10 Pro yükseltmek](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)için hakkı verir.
    - Windows 10 aygıtları ilkelerini yapılandırmak için [Kurulum Sihirbazı](set-up.md#set-up-security-policies-and-device-configurations) ' nı kullanın.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Office 365 iş yükleme
- [Kurulum Sihirbazı](set-up.md#deploy-office-365-client-apps)' nı kullanarak Windows aygıtlardan Office otomatik olarak yükleyebilir.
- Otomatik olarak [Office yükleme](auto-install-or-uninstall-office.md) Yönetim Merkezi'nden.
- Kullanıcıların [Office uygulamaları yüklemek](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows ve aygıtlar için olanak sağlar.
     
## <a name="advanced"></a>Gelişmiş
- **Yeni aygıtları için AutoPilot kullanın**
            
     [Windows Autopilot](add-autopilot-devices-and-profile.md) otomatik olarak **Yeni** bir kullanıcı Windows 10 aygıtları önceden yapılandırmak için kullanabilirsiniz, ancak sizin için bunu yapmak için bir [ortak](https://www.microsoft.com/solution-providers/search) almak daha kolay olabilir. [Microsoft mağaza](https://go.microsoft.com/fwlink/?linkid=874598) ve yeni aygıtlar için satın bir bulut teknoloji uzmanı ayarlamak isteyin.

- **Şirket içi kaynaklara erişmek**

     - Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz. Bunu ayarlamak için [Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış Windows 10 aygıtları etkinleştirme](manage-windows-devices.md) adımlarını izleyin. Tercih edilen yöntem budur ve bu durumda aygıtları karma Azure adı verilen AD alanına bağlı aygıtlar.

    - Bazı içeren Active Directory yerinde kaynaklar (örneğin, dosya paylaşımları ve yazıcılar), bu kaynakların Azure AD alanına bağlı aygıtlara erişiminizi burada adımları izleyerek verebilirsiniz İşletmenizde yerel varsa: [erişim şirket içi kaynaklardan bir 365 işletmede Azure AD alanına bağlı aygıt](access-resources.md).

  