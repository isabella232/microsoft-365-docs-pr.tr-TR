---
title: Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Windows 10 aygıtına katılan bir Azure Active Directory'den Line Of Business uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara nasıl erişebilirsiniz öğrenin.
ms.openlocfilehash: 2af5d4b4f84f39f5b157313e5b38ef030da7263d
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030544"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin

Azure Active Directory'nin birleştiği tüm Windows 10 aygıtları Office 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişebilir ve Microsoft 365 Business tarafından korunabilir. Ayrıca, Business Line (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim eizin vermek için, [Azure AD Connect'i](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)kullanarak şirket içi Active Directory'nizi Azure Etkin Dizini ile eşitlemeniz gerekir. 

Daha fazla bilgi edinmek [için Azure Active Directory'de aygıt yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction) e-giriş e bakın.
Adımlar da aşağıdaki bölümlerde özetlenmiştir.

## <a name="run-azure-ad-connect"></a>Azure AD Connect çalıştırın

Kuruluşunuzun Azure AD'sinin birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.
  
1. Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.
    
2. Dizin eşitlemesi tamamlandıktan sonra, kuruluşunuzun Windows 10 aygıtlarının Azure AD'ye katıldığından emin olun. Bu adım her Windows 10 aygıtında ayrı ayrı yapılır. Ayrıntılar [için Microsoft 365 Business kullanıcıları için Windows aygıtları ayarlama'ya](set-up-windows-devices.md) bakın. 
    
3. Windows 10 aygıtları Azure AD'ye katıldıktan sonra, her kullanıcı cihazlarını yeniden başlatmalı ve Microsoft 365 Business kimlik bilgileriyle oturum açmalıdır. Artık tüm aygıtlar şirket içi kaynaklara da erişeceksiniz.
    
Azure AD'ye katılan aygıtlar için şirket içi kaynaklara erişmek için ek adım gerekmez. Bu, Windows 10'da bulunan yerleşik işlevselliktir. 
  
Kuruluşunuz yukarıda açıklanan Azure AD Joined Aygıt Yapılandırmasında kullanıma hazır değilse, [Karma Azure AD Joined aygıt yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünün.
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Windows aygıtlarınızı Azure AD'ye katılırken dikkat edilmesi gerekenler

Azure AD'nin daha önce etki alanına veya bir çalışma grubunda bir araya getirilmiş bir Windows aygıtına katılması durumunda, aşağıdaki sınırlamaları göz önünde bulundurmanız gerekir:
  
- Bir aygıt Azure AD katıldığında, varolan bir profile başvurmadan yeni bir kullanıcı oluşturur. Bunu düzeltmek için profillerin el ile geçirilmesi gerekir. Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları, Başlat menüsü ayarları gibi bilgiler içerir. En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için bir üçüncü taraf aracı bulmaktır

- Aygıt Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPO'larda Intune'da karşılaştırılabilir bir [Yapılandırma Hizmet Sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir. Mevcut GPO'lar için karşılaştırılabilir CSP'ler bulmak için [MMAT aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırın.

- Kullanıcılar Active Directory kimlik doğrulamasına bağlı olan uygulamaların kimliğini doğrulayamayacaktır. Bu işlemle başa çıkmak için eski bir uygulamayı kullanarak değerlendirin ve mümkünse modern Auth kullanan bir uygulamaya güncellemeyi düşünün.

- Etkin Dizin yazıcı sı yatsı bulma çalışmaz. Bunu düzeltmek için, tüm kullanıcılar için doğrudan yazıcı yolları sağlayın veya [Karma Bulut Baskısından](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)yararlanın.
