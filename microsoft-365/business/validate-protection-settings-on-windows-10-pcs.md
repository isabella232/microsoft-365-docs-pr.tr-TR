---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Mobil Microsoft 365 İş Ekstra koruma ayarlarını doğrulayın Windows 10 kullanıcıların şirket verilerini kişisel dosyalara veya yönetilmeyen uygulamalara kopyalayamalarını doğrulayın.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861765"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir. Şirkete ait  cihazlar için Kullanıcıların şirket verilerini kişisel dosyalara kopyalamalarını engelle ve iş dosyalarını **OneDrive İş'e** kaydetmelerini zorla ayarını Açık olarak ayarlarsanız, kullanıcılar Azure AD'ye bağlandıktan ve oturum aktan sonra bunu kullanıcının cihazında kontrol edebilirsiniz. 
  
 **Bağlantı ayarlarını doğrulama**
  
1. Microsoft 365 İş Ekstra kullanıcıları için Windows cihazları ayarlama konusunda açıklandığı gibi Azure [](set-up-windows-devices.md)AD ile oturum açın ve Azure AD'ye bağlanın ve Microsoft 365 İş Ekstra Hesaplarına erişme (İş veya okul) için Windows Ayarlar hesaplarına  \>  \> **erişme 'ye gidin.** **\<tenant name\> Azure AD'ye bağlı'yi** seçin ve sonra da Bilgi **'yi seçin.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Yönetilen **sayfasında,** aşağıdaki şekilde gösterilene benzer bir Yönetim Sunucusu \<tenant name\> **Adresi içeren** Bağlantı  bilgileri'ne bakın. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştırama işleminizi doğrulama**
  
1. Microsoft 365 İş Ekstra Outlook 2016 tarafından yüklenmiş olan diğer Microsoft 365 İş Ekstra.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulamanın içeriğe erişe olmadığını haber alan bir hata alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

 **Bağlantı ayarlarını doğrulama**
  
1. Yerel Windows 10 oturum açtığınız kişisel cihazınızı kullanarak Hesap Ekle seçeneğine gidin ve Hesaplar İş yeri  veya okula erişim 'e Windows Ayarlar tıklayın \> **veya dokunun.**
    
2. **İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.
    
3. İş Microsoft 365 İş Ekstra veya okul hesabı **ayarla iletişim kutusuna oturum açmak için oturum açma bilgilerinizi** \> **girin.**
    
4. **İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.
    
    ![İş veya okul hesabı iletişim kutusunda Bilgi'ye tıklayın veya dokunun.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. İş veya **okula** erişim sayfasında, aşağıdaki  şekilde gösterilene  benzer bir Yönetim Sunucusu Adresi içeren ve içinde *wip* ile mam sözcükleri bulunan Bağlantı *bilgileri'ne* bakabilirsiniz. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştırama işleminizi doğrulama**
  
1. Oturum Outlook 2016 ve gerekirse Microsoft 365 İş Ekstra e-postanızı ekleyin ve kimlik bilgilerinizle Microsoft 365 İş Ekstra açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulama içeriğe erişemedi hatasını alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    

