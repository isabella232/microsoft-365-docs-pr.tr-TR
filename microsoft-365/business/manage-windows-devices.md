---
title: Etki alanına birleştirilmiş Windows 10 aygıtlarını iş için Microsoft 365 tarafından yönetilmesini etkinleştirin
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
description: Microsoft 365'in yerel Active-Directory'ye katılan Windows 10 aygıtlarını yalnızca birkaç adımda nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560853"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Etki alanına bağlı Windows 10 cihazlarının Microsoft 365 Business Premium tarafından yönetilmesini etkinleştirme

Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 cihazlarınızı korumak için Microsoft 365 Business Premium'u ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.
Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz. Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.

Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacağına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Başlamadan önce şu adımları tamamladığınızdan emin olun:
- Azure AD Connect ile kullanıcıları Azure AD ile senkronize edin.
- Azure AD Connect Kuruluş Birimi (OU) eşitlemeyi tamamlayın.
- Eşitlediğiniz tüm etki alanı kullanıcılarının Microsoft 365 Business Premium lisansına sahip olduğundan emin olun.

Bkz. Adımlar için [etki alanı kullanıcılarını Microsoft'a senkronize edin.](manage-domain-users.md)

## <a name="1-verify-mdm-authority-in-intune"></a>1. Intune MDM Yetki doğrulayın

[Endpoint Manager'a](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) gidin ve Microsoft Intune sayfasında Cihaz **kaydını**seçin ve ardından **Genel Bakış** sayfasında **MDM yetkilisinin** **Intune**olduğundan emin olun.

- **MDM yetkisi** **Yok**ise, **Intune**ayarlamak için **MDM yetkisini** tıklatın.
- **MDM yetkisi** **Microsoft Office 365**ise, **Aygıtlar**Kayıt  >  **aygıtlarına** gidin ve **Intune MDM** yetkilisi ekleme hakkını sağdaki **MDM yetki** ekle iletişim kutusunu kullanın **(MDM Yetkilisi Ekle** iletişim kutusu yalnızca **MDM Yetkilisi** Microsoft Office 365'e ayarlanırsa kullanılabilir).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Bilgisayarlara katılmak için Azure AD'nin etkinleştirildiğinden doğrulayın

- Yönetici merkezleri listesinde yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve Azure **Active Directory'yi** seçin (Azure **Admin centers** Etkin Dizini görünmüyorsa tümünü göster'i seçin). 
- Azure **Etkin Dizin yönetici merkezinde,** **Azure Etkin Dizin'e** gidin, **Aygıtlar'ı** seçin ve ardından **Aygıt ayarlarını seçin.**
- **Kullanıcıların Azure AD'de aygıtlara katılıp katılamayada** olabileceğini doğrulayın etkin 
    1. Tüm kullanıcıları etkinleştirmek için **Tümü'ne**ayarlayın.
    2. Belirli kullanıcıları etkinleştirmek için, belirli bir kullanıcı grubunu etkinleştirmek için **Seçili** olarak ayarlayın.
        - Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.
        - Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. MDM için Azure AD'nin etkinleştirildiğinden doğrulayın

- Yönetici merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve **Endpoint Managemen**t'yi seçin **(Endpoint Manager** görünmüyorsa **tümünü göster'i** seçin)
- Microsoft **Endpoint Manager yönetici merkezinde,** **Windows**Windows Kayıt Otomatik Kayıt Cihazlar  >  **Windows**  >  **Windows Enrollment**  >  **Automatic Enrollment**gidin.
- MDM kullanıcı kapsamının etkin olduğunu doğrulayın.

    1. Tüm bilgisayarları kaydetmek için, kullanıcılar Windows'a bir iş hesabı eklediğinde Azure AD'ye katılan tüm kullanıcı bilgisayarlarını ve yeni bilgisayarları otomatik olarak kaydetmek için **Tümü'ne** ayarlayın.
    2. Belirli bir kullanıcı grubunun bilgisayarlarını kaydetmek için **Bazıları'na** ayarlayın.
        -  Azure AD'de senkronize edilen istenen etki alanı kullanıcılarını bir [güvenlik grubuna](../admin/create-groups/create-groups.md)ekleyin.
        -  Bu güvenlik grubu için MDM kullanıcı kapsamını etkinleştirmek için **Grupları Seç'i** seçin.

## <a name="4-create-the-required-resources"></a>4. Gerekli kaynakları oluşturma 

[Karma Azure AD birleştirmeyapılandırmak](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) için gerekli görevlerin yerine getirilmesi, [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modülünde bulunan [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'inin kullanımı yla basitleştirilmiştir. Bu cmdlet'i çağırdığınızda, gerekli servis bağlantı noktası ve grup ilkesini oluşturur ve yapılandıracaktır.

PowerShell örneğinden aşağıdakileri çağırarak bu modülü yükleyebilirsiniz:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Bu modülü Azure AD Connect çalıştıran Windows Server'a yüklemeniz önerilir.

Gerekli servis bağlantı noktası ve grup ilkesini oluşturmak için [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet'ini çağırırsınız. Bu görevi yerine getirirken Microsoft 365 Business Premium global yönetici kimlik bilgilerinize ihtiyacınız olacaktır. Kaynakları oluşturmaya hazır olduğunuzda aşağıdakileri çağırın:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

İlk komut Microsoft bulutuyla bir bağlantı kurar ve sizden istendiğinde Microsoft 365 Business Premium global yönetici kimlik bilgilerinizi belirtin.

## <a name="5-link-the-group-policy"></a>5. Grup İlkesini Bağla

1. Grup İlkesi Yönetim Konsolu'nda (GPMC), politikayı bağlamak istediğiniz konuma sağ tıklayın ve bağlam menüsünden *varolan bir GPO'yu bağlayın...* seçeneğini belirleyin.
2. Yukarıdaki adımda oluşturulan ilkeyi seçin ve **ardından Tamam'ı**tıklatın.

## <a name="get-the-latest-administrative-templates"></a>En son Yönetim Şablonlarını Alın

**Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bunun nedeni Windows 10, sürüm 1803, sürüm 1809 veya sürüm 1903 için ADMX yüklü değil. Sorunu gidermek için aşağıdaki adımları izleyin (Not: en son MDM.admx geriye dönük uyumludur):

1.  Indirin: [Windows 10 Mayıs 2019 Güncelleştirmesi (1903) için Yönetim Şablonları (.admx)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Paketi Birincil Etki Alanı Denetleyicisi'ne (PDC) yükleyin.
3.  Klasöre sürülmeye bağlı olarak gidin: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 Mayıs 2019 Güncelleştirmesi (1903) v3**.
4.  **İlke** **Tanımları** klasörünü yukarıdaki yolda Yeniden adlandırın.
5.  **İlke Tanımlar** klasörünü **C:\Windows\SYSVOL\domain\İlkeler'e**kopyalayın. 
    -   Tüm etki alanınız için merkezi bir ilke deposu kullanmayı planlıyorsanız, PolicyDefinitions'ın içeriğini oraya ekleyin.
6.  İlkenin kullanılabilir olması için Birincil Etki Alanı Denetleyicisini yeniden başlatın. Bu yordam, gelecekteki herhangi bir sürüm için de çalışacaktır.

Bu noktada, kullanılabilir varsayılan Azure **REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir** ilkesini görebilmeniz gerekir.
