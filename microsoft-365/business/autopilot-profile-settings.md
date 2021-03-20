---
title: AutoPilot Profili ayarları hakkında
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: AutoPilot profilleri, Windows'un kullanıcı cihazlarına nasıl yük olduğunu denetlemeye yardımcı olur. Profiller, Cortana yüklemesini atlama gibi varsayılan ve isteğe bağlı ayarlar içerir.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913388"
---
# <a name="about-autopilot-profile-settings"></a>AutoPilot Profili ayarları hakkında

## <a name="autopilot-profile-settings"></a>AutoPilot profil ayarları

Kullanıcı cihazlarına Windows'un nasıl yük olduğunu kontrol etmek için AutoPilot profillerini kullanabilirsiniz. Profiller aşağıdaki ayarları içerir.
  
 **Otomatik olarak ayarlanmış AutoPilot varsayılan özellikleri (gerekli):**
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Cortana, OneDrive ve OEM kaydını atlama  <br/> |Cortana ve kişisel OneDrive gibi tüketici uygulamalarının yüklemesini atlar. Kullanıcı cihazda yerel yönetici olduğu sürece cihaz kullanıcısı bunları daha sonra yükleyebilir. Cihaz Microsoft 365 İş Ekstra tarafından yönetilecek olduğundan orijinal üretici kaydı atlanır.  <br/> |
|Şirket markanız ile oturum açma deneyimi  <br/> |Şirketinizin Microsoft [365](../admin/setup/customize-sign-in-page.md)Oturum Açma sayfasına şirket markası eklemesi varsa, cihaz kullanıcısı oturum aken bu deneyimi edinecektir.  <br/> |
|Yapılandırılmış AAD hesaplarıyla MDM otomatik kaydı.  <br/> |Kullanıcı kimliği Azure Active Directory tarafından yönetiliyor ve kullanıcılar Windows ve Microsoft 365'te Microsoft 365 İş Ekstra kimlik bilgileriyle oturum aecek.  <br/> |
   
 **İsteğe bağlı ayarlar:**
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Gizlilik ayarlarını atla (Varsayılan olarak kapalı)  <br/> |Bu seçenek Açık olarak **ayarlanırsa,** cihaz kullanıcısı ilk kez oturum anlaşmayı kabul etmek için cihaz ve Windows lisans sözleşmesini görmez.  <br/> |
|Kullanıcının yerel yönetici olmasına izin verme  <br/> |Bu seçenek Açık olarak **ayarlanırsa,** cihaz kullanıcısı Cortana gibi hiçbir kişisel uygulama yükleyemz.<br/> |
