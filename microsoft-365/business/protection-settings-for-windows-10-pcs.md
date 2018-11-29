---
title: Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Varsayılan Windows 10 aygıtları güvenliğini sağlamak için Microsoft 365 işletmede bulunan diğer ayarlar hakkında bilgi edinin.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982150"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme

## <a name="secure-windows-10-devices"></a>Windows 10 cihazlarının güvenliğini sağlama

Microsoft 365 İş ile Windows 10 cihazlarının güvenliğini sağlama hakkındaki videoyu izleyin:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Genel yönetici kimlik bilgileriyle [Microsoft 365 Business](https://portal.office.com)'da oturum açın. 
    
2. Yönetim merkezinde, **Cihaz ilkeleri** kartında **İlke ekle**'yi seçin.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında **Windows 10 Cihaz Yapılandırması**'nı seçin.
    
5. **Güvenli Windows 10 aygıtları** genişletin \> nasıl istediğiniz ayarları yapılandırın. Daha fazla bilgi için bkz: [kullanılabilir ayarları](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) . 
    
    Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Sonra karar **Bu ayarları elde kim?** Eleman **değişikliği**, varsayılan **tüm kullanıcıların** güvenlik grubu kullanmak istemiyorsanız, bu ayarları alırsınız güvenlik grubu için arama \> **seçin**.
    
7. Son olarak, **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Varsayılan olarak tüm ayarlar **Açık** durumdadır. Aşağıdaki ayarlar kullanılabilir.
  
Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md) 
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol  <br/> |Bilgisayarları İnternet'e bağlı olmanın tehlikelerinden korumak için Windows Defender Virüsten Koruma programının açık olmasını gerektirir.  <br/> |
|Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol  <br/> |Edge'de, kullanıcıları kötü amaçlı sitelerden ve indirmelerden korumaya yardımcı olan ayarları açar.  <br/> |
|Cihazların saldırı alanını azaltan kuralları kullan  <br/> |Saldırı alanı azaltma özelliği açık olarak ayarlandığında zararlı yazılımlar tarafından cihazlara bulaşmak için tipik olarak kullanılan eylemleri ve uygulamaları engeller. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi edinmek için [Saldırı alanlarını azaltma](https://go.microsoft.com/fwlink/?linkid=870417) bölümüne bakın.  <br/> |
|Klasörleri fidye yazılımı gibi tehditlerden koruma  <br/> |Bu ayar, şirket verilerini fidye yazılımı gibi şüpheli veya zararlı uygulamalar tarafından gerçekleştirilen değişikliklere karşı korumak için denetimli klasör erişimini kullanır. Bu türdeki uygulamaların korumalı klasörlerde değişiklik yapması engellenir. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi almak için [Denetimli klasör erişimi ile klasörleri koruma](https://go.microsoft.com/fwlink/?linkid=870418) bölümüne bakın.  <br/> |
|İnternetteki olası zararlı içeriklerin ağa erişimini engelle  <br/> |Kimlik avı dolandırıcılığı, açıkları kötüye kullanan yazılımlar veya diğer zararlı içerikleri barındırabilecek, güvenilirliği düşük İnternet konumlarına yönelik giden kullanıcı bağlantılarını engellemek için bu ayarı kullanın. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi için [Ağınızı koruma](https://go.microsoft.com/fwlink/?linkid=870419) bölümüne bakın.  <br/> |
|BitLocker ile PC'lerdeki dosyaların ve klasörlerin yetkisiz erişime karşı korunmasına yardımcı ol  <br/> |BitLocker bilgisayar sabit sürücülerini şifreleyerek verileri korur ve bilgisayar kaybolduğunda veya çalındığında verilerin açığa çıkma durumuna karşı koruma sağlar. Daha fazla bilgi için [Bitlocker SSS](https://go.microsoft.com/fwlink/?linkid=871000) bölümüne bakın.  <br/> |
|Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver  <br/> |Kullanıcıların Microsoft Store'ndan uygulama indirmesine ve yüklemesine izin verir. Uygulamalar, oyunlardan üretkenlik araçlarına kadar her şeyi içerebilir, dolayısıyla bu ayar **Açık** durumdadır ancak ek güvenlik için kapatabilirsiniz.  <br/> |
|Kullanıcıların Cortana'ya erişmesine izin ver  <br/> |Cortana çok yararlı olabilir! Cortana sizin yerinize ayarları açıp kapatabilir, yol tarif edebilir ve randevularınıza zamanında gitmenizi sağlayabilir; dolayısıyla bu ayar varsayılan olarak **Açık** durumdadır.  <br/> |
|Kullanıcıların Microsoft'tan Windows ipucu ve reklam almasına izin ver  <br/> |Windows ipuçları kullanışlı olabilir ve yeni özellikler kullanıma sunulduğunda kullanıcıların yönlendirilmesine yardım edebilir.  <br/> |
|Windows 10 cihazları otomatik olarak güncelleştir  <br/> |Windows 10 cihazların son güncelleştirmeleri otomatik olarak aldığından emin olur.  <br/> |
|Cihaz şu kadar süre boşta kaldığında ekranı kapat  <br/> |Kullanıcı cihaz başında olmadığında şirket verilerinin korunmasını sağlar. Kullanıcı bir kafe gibi herkese açık bir konumda çalışıyorken kısa süreliğine uzaklaşabilir veya başka bir şeyle ilgilenebilir, bu durumda cihaz rastgele bakışlara açık hale gelir. Bu ayar sayesinde ekran kapanmadan önce kullanıcının ne kadar süre boşta olabileceğini denetleyebilirsiniz.  <br/> |
   
  

