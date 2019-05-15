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
description: 365 korumak Microsoft etkinleştirmeyi öğrenin Yerel AD alanına katılmış Windows 10 aygıtlar.
ms.openlocfilehash: af0e78ef6e79bfd612b11a16538e7afcd377ffb0
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071560"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme

Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz. Bu ilk Active Directory Azure Windows 10 aygıtları ile Azure AD kaydetme ve bunları Microsoft 365 Business tarafından mobil aygıt yönetimi için kaydolma ve ardından, Active Directory ile eşitlenmesi yoluyla ayarlayabilirsiniz.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış aygıtları Ayarla

Kuruluşunuzun etki alanına katılmış aygıtları Azure yerinde Active Directory ek olarak Active Directory tarafından sağlanan yeteneklerinin sağladığı avantajlardan yararlanabilmenizi ayarlamak için **karma Azure AD alanına bağlı aygıtlar**uygulayabilirsiniz. Bunlar hem yerinde Active Directory ve Active Directory Azure katılan aygıtlardır. Karma Azure AD alanına bağlı aygıtların korumalı ve Microsoft 365 işletme tarafından yönetilir. 
  
Windows 10 aygıtlarınızın karma katıldı ve Microsoft 365 işletme tarafından yönetilen Azure Reklam yapmak için aşağıdaki adımları tamamlayın.
  
1. Azure Active Directory'ye, kullanıcıları, grupları ve yerel Active Directory'den kişileri eşitlemek için dizin eşitleme Sihirbazı ve Azure Active Directory [dizin eşitleme için Office 365 ayarlamak](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi bağlanmak çalışır.
    
    > [!NOTE]
    > Tam olarak Microsoft 365 iş için aynı adımlardır. 
  
2. Karma Azure AD alanına bağlı olarak Windows 10 aygıtları etkinleştirmek için 3 adım tamamlamadan önce aşağıdaki önkoşulları karşıladığından emin olmanız gerekir:

   - Azure AD'ın en son sürümünü çalıştırdığınızı bağlayın.

   - Azure AD bağlanmak karma Azure AD alanına dahil olmasını istediğiniz aygıtların tüm bilgisayar nesneleri eşitlendi. Bilgisayar nesnelerine ait belirli kuruluş birimleri (OU), sonra bu OU Azure AD alanında eşitleme için ayarlandığından emin olun, aynı zamanda bağlayın.
    
3. Karma Azure AD katılmış olması ve Mobil Aygıt Yönetimi tarafından Intune (Microsoft 365 iş) kaydolmak için varolan etki alanına katılmış Windows 10 aygıtları kaydedin:
    
4. [Karma Azure Active Directory alanına bağlı aygıtları yapılandırma hakkında](https://go.microsoft.com/fwlink/p/?linkid=872870)adım adım yönergeleri izleyin. Bu, şirket içi Active Directory eşitlemesine olanak sağlar Windows 10 bilgisayar katıldı ve bunları bulut hazır olun.
    
5. Windows 10 aygıt taşınabilir aygıt yönetimi için kaydolmak için [Grup İlkesi kullanarak Intune Windows 10 aygıtla kaydetmek](https://go.microsoft.com/fwlink/p/?linkid=872871) yönergeler için bkz. Grup İlkesi yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için etki alanı denetleyicisi sunucunuzda bu Grup İlkesi ayarı oluşturabilirsiniz.