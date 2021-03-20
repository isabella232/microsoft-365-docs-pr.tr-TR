---
title: AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: İşletmeniz için çalışan kullanımına hazır olacak şekilde yeni Windows 10 cihazlarını ayarlamak üzere Windows AutoPilot'u nasıl kullanabileceğinizi öğrenin.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913512"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.

Windows AutoPilot'u kullanarak **işletmeniz** için yeni Windows 10 cihazlarını çalışanlarınıza verdiyken kullanıma hazır olacak şekilde kurabilirsiniz.
  
## <a name="device-requirements"></a>Cihaz gereksinimleri

Cihazlar şu gereksinimleri karşılamalıdır:
  
- Windows 10, sürüm 1703 veya sonrası
    
- Windows'un ilk gelen deneyimine henüz sahip olmayan yeni cihazlar
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma

[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)

Henüz cihaz grupları veya profil oluşturmadınız, kullanmaya başlamanın en iyi yolu adım adım kılavuzu kullanmaktır. Ayrıca, [kılavuzu kullanmadan](create-and-edit-autopilot-devices.md) [cihazlar ekleyebilir ve](create-and-edit-autopilot-profiles.md) onlara profil atabilirsiniz. 
  
1. Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin:

2. Sol gezinti bölmesinde Cihazlar  \> **AutoPilot'ı seçin.**

    ![Yönetim merkezinde cihazları ve ardından AutoPilot'ı seçin.](../media/AutoPilot.png)
  
2. **AutoPilot sayfasında Kılavuzu** başlat'a tıklayın **veya dokunun.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Cihaz **listesinin bulunduğu .csv dosyasını** karşıya yükle sayfasında, hazır bulundurarak bir konuma gidin. CSV dosyasını ve ardından **Sonrakini** \> **Aç'ı seçin.** Dosyanın üç üst bilgisi olmalı:
    
    - A sütunu: Cihaz Seri Numarası
    
    - B sütunu: Windows Ürün Kimliği
    
    - C sütunu: Donanım Numarası
    
    Bu bilgileri donanım satıcıdan edinebilirsiniz veya CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) betiği kullanabilirsiniz. 
    
    Daha fazla bilgi için bkz. [Cihaz listesi CSV dosyası](../admin/misc/device-list.md). **Cihaz listesiyle .csv dosyası yükleme** sayfasında bir örnek dosya da indirebilirsiniz. 
    
> [!NOTE]
> Bu betikte, müşterinin Windows Autopilot'a cihaz kaydetmesi için gereken özellikleri almak için ISEMN kullanılır. Sonuçta elde edilen CSV dosyasının Windows Ürün Kimliği (PKID) değerini toplamamanın normal olduğunu unutmayın, çünkü bu bir cihazı kaydetmek için gerekli değildir ve PKID'nin CSV çıktısı CSV'de NULL olması tamamen iyidir. Yalnızca seri numarası ve donanım karması doldurulur.
    
4. Profil **atama sayfasında,** mevcut bir profili seçebilirsiniz veya yeni bir profil oluşturabilirsiniz. Henüz bir tane yoksa, bir tane oluşturmanız istenir. 
    
    Profil, tek bir cihaza veya bir cihaz grubuna uygulanabilen ayarlar koleksiyonudur.
    
    Varsayılan özellikler gereklidir ve otomatik olarak ayarlanır. Varsayılan özellikler şunlardır:
    
    - Cortana, OneDrive ve OEM kaydını atla.
    
    - Şirketinizin markasıyla oturum açma deneyimi oluşturma.
    
    - Cihazlarınızı Azure Active Directory hesaplarına bağlanın ve bunları Microsoft 365 İş Ekstra tarafından yönetilleri için otomatik olarak kaydettirin.
    
    Daha fazla bilgi için [bkz. AutoPilot Profili ayarları hakkında.](autopilot-profile-settings.md) 
    
5. Diğer ayarlar, **Gizlilik ayarlarını atla** ve **Kullanıcının yerel yönetici olmasına izin verme** şeklindedir. Varsayılan olarak ikisi de **Kapalı** durumdadır. 
    
    **İleri**'yi seçin.
    
6. **Oluşturduğunuz (veya** seçtiğiniz) profilin, cihaz listesini yükerek oluşturduğunuz cihaz grubuna uygulan olacağını gösterir. Ayarlar, cihaz kullanıcıları bir sonraki oturum açmada etkili olur. **Kapat**'ı seçin.
