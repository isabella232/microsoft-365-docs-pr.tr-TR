---
title: Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Bir uygulama yönetimi ilkesi oluşturabilir ve iş dosyalarını Windows 10 aygıtlarda korumak öğrenin.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278206"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10 için uygulama yönetimi ilkesi oluşturma

Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.
  
1. [Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=837890) genel yönetim kimlik bilgileri ile oturum açın. Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin. 
    
2. **Aygıtlar** üzerinde sol nav, seçim \> **ilkeleri** \> **Ekle**.

3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.
    
5. Under ** Device type **, choose either **Personal** or **Company Owned**.
    
6. **İş dosyalarını şifrele** seçeneği otomatik olarak açılır. 
    
7. Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın. 
    
8. Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. Daha fazla bilgi için bkz: [kullanılabilir ayarları](#available-settings). 
    
    Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz. 
    
9. **Windows cihazlarındaki verileri kurtar** seçeneğini genişletin; bu seçeneği **Açık** duruma getirmeniz önerilir.
    
    Veri Kurtarma Aracısı sertifikasının konumuna göz atabilmeniz için, önce bir sertifika oluşturmanız gerekir. Yönergeler için bkz. [Şifreleme Dosya Sistemi (EFS) Veri Kurtarma Aracısı (DRA) sertifikasını oluşturma ve doğrulama](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir. Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir. Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir. Dosyanın şifresini çözmek için yönetici, Veri Kurtarma Aracısı (DRA) sertifikası kullanabilir.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Listelenen tüm uygulamalardaki dosyaların korunduğundan emin olmak için başka etki alanları veya SharePoint Online konumları eklemek istiyorsanız, **Ek ağ ve bulut konumlarını koru** seçeneğini genişletin. Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
12. Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Kullanıcıların Office iş dosyalarına erişimini yönetmek şu ayarlar kullanılabilir:
  
Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> |Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.  <br/> |
|Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla  <br/> |Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.  <br/> |
|Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste  <br/> |Bu ayar, bir kullanıcının yeniden oturum açması istenmeden önce ne kadar süreliğine boşta kalabileceğini belirler.  <br/> |
   

