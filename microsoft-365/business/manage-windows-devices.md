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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564963"
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

portal.azure.com gidin ve Intune için sayfa arama üst kısmında.
Microsoft Intune sayfasında Cihaz **kaydını** seçin ve **Genel Bakış** sayfasında **MDM yetkilisinin** **Intune**olduğundan emin olun.

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

## <a name="4-set-up-service-connection-point-scp"></a>4. Servis bağlantı noktasını (SCP) ayarlama

Bu [adımlar, karma azure AD birleştirme](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)yapılandırmabasitleştirilmiştir. Adımları tamamlamak için Azure AD Connect'i ve Microsoft 365 Business Premium global yöneticinizi ve Active Directory yönetici parolalarınızı kullanmanız gerekir.

1.  Azure AD Connect'i başlatın ve sonra **Yapıla'yı**seçin.
2.  Ek **görevler** sayfasında, **aygıtı yapılandır'ı**seçin ve **sonra İleri'yi**seçin.
3.  Genel **Bakış** sayfasında **İleri'yi**seçin.
4.  **Azure'a Bağlan AD** sayfasında, Microsoft 365 Business Premium için global bir yöneticinin kimlik bilgilerini girin.
5.  Aygıt **seçenekleri** sayfasında, **Karma Azure AD birleştirme'yi yapılandır'ı**ve **ardından İleri'yi**seçin.
6.  **SCP** sayfasında, Azure AD Connect'in SCP'yi yapılandırmasını istediğiniz her orman için aşağıdaki adımları tamamlayın ve **sonra İleri'yi**seçin:
    - Orman adının yanındaki kutuyu işaretleyin. Orman, AD alan adınız olmalıdır.
    - Kimlik **Doğrulama Hizmeti** sütununda açılır dosyayı açın ve eşleşen etki alanı adını seçin (yalnızca tek bir seçenek olmalıdır).
    - Etki alanı yöneticisi kimlik bilgilerini girmek için **Ekle'yi** seçin.  
7.  Aygıt **işletim sistemleri** sayfasında yalnızca Windows 10 veya daha sonraki etki alanına bağlı aygıtları seçin.
8.  **Yapılandırmaya Hazır** **sayfasında, Yapılandırma'yı**seçin.
9.  Yapılandırma **tam** **sayfasında, Exit'i**seçin.


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Intune Kayıt için bir GPO oluşturma – ADMX yöntemi

Kullanın. ADMX şablon dosyası.

1.  AD sunucusunda oturum açın, **Sunucu Yöneticisi**  >  **Araçları**Grup  >  **İlkesi Yönetimi'ni**arayın ve açın.
2.  **Etki Alanları** altında etki alanı adınızı seçin ve **Yeni'yi**seçmek için **Grup İlkesi Nesneleri'ni** sağ tıklatın.
3.  Yeni GPO'ya bir ad verin, örneğin "*Cloud_Enrollment*" ve sonra **Tamam'ı**seçin.
4.  **Grup İlkesi Nesneleri** altındaki yeni GPO'ya sağ tıklayın ve **Edit'i**seçin.
5.  Grup **İlkesi Yönetimi**Düzenleyicisi'nde, **Bilgisayar Yapılandırma**  >  **İlkeleri**  >  **Yönetim Şablonları**Windows  >  **Components**  >  **MDM'ye**gidin.
6. **Varsayılan Azure AD kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir'e** sağ tıklatın ve ardından Etkin **Enabled**  >  **Tamam'ı**seçin. Editör penceresini kapatın.

> [!IMPORTANT]
> **Varsayılan Azure REKLAM kimlik bilgilerini kullanarak otomatik MDM kaydını etkinleştir**ilkesini görmüyorsanız, bkz. [Get the latest Administrative Templates](#get-the-latest-administrative-templates)

## <a name="6-deploy-the-group-policy"></a>6. Grup İlkesini Dağıtmak

1.  Sunucu Yöneticisi'nde, **Etki Alanları** > Grup İlkesi nesneleri altında, "Cloud_Enrollment" gibi yukarıdaki Adım 3'ten GPO'yu seçin.
2.  GPO'nuz için **Kapsam** sekmesini seçin.
3.  GPO'nun Kapsam sekmesinde, **Linkler**altındaki etki alanına bağlantısağ tıklayın.
4.  GPO'yu dağıtmak için **Zorla'yı** seçin ve onay ekranında **Tamam'ı** seçin.

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

