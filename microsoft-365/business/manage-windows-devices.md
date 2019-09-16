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
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992239"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme

Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz. Bunu, önce Active Directory ile senkronize ederek, ardından Windows 10 aygıtlarını Azure AD'ye kaydederek ve Microsoft 365 Business tarafından mobil cihaz yönetimine kaydederek ayarlayabilirsiniz.
Aşağıdaki video, bunu en yaygın senaryo için nasıl ayarlayabilmek için gereken adımları ayrıntılarıyla açıklar.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Microsoft 365 Business tarafından yönetilecek etki alanı birleştirilmiş aygıtları ayarlama

Kurum içi Active Directory'ye ek olarak Azure Active Directory tarafından sağlanan özelliklerden yararlanacak şekilde kuruluşunuzun etki alanına katılan aygıtlarını ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz. Bunlar, hem şirket içi Active Dizininize hem de Azure Etkin Dizininize katılan aygıtlardır. Karma Azure AD birleştirilmiş aygıtlar Microsoft 365 Business tarafından korunabilir ve yönetilebilir. 
  
Windows 10 cihazlarınızı Karma Azure AD'nin Microsoft 365 Business tarafından birleştirilmiş ve yönetildiği yapmak için aşağıdaki adımları tamamlayın.
  
1. Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure Etkin Dizin Bağlantısı'nı çalıştırın.
    
    > [!NOTE]
    > Adımlar Microsoft 365 Business için tam olarak aynıdır. 
  
2. Windows 10 aygıtların Karma Azure AD'ye katılmasını sağlamak için 3.

   - Azure AD bağlantısının en son sürümünü çalıştırıyorsunuz.

   - Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti. Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.
    
3. Karma Azure AD Joined olmak üzere varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydedin ve Bunları Intune (Microsoft 365 Business) tarafından mobil cihaz yönetimine kaydedin:
    
4. [Karma Azure Active Directory'yi birleştirme aygıtlarını yapılandırma](https://go.microsoft.com/fwlink/p/?linkid=872870)konusunda adım adım yönergeleri izleyin. Bu, şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını sağlar ve bulutları hazır hale getirecektir.
    
5. Mobil aygıt yönetimi için bir Windows 10 aygıtı kaydetmek için, talimatlar için [Bir Grup İlkesi kullanarak Bir Windows 10 aygıtını Intune'a](https://go.microsoft.com/fwlink/p/?linkid=872871) kaydedin' e bakın. Grup İlkesi'ni yerel bir bilgisayar düzeyinde veya toplu işlemler için ayarlayabilirsiniz, etki alanı denetleyici sunucunuzda bu grup ilkesi ayarını oluşturabilirsiniz.