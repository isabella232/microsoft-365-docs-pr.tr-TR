---
title: AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: İşletmeniz için yeni Windows 10 aygıtları kurmak için Windows AutoPilot kullanmayı öğrenin.
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660699"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.

Windows AutoPilot, çalışanlarınıza vermediğiniz sürece bunlar üretken kullanılmak üzere hazır olacak şekilde işletmeniz için **Yeni** Windows 10 aygıtları belirlemek için kullanabilirsiniz.
  
## <a name="device-requirements"></a>Cihaz gereksinimleri

Cihazların şu gereksinimleri karşılaması gerekir:
  
- Windows 10, sürüm 1703 veya üstü.
    
- Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma

![Üzerine kapak https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Henüz cihaz grubu veya profil oluşturmadıysanız başlamanın en iyi yolu adım adım kılavuzu kullanmaktır. Bununla birlikte, kılavuzu kullanmadan da [cihaz ekleyebilir](create-and-edit-autopilot-devices.md) ve bu cihazlara [profil atayabilirsiniz](create-and-edit-autopilot-profiles.md). 
  
1. Yönetim merkezinde mi <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. **Aygıtlar** üzerinde sol nav seçin \> **AutoPilot**.

    ![Yönetim Merkezi'nde aygıtları ve AutoPilot seçin.](media/AutoPilot.png)
  
2. **AutoPilot** sayfasında **Kılavuzu Başlat**' a dokunun veya tıklatın.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. **Cihaz listesiyle .csv dosyası yükleme** sayfasında, .CSV dosyanızın hazır bulunduğu konuma gidin ve sonra **Aç** \> **İleri**'yi seçin. Dosyada üç üst bilgi olmalıdır:
    
  - A sütunu: Cihaz Seri Numarası
    
  - B sütunu: Windows Ürün Kimliği
    
  - C sütunu: Donanım Numarası
    
    Bu bilgileri donanım satıcınızdan edinebilir veya CSV dosyasını oluşturmak için [Get-WindowsAutoPilotInfo PowerShell betiğini](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz. 
    
    Daha fazla bilgi için bkz. [Cihaz listesi CSV dosyası](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). **Cihaz listesiyle .csv dosyası yükleme** sayfasında bir örnek dosya da indirebilirsiniz. 
    
4. **Profil atama** sayfasında mevcut bir profili seçebilir veya yeni bir profil oluşturabilirsiniz. Henüz profiliniz yoksa yenisini oluşturmanız istenir. 
    
    Profil, tek bir cihaza veya bir cihaz grubuna uygulanabilen ayarlar koleksiyonudur.
    
    Varsayılan özellikler gereklidir ve otomatik olarak ayarlanır. Varsayılan özellikler şunlardır:
    
  - Cortana, OneDrive ve OEM kaydı atlanır.
    
  - Şirketinizin markasıyla oturum açma deneyimi oluşturma.
    
  - Cihazlarınız Azure Active Directory hesaplarına bağlanır ve Microsoft 365 İş tarafından yönetilmek üzere otomatik olarak kaydedilir.
    
    Daha fazla bilgi için bkz.
    
    [AutoPilot Profili ayarları hakkında](autopilot-profile-settings.md) . 
    
5. Diğer ayarlar, **Gizlilik ayarlarını atla** ve **Kullanıcının yerel yönetici olmasına izin verme** şeklindedir. Varsayılan olarak ikisi de **Kapalı** durumdadır. 
    
    **İleri**'yi seçin.
    
6. **Hepsi bu kadar** sayfası oluşturduğunuz (veya seçtiğiniz) profilin, cihaz listesini yükleyerek oluşturduğunuz cihaz grubuna uygulanacağı anlamına gelir. Cihaz kullanıcıları bir daha oturum açtığında bu ayarlar geçerli olur. **Kapat**'ı seçin.
    