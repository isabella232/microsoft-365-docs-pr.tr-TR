---
title: Windows 10 cihazları için uygulama koruma ayarlarını düzenleme veya ayarlama
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Kullanıcılarınızı kişisel Windows 10 cihazlarında uygulama yönetimi ilkelerini oluşturma veya düzenlemeyi ve iş dosyalarını korumayı öğrenin.
ms.openlocfilehash: aa270c563e6bdce6fd48f8713d7db3ce23921925
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580024"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Windows 10 cihazları için uygulama koruma ayarlarını ayarlama veya düzenleme

Bu makale Microsoft 365 İş Ekstra için geçerlidir.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Windows 10 için uygulama yönetimi ilkesi düzenleme

1. Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin:     
2. Sol gezintide Cihaz **İlkeleri'ne** \> **seçin.**
1. Var olan bir Windows uygulama ilkesi seçin ve ardından **Düzenle'yi seçin.**
1. Değiştirmek **istediğiniz** ayarın yanındaki Düzenle'yi ve ardından Kaydet'i **seçin.**

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10 için uygulama yönetimi ilkesi oluşturma

Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.
  
1. Yönetim merkezine <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> gidin: 
2. Sol gezintide Cihaz **İlkeleri** \> **Ekle'yi** \> **seçin.**
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
4. **İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.
5. Cihaz **türü altında,** Kişisel'i **veya Şirkete** **Ait'i seçin.**
6. **İş dosyalarını şifrele** seçeneği otomatik olarak açılır. 
7. Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın. 
9. **Windows cihazlarda Verileri kurtar'ı genişletin.** Bu açmanizi **öneririz.**
    Veri Kurtarma Aracısı sertifikasının bulunduğu konuma göz atmadan önce bir sertifika oluşturmanız gerekir. Yönergeler için, Şifreleme [Dosyası Sistemi (EFS)](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)Veri Kurtarma Aracısı (DRA) sertifikası oluşturma ve doğrulama.
    
    Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir. Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir. Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir. Yönetici, dosyanın şifresini çözmek için Veri Kurtarma Aracısı (DRA) sertifikasını kullanabilir.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Listelenen **tüm uygulamalardaki dosyaların** korun olduğundan emin olmak için ek etki alanları veya SharePoint Online konumları eklemek için Ek ağ ve bulut konumlarını koru'ya genişletin. Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
12. Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.