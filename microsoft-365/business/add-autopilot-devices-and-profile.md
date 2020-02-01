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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: İşletmeniz için yeni Windows 10 aygıtları ayarlamak için Windows AutoPilot'u nasıl kullanacağınızı öğrenin.
ms.openlocfilehash: 1fd0abb76d16b79dd11ef27b6b27a87894d89ef9
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593283"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>AutoPilot cihaz ve profilleri eklemek için adım adım kılavuzu kullanın.

Windows AutoPilot'u, işletmeniz için **yeni** Windows 10 aygıtları ayarlamak için kullanabilirsiniz, böylece bunları çalışanlarınıza verdiğinizde kullanıma hazır olurlar.
  
## <a name="device-requirements"></a>Cihaz gereksinimleri

Aygıtlar bu gereksinimleri karşılamalıdır:
  
- Windows 10, sürüm 1703 veya sonrası
    
- Windows'dan kutudan çıkma deneyiminden geçmemiş yeni aygıtlar
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Cihaz ve profil oluşturmak için kurulum kılavuzunu kullanma

[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Henüz aygıt grupları veya profiller oluşturmadıysanız, başlamanın en iyi yolu adım adım kılavuzu kullanmaktır. Ayrıca, kılavuzu kullanmadan [aygıtlar ekleyebilir](create-and-edit-autopilot-devices.md) ve [onlara profil atayabilirsiniz.](create-and-edit-autopilot-profiles.md) 
  
1. 'deki <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine gidin.

2. Soldaki gezinti bölmesine **Aygıtlar** \> **Otomatik Pilot'u**seçin.

    ![Yönetici merkezinde, aygıtları ve ardından Otomatik Pilot'u seçin.](media/AutoPilot.png)
  
2. Otomatik **Pilot** sayfasında **Başlat kılavuzuna**tıklayın veya dokunun.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Cihazların **listesi sayfasının bulunduğu Upload .csv dosyasında,** hazır bulunduğunuz konuma göz atın. CSV dosyası, ardından \> **Sonraki'ni Aç.** **** Dosyanın üç üstbilgi olmalıdır:
    
    - A sütunu: Cihaz Seri Numarası
    
    - B sütunu: Windows Ürün Kimliği
    
    - C sütunu: Donanım Numarası
    
    Bu bilgileri donanım satıcınızdan alabilir veya Bir CSV dosyası oluşturmak için [Get-WindowsAutoPilotInfo PowerShell komut dosyasını](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) kullanabilirsiniz. 
    
    Daha fazla bilgi için bkz. [Cihaz listesi CSV dosyası](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). **Cihaz listesiyle .csv dosyası yükleme** sayfasında bir örnek dosya da indirebilirsiniz. 
    
4. Profil sayfası **atarken,** varolan bir profili seçebilir veya yeni bir profil oluşturabilirsiniz. Henüz bir tane yoksa, bir tane oluşturmanız istenir. 
    
    Profil, tek bir cihaza veya bir cihaz grubuna uygulanabilen ayarlar koleksiyonudur.
    
    Varsayılan özellikler gereklidir ve otomatik olarak ayarlanır. Varsayılan özellikler şunlardır:
    
    - Cortana, OneDrive ve OEM kaydını atlayın.
    
    - Şirketinizin markasıyla oturum açma deneyimi oluşturma.
    
    - Aygıtlarınızı Azure Active Directory hesaplarına bağlayın ve otomatik olarak Microsoft 365 Business tarafından yönetilecek şekilde kaydedin.
    
    Daha fazla bilgi için [Otomatik Pilot Profil ayarları hakkında](autopilot-profile-settings.md)bilgi sahibi olayın. 
    
5. Diğer ayarlar, **Gizlilik ayarlarını atla** ve **Kullanıcının yerel yönetici olmasına izin verme** şeklindedir. Varsayılan olarak ikisi de **Kapalı** durumdadır. 
    
    **İleri**'yi seçin.
    
6. **Bittiyseniz,** oluşturduğunuz (veya seçtiğiniz) profilin, aygıt listesini yükleyerek oluşturduğunuz aygıt grubuna uygulanacağını gösterir. Aygıt kullanıcıları bir sonraki oturum açtığında ayarlar etkin olacaktır. **Kapat**'ı seçin.
    