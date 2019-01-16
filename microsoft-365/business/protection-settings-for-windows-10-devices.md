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
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982830"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme

## <a name="create-an-app-management-policy-for-windows-10"></a>Windows 10 için uygulama yönetimi ilkesi oluşturma

Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.
  
1. Genel yönetici kimlik bilgileriyle [Microsoft 365 Business](https://portal.office.com)'da oturum açın. Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin. 
    
2. Yönetici portalındaki **Cihaz ilkeleri** kartında **İlke ekle**'yi seçin.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.
    
5. Altında ** aygıt türü **, **Kişisel** ya da **Şirket sahibi**seçin.
    
6. **İş dosyalarını şifrele** seçeneği otomatik olarak açılır. 
    
7. Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın. 
    
8. **Kullanıcıların Office dosyalarını aygıtlarda nasıl eriştiğini yönetmek** genişletin \> nasıl istediğiniz ayarları yapılandırın. ** **Kullanıcıların Office içeren aygıtlar mobil aygıtlarda nasıl eriştiğini yönetmek** varsayılan olarak kapalıdır** , ancak **bunu açın** ve varsayılan değerleri kabul tavsiye edilir. Daha fazla bilgi için bkz: [kullanılabilir ayarları](protection-settings-for-windows-10-devices.md#bkmk_settings) . 
    
    Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz. 
    
9. **Windows cihazlarındaki verileri kurtar** seçeneğini genişletin; bu seçeneği **Açık** duruma getirmeniz önerilir.
    
    Veri Kurtarma Aracısı sertifikasının konumuna göz atabilmeniz için, önce bir sertifika oluşturmanız gerekir. Yönergeler için bkz. [Şifreleme Dosya Sistemi (EFS) Veri Kurtarma Aracısı (DRA) sertifikasını oluşturma ve doğrulama](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir. Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir. Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir. Dosyanın şifresini çözmek için yönetici, Veri Kurtarma Aracısı (DRA) sertifikası kullanabilir.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Listelenen tüm uygulamalardaki dosyaların korunduğundan emin olmak için başka etki alanları veya SharePoint Online konumları eklemek istiyorsanız, **Ek ağ ve bulut konumlarını koru** seçeneğini genişletin. Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Sonra karar **Bu ayarları elde kim?** Varsayılan **Tüm kullanıcıların** güvenlik grubu kullanmak istemiyorsanız, **Değiştir**' i seçin, bu ayarları alırsınız güvenlik grupları seçin \> **seçin**.
    
12. Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Kullanıcıların Office iş dosyalarına erişimini yönetmek şu ayarlar kullanılabilir:
  
Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)
  
|**Ayar**|**Açıklama**|
|:-----|:-----|
|Office uygulamalarına erişirken PIN veya parmak izi iste  <br/> |Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.  <br/> |
|Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla  <br/> |Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.  <br/> |
|Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste  <br/> |Bu ayar, bir kullanıcının yeniden oturum açması istenmeden önce ne kadar süreliğine boşta kalabileceğini belirler.  <br/> |
   

