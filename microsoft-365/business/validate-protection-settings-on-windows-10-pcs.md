---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 aygıtları'nda bulunan Microsoft 365 iş app koruma ayarlarını doğrulamak öğrenin.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983300"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir. Şirkete ait cihazlar için **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamalarını engelle ve iş dosyalarını OneDrive İş'e kaydetmelerini zorla** ayarını **Açık** duruma getirdiyseniz, kullanıcılar Azure AD'ye bağlanıp oturum açtıktan sonra bunu kullanıcının cihazında denetleyebilirsiniz. 
  
 **Bağlantı ayarlarını doğrulama**
  
1. [Microsoft 365 İş kullanıcıları için Windows cihazlarını ayarlama](set-up-windows-devices.md) konusunda açıklandığı gibi Microsoft 365 İş kimlik bilgileriyle oturum açtıktan ve Azure AD'ye bağlandıktan sonra, **Windows Ayarları** \> **Hesaplar** \> **İş yeri veya okula eriş** seçeneğine gidin. **Bağlanılan \<kiracı adı\> Azure AD**'yi seçin ve sonra da **Bilgi**'yi seçin.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. **Yöneten** \<kiracı adı\> sayfasında, aşağıdaki şekilde gösterilene benzer bir **Yönetim Sunucusu Adresi** içeren **Bağlantı bilgileri** kutusunu görebilirsiniz. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Şirket verilerini yönetilmeyen bir uygulamaya yapıştıramadığınızı doğrulama**
  
1. Microsoft 365 İş tarafından yüklenmiş olan Outlook 2016'yı açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulama içeriğe erişemiyor hatasını alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

 **Bağlantı ayarlarını doğrulama**
  
1. Yerel kullanıcı olarak oturum açtığınız Windows 10 kişisel cihazınızda **Windows Ayarları**'na gidin ve **Hesaplar** \> **İş yeri veya okula eriş**'e tıklayın veya dokunun.
    
2. **İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.
    
3. **İş yeri veya okul hesabı oluştur iletişim kutusu** \> **Oturum aç** için Microsoft 365 İş kimlik bilgilerinizi girin.
    
4. **İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. **İş yeri veya okula eriş** sayfasında, aşağıdaki şekilde gösterilene benzeyen ve içinde  **wip**  ile  **mam**  sözcükleri bulunan bir *Yönetim Sunucusu Adresi*'nin yer aldığı *Bağlantı bilgileri* kutusunu görebilirsiniz. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Şirket verilerini yönetilmeyen bir uygulamaya yapıştıramadığınızı doğrulama**
  
1. Outlook 2016'yı açın, gerekirse Microsoft 365 İş hesabınızı ekleyin ve Microsoft 365 İş kimlik bilgilerinizle oturum açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulama içeriğe erişemiyor hatasını alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    

