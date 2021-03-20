---
title: Etki alanına katılmış Windows 10 cihazlarının Microsoft 365 İş tarafından yönetilsini etkinleştirme
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Microsoft 365'in yalnızca birkaç adımda Active Directory'ye katılmış yerel Windows 10 cihazlarını korumayı nasıl etkinleştirebilirsiniz?
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913204"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş Ekstra tarafından yönetillerini etkinleştirme

Kuruluşta Windows Server Active Directory şirket içi kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 İş Ekstra'nın ayarlamasını yaparken, yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi de koruyabilirsiniz.
Bu korumayı ayarlamak için, Karma **Azure AD'ye katılmış cihazları kullanabilirsiniz.** Bu cihazlar hem şirket içi Active Directory'nize hem de Azure Active Directory'nize katılmış olur.

Bu videoda, bunu en yaygın senaryo için ayarlama adımları açıklanan ve aşağıdaki adımlarda da ayrıntılı olarak açıklanan bir senaryo yer almaktadır.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Başlamadan önce şu adımları tamamlayın:
- Azure AD Connect ile kullanıcıları Azure AD'ye eşitle.
- Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlama.
- Eşitleyilen tüm etki alanı kullanıcılarının Microsoft 365 İş Ekstra lisansları olduğundan emin olun.

Adımlar [için bkz. Etki alanı kullanıcılarını Microsoft'a](manage-domain-users.md) eşitleme.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Intune'da MDM Yetkilisini doğrulama

Uç Nokta [Yöneticisi'ne](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) gidin ve Microsoft Intune sayfasında  Cihaz kaydı'na tıklayın, ardından Genel Bakış sayfasında **MDM** yetkilisinin **Intune** olduğundan emin olun.

- **MDM yetkilisi Yok** **ise,** **MDM yetkilisini** **intune** olarak ayarlamak için tıklatın.
- **MDM** yetkilisi **Microsoft Office 365** ise Cihazları Kaydetme cihazlarına gidin ve   >   **Intune MDM** yetkilisini eklemek için sağdan **MDM** yetkili ekle iletişim kutusunu kullanın **(MDM** Yetkilisini Ekle iletişim kutusu yalnızca **MDM** Yetkilisi Microsoft Office 365 olarak ayarlanmışsa kullanılabilir).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Bilgisayarları birleştirme için Azure AD'nin etkinleştirildiğinden emin olun

- Yönetim merkezleri listesinden yönetim merkezine gidin ve Azure Active Directory'yi seçin (Azure Active Directory görünür durumda değilse hepsini <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **göster'i** seçin).  
- Azure **Active Directory yönetim merkezinde,** **Azure Active Directory'ye** gidin, Cihazlar'ı **ve ardından** Cihaz **ayarlarını seçin.**
- Kullanıcıların **cihazları Azure AD'ye katılanın etkinleştirildiğinden** emin olun 
    1. Tüm kullanıcıları etkinleştirmek için, All olarak **ayarlayın.**
    2. Belirli kullanıcıları etkinleştirmek için, belirli bir **kullanıcı grubunu** etkinleştirmek üzere Seçili olarak ayarlayın.
        - Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)
        - Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. MDM için Azure AD'nin etkinleştirildiğinden emin olun

- Yönetim merkezine gidin ve Uç Nokta Yönetimi t'yi seçin (Uç Nokta Yöneticisi görünür durumda <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> değilse Hepsini göster'i seçin)  
- Microsoft **Endpoint Manager yönetim merkezinde Cihazlar** Windows Kaydı Otomatik   >    >  **Kaydı'ne**  >  **gidin.**
- MDM kullanıcı kapsamının etkinleştirildiğinden emin olun.

    1. Tüm bilgisayarları kaydetmek için, Kullanıcılar Windows'a iş hesabı eklensinken Azure AD'ye katılmış tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydeden All olarak ayarlayın. 
    2. Belirli bir **kullanıcı** grubunun bilgisayarlarını kaydetmek için Bazıları olarak ayarlayın.
        -  Azure AD'de eşitlenen istenen etki alanı kullanıcılarını bir güvenlik [grubuna ekleyin.](../admin/create-groups/create-groups.md)
        -  Bu **güvenlik grubu için** MDM kullanıcı kapsamını etkinleştirmek için Grupları seç'i seçin.

## <a name="4-create-the-required-resources"></a>4. Gerekli kaynakları oluşturma 

Karma [Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) birleştirmesini yapılandırmak için gereken görevlerin gerçekleştirilip [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'i kullanımı basitleştirildi. Bu cmdlet'i çağırıldığında, gerekli hizmet bağlantı noktası ve grup ilkesi oluşturularak yapılandırılır.

Bir PowerShell örneğinden aşağıdakini kullanarak bu modülü yükleyebilirsiniz:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Bu modülü Azure AD Connect çalıştıran Windows Server'a yüklemeniz önerilir.

Gerekli hizmet bağlantı noktası ve grup ilkesi oluşturmak  [için, Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırmış olursunuz. Bu görevi gerçekleştirmek için Microsoft 365 İş Ekstra genel yönetici kimlik bilgileriniz gerekir. Kaynakları oluşturmaya hazır olduğunda, aşağıdakini çağırın:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

İlk komut Microsoft bulutuyla bağlantı kuracak ve sizden istendiğinde Microsoft 365 İş Ekstra genel yönetici kimlik bilgilerinizi belirtir.

## <a name="5-link-the-group-policy"></a>5. Grup İlkesini bağlama

1. Grup İlkesi Yönetim Konsolu'nda (GPMC), ilkeyi bağlamayı istediğiniz konuma sağ tıklayın ve bağlam menüsünden Var olan *bir GPO'ya bağla...* öğesini seçin.
2. Yukarıdaki adımda oluşturulan ilkeyi seçin ve Tamam'a **tıklayın.**

## <a name="get-the-latest-administrative-templates"></a>En son Yönetim Şablonlarını al

Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik **MDM** kaydı etkinleştir ilkesini görmüyorsanız bunun nedeni Windows 10, sürüm 1803 veya sonraki sürümlerde ADMX'in yüklü olması olabilir. Sorunu düzeltmek için şu adımları izleyin (Not: En son MDM.admx geriye doğru uyumludur):

1.  İndir: [Windows 10 Ekim 2020 Güncelleştirmesi (20H2)](https://www.microsoft.com/download/102157)için Yönetim Şablonları (.admx).
2.  Paketi Etki Alanı Denetleyicisi'ne yükleyin.
3.  Yönetim Şablonları sürümüne bağlı olarak şu klasöre gidin: **C:\Program Files (x86)\Microsoft Grup İlkesi\Windows 10 Ekim 2020 Güncelleştirmesi (20H2)**.
4.  Yukarıdaki **yolda İlke Tanımları** klasörünü **policyDefinitions olarak yeniden adlandırabilirsiniz.**
5.  **PolicyDefinitions klasörünü** varsayılan olarak **C:\Windows\SYSVOL\domain\Policies** konumunda bulunan SYSVOL paylaşımınıza kopyalayın. 
    -   Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, policyDefinitions içeriğini buraya ekleyin.
6.  Birden fazla Etki Alanı Denetleyici varsa, ilkelerin kullanılabilir olması için SYSVOL'nin çoğaltmasını bekleyin. Bu yordam, Yönetim Şablonları'nın gelecekteki tüm sürümü için de çalışır.

Bu noktada, varsayılan Azure AD kimlik bilgilerini kullanarak otomatik **MDM kaydı etkinleştirme ilkesine bakabilirsiniz.**