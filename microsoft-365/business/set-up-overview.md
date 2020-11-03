---
title: Kuruluma genel bakış
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business Premium için kurulum adımlarını, abone olmak, etki alanı ve kullanıcıları eklemeye, güvenlik ilkelerini ayarlamayı ve daha fazlasını öğrenin.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842140"
---
# <a name="overview-of-setup"></a>Kuruluma genel bakış

Microsoft 365 Business Premium kurulumu hakkında kısa bir video izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

Kurulum adımlarının çoğu Kılavuzlu kurulumda yapılabilir, ancak diğer seçenekler de listelenir.

## <a name="step-1-add-your-domain-and-users"></a>Adım 1: etki alanınızı ve kullanıcılarınızı ekleme

   - **[Etki alanınızı ekleyin](set-up.md#add-your-domain-to-personalize-sign-in)** ( [kaydolma](sign-up.md)sırasında etki alanınızı satın aldıysanız, bu adım zaten yapılır.)

   - **Kullanıcıları ekleyin**. Kullanıcıları üç şekilde ekleyebilirsiniz:
        - [Kılavuzlu kurulumda](set-up.md#add-users-in-the-wizard).
        - Şirket içi Active Directory 'niz varsa [Azure AD Connect 'i kullanarak kullanıcıları eklemek](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) için dizin eşitlemesi kullanın.
        - Ayrıca, [daha sonra Yönetim merkezinde kullanıcı ekleyebilirsiniz](add-users-m365b.md) .
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Adım 2: güvenlik ilkelerini ayarlama ve cihazları yapılandırma 

  - Cihaz ilkelerini yapılandırmak için [Kılavuzlu kurulumu](set-up.md#protect-your-organization) kullanın. 
  - Ayrıca, daha sonra [Yönetim merkezinde](view-policies-and-devices.md) ve [Intune portalında](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)daha fazla ekleyebilir veya düzenleyebilirsiniz.
  - Kurulum Sihirbazı ayrıca temel tehdit koruması ve veri kaybı önleme ayarlarını da ayarlar.
  
  Kurulum sihirbazındaki güvenlik ayarlarına ek olarak, aşağıdaki ayarları ekleyerek güvenliğinizi artırabilirsiniz:

- **Eposta koruması**
- **Office 365 Defender 'da kimlik avını önleme**
- **Exchange Online Arşivleme**
- **Azure bilgi koruması (Plan1** )

Başlamak için [tehdit korumasını arttırın](increase-threat-protection.md) ve [uyumluluk özelliklerini ayarlayın](set-up-compliance.md).

[Microsoft 365 Iş ekstra için güvenli](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) bir yol haritası-en iyi güvenlik uygulamaları

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Adım 3: Windows 10 cihazlarını ayarlama ve yönetme

Kılavuzlu kurulumu tamamladıktan sonra, kuruluşunuzdaki tüm Windows 10 bilgisayarlarını korumanız gerekecektir.
  
- Windows 10 Pro, Microsoft 365 Business Premium için bir [önkoşuldur](pre-requisites-for-data-protection.md) , ancak Windows 7 Pro, Windows 8 Pro veya Windows 8,1 Pro kullanıyorsanız, aboneliğiniz [Windows 10 Pro 'ya yükseltme](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)yapmanız aboneliğiniz.
- Windows 10 cihazlarında ilkeler ayarlamak için [Windows 10 bilgisayarlarında güvenli](secure-win-10-pcs.md) olan adımları izleyin.

Windows 10 bilgisayarlarında bir Windows 10 aygıtına katıldığınızda, Windows 10 bilgisayarlarında ayarladığınız ilkeler buna uygulanır. Daha fazla bilgi için bkz: [Microsoft 365 kullanıcıları Için Windows cihazları ayarlama](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Adım 4: işletmeler için Microsoft 365 uygulamalarını yükleme
- [Kurulum sihirbazını](set-up.md#deploy-office-365-client-apps)kullanarak Windows cihazlarında Office 'i otomatik olarak yükleyebilirsiniz.
- Kullanıcıların Windows için [Office uygulamalarını](https://docs.microsoft.com/office365/admin/setup/install-applications) ve aygıtlarını yüklemesini sağlayın.
     
## <a name="advanced"></a>Gelişmiş
- **Yeni cihazları ayarlamak için Autopilot 'ı kullanma**
            
     [Windows Autopilot](add-autopilot-devices-and-profile.md) 'ı kullanarak bir kullanıcı için **Yeni** Windows 10 cihazlarını otomatik olarak yapılandırabilirsiniz, ancak bunu sizin için yapabileceği bir [iş ortağı](https://www.microsoft.com/solution-providers/search) almanız daha kolaydır. Ayrıca, [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)'a gidebilir ve bir bulut teknoloji uzmanından satın aldığınız yeni cihazları kurulumunu isteyebilirsiniz.

- **Şirket içi kaynaklara erişme**

     - Kuruluşunuzda Windows Server Active Directory 'yi şirket içinde kullanıyorsanız, Microsoft 365 Iş ekstra 'ı, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürmeye devam ederken Windows 10 aygıtlarınızı korumak için ayarlayabilirsiniz. Bu ayarı ayarlamak için [etki alanı odaklı Windows 10 aygıtlarının Microsoft 365 Iş ekstra tarafından yönetilmesini sağlama](manage-windows-devices.md) konusundaki adımları izleyin. Bu tercih edilen yöntemdir ve bu durumdaki cihazlar karma Azure AD birleştirilmiş cihazları olarak adlandırılır.

    - İşletmenizde bazı şirket içi kaynaklar (dosya paylaşımları ve yazıcılar gibi) içeren yerel bir Active Directory varsa, buradaki adımları izleyerek Azure AD-birleştirilmiş cihazlarınıza bu kaynaklara erişim sağlayabilirsiniz: [Microsoft 365 Business Premium 'Da Azure AD 'a katılmış cihazından şirket içi kaynaklara erişim](access-resources.md)sağlayabilirsiniz.

## <a name="see-also"></a>Ayrıca bkz.

[Microsoft 365 iş eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
