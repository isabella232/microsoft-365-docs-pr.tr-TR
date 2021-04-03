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
description: Windows 10 cihazlarında Microsoft 365 İş Ekstra uygulama koruma ayarlarını doğrulayın ve kullanıcıların şirket verilerini kişisel dosyalara veya yönetilmeyen uygulamalara kopyalayamalarını doğrulayın.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579872"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir. Kullanıcıların şirket  verilerini kişisel dosyalara kopyalamasını engelle ayarını etkinleştirirseniz ve şirkete ait cihazlar için iş dosyalarını **OneDrive** İş ayarına kaydetmelerini zorlarsanız, Azure AD'ye bağlandıktan ve oturum açınktan sonra kullanıcının cihazında bunu kontrol edebilirsiniz. 
  
 **Bağlantı ayarlarını doğrulama**
  
1. Microsoft 365 İş Ekstra kimlik bilgileriyle oturum açın ve [Microsoft 365 İş](set-up-windows-devices.md)Ekstra kullanıcıları için Windows cihazlarını ayarlama konusunda açıklandığı gibi Azure AD'ye bağlanın, iş veya okul için **Windows** Ayarları Hesapları Erişimi'ne \>  \> gidin. **\<tenant name\> Azure AD'ye Bağlan'ı** ve ardından Bilgi'yi **seçin.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Yönetilen **sayfasında,** aşağıdaki şekilde gösterilene benzer bir \<tenant name\> Yönetim Sunucusu Adresi **içeren** Bağlantı  bilgilerini görebilirsiniz. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramay işleminizi doğrulama**
  
1. Microsoft 365 İş Ekstra tarafından yüklenmiş olan Outlook 2016'ya açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulamanın içeriğe erişe olmadığını haber alan bir hata alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

 **Bağlantı ayarlarını doğrulama**
  
1. Yerel kullanıcı olarak oturum açtığınız Windows 10 kişisel aygıtınızda, **Windows** Ayarları'na  gidin ve Hesaplar Erişimi'ne iş veya okul tıklayın \> **veya dokunun.**
    
2. **İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.
    
3. İş veya okul hesabı ayarla iletişim kutusunda Microsoft 365 İş Ekstra kimlik **bilgilerinizi** \> **girin.**
    
4. **İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.
    
    ![İş veya okul hesabı iletişim kutusunda Bilgi'ye tıklayın veya dokunun.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Access **iş** veya okul sayfasında, aşağıdaki  şekilde gösterilene benzer bir **Yönetim** Sunucusu Adresi içeren ve içinde *wip* ve mam sözcükleri bulunan Bağlantı *bilgilerini* görebilirsiniz. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramay işleminizi doğrulama**
  
1. Outlook 2016'yi açın, gerekirse Microsoft 365 İş Ekstra hesabını ekleyin ve Microsoft 365 İş Ekstra kimlik bilgilerinizle oturum açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulama'nın içeriğe erişe olmadığını haber alan bir hata alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    

