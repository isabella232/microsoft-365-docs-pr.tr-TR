---
title: AutoPilot Profili ayarları hakkında
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profilleri, kullanıcı cihazlarına Windows ayarları denetlemeye yardımcı olur. Profiller, yükleme işlemini atlama gibi varsayılan ve Cortana içerir.
ms.openlocfilehash: 67ad6e92583d71207e2807657a7ad00261e1249291e2e6a7546f544ea924b394
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896333"
---
# <a name="about-autopilot-profile-settings"></a>AutoPilot Profili ayarları hakkında

## <a name="autopilot-profile-settings"></a>AutoPilot profil ayarları

AutoPilot profillerini kullanarak, kullanıcı cihazlarına Windows postanın nasıl yük olduğunu kontrol edin. Profiller aşağıdaki ayarları içerir.
  
 **Otomatik olarak ayarlanmış AutoPilot varsayılan özellikleri (gerekli):**
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Kayıt Cortana, OneDrive OEM kaydı atla  <br/> |Kişisel ve kişisel müşteri uygulamaları gibi tüketici Cortana yüklemesini OneDrive. Kullanıcı cihazda yerel yönetici olduğu sürece cihaz kullanıcısı bunları daha sonra yükleyebilir. Orijinal üretici kaydı atlanır çünkü cihaz diğer üretici tarafından Microsoft 365 İş Ekstra.  <br/> |
|Şirket markanız ile oturum açma deneyimi  <br/> |If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.  <br/> |
|Yapılandırılmış AAD hesaplarıyla MDM otomatik kaydı.  <br/> |Kullanıcı kimliği E-posta Azure Active Directory tarafından yönetilir ve kullanıcılar kendi kimlik Windows ile Microsoft 365 oturum Microsoft 365 İş Ekstra.  <br/> |
   
 **İsteğe bağlı ayarlar:**
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Gizlilik ayarlarını atla (Varsayılan olarak Kapalı)  <br/> |Bu seçenek On olarak **ayarlanırsa,** cihaz kullanıcısı cihazın lisans sözleşmelerini görmez ve Windows ilk kez oturum a açınca oturum açın.  <br/> |
|Kullanıcının yerel yönetici olmasına izin verme  <br/> |Bu seçenek Açık olarak **ayarlanırsa,** cihaz kullanıcısı Kullanıcı Hesabı gibi hiçbir kişisel Cortana.<br/> |
