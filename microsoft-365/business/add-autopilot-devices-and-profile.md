---
title: AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
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
ms.openlocfilehash: 56225424125e9eed9f46867837c564aa5d1c4adc
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982170"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.

Cihazların çalışanlarınıza verdiğiniz anda üretken kullanıma hazır olması için, kuruluşunuza yönelik yeni Windows 10 cihazlarını Windows AutoPilot ile ayarlayabilirsiniz.
  
## <a name="device-requirements"></a>Cihaz gereksinimleri

Cihazların şu gereksinimleri karşılaması gerekir:
  
- Windows 10, sürüm 1703 veya üstü.
    
- Windows ilk çalıştırma deneyimi uygulanmamış olan yeni cihazlar.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma

Henüz cihaz grubu veya profil oluşturmadıysanız başlamanın en iyi yolu adım adım kılavuzu kullanmaktır. Bununla birlikte, kılavuzu kullanmadan da [cihaz ekleyebilir](create-and-edit-autopilot-devices.md) ve bu cihazlara [profil atayabilirsiniz](create-and-edit-autopilot-profiles.md). 
  
1. Microsoft 365 İş yönetim merkezinde **Cihaz eylemleri** kartını bulun ve **Windows'u Autopilot ile Dağıt**'ı seçin.
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. **Windows'u hazırlama** sayfasında **Başlangıç kılavuzuna** tıklayın veya dokunun.
    
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
    