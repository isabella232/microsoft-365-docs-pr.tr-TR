---
title: Kuruluma genel bakış
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business için kurulum adımlarının genel görünümü.
ms.openlocfilehash: 50f172c235aa06aa78fec60fc119ac7f568df308
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575598"
---
# <a name="overview-of-setup"></a>Kuruluma genel bakış

Kurulum adımlarının çoğu kurulum sihirbazında yapılabilir, ancak diğer seçenekler de listelenir.


## <a name="step-1-add-your-domain-and-users"></a>Adım 1: Etki alanınızı ve kullanıcılarınızı ekleyin

   - **[Etki alanınızı ekleyin](set-up.md#add-your-domain-to-personalize-sign-in)** [(kaydolma](sign-up.md)sırasında etki alanınızı satın aldıysanız, bu adım zaten tamamlanır.)

    - **Kullanıcı ekle.** Bunu üç şekilde yapabilirsiniz:
        - [Büyücüde.](set-up.md#add-users-in-the-wizard)
        - Şirket içinde Etkin dizininiz varsa [Azure AD Connect'i kullanarak kullanıcıları eklemek](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) için dizin eşitlemesi kullanın.
        - Daha sonra yönetici merkezine [de kullanıcı ekleyebilirsiniz.](add-users-m365b.md)
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Adım 2: Güvenlik ilkeleri ayarlama ve aygıtları yapılandırma 

  - Aygıt ve güvenlik ilkelerini yapılandırmak için [Kurulum sihirbazını](set-up.md#protect-data-and-devices) kullanın. 
  - Ayrıca daha fazla ekleyebilir veya daha sonra [yönetici merkezinde](view-policies-and-devices.md) ve [Intune portalında](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)bunları edebilirsiniz.
  - Kurulum sihirbazındaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:

      - **Kötü amaçlı yazılımkoruması e-postayla gönder**
      - **Gelişmiş Tehdit Koruması (ATP) Güvenli bağlantılar**
      - **ATP Güvenli Ekler**
      - **ATP kimlik avı önleme**
      - **Exchange Online Arşivleme**
      - **Veri Kaybı Önleme (DLP)**
      - **Azure Bilgi Koruması (Plan1**)

          Görmeye başlamak için [gelişmiş güvenlik ilkeleri ayarlayın.](set-up-advanced-security.md)

        Microsoft [365 Business'ınızı](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) en iyi güvenlik uygulamalarının yol haritası için güvence altına almanın en iyi 10 yolunu da görün.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Adım 3: Windows 10 aygıtlarını ayarlama ve yönetme

   Bir Windows 10 aygıtına Azure AD'ye katıldığınızda, [Adım 2'de](#step-2-set-up-security-policies-and-configure-devices) ayarladığınız ilkeler uygulanır.

   - Windows 10 Pro, Microsoft 365 Business için bir [ön koşuldur,](pre-requisites-for-data-protection.md) ancak Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro'nuz varsa, aboneliğiniz size [Windows 10 Pro'ya yükseltme](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)hakkı verir.
    - Windows 10 aygıtları için ilkeleri yapılandırmak için [Kurulum sihirbazını](set-up.md#protect-data-and-devices) kullanın.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Office 365 İş install
- [Kurulum sihirbazını](set-up.md#deploy-office-365-client-apps)kullanarak Office'i Windows aygıtlarına otomatik olarak yükleyebilirsiniz.
- Office'i yönetici merkezinden otomatik olarak [yükleyin.](auto-install-or-uninstall-office.md)
- Kullanıcıların Windows ve aygıtlar için [Office uygulamalarını yüklemesine](https://docs.microsoft.com/office365/admin/setup/install-applications) izin verin.
     
## <a name="advanced"></a>Gelişmiş
- **Yeni aygıtlar kurmak için Otomatik Pilot'u kullanma**
            
     Bir kullanıcı için **yeni** Windows 10 aygıtlarını otomatik olarak önceden yapılandırmak için [Windows Otomatik Pilot'u](add-autopilot-devices-and-profile.md) kullanabilirsiniz, ancak bunu sizin için yapabilecek bir [iş ortağı](https://www.microsoft.com/solution-providers/search) bulmak daha kolay olabilir. Ayrıca [Microsoft Mağazası'na](https://go.microsoft.com/fwlink/?linkid=874598) gidip bir bulut teknolojisi uzmanından sizin için satın aldığınız yeni aygıtlar ayarlamasını isteyebilirsiniz.

- **Şirket içi kaynaklara erişim**

     - Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz. Bunu ayarlamak için [Microsoft 365 Business tarafından yönetilecek etki alanına birleştirilmiş Windows 10 aygıtlarını etkinleştir](manage-windows-devices.md) metodu adımlarını izleyin. Bu tercih edilen yöntemdir ve bu durumdaki aygıtlar Karma Azure AD birleştirilmiş aygıtlar olarak adlandırılır.

    - İşletmenizde bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Etkin Dizin varsa, Azure AD'ye katılan aygıtlarınıza bu kaynaklara buradaki adımları izleyerek erişim sağlayabilirsiniz: [Şirket içi kaynaklara bir Microsoft 365 Business'ta Azure AD'ye bağlı aygıt.](access-resources.md)

  