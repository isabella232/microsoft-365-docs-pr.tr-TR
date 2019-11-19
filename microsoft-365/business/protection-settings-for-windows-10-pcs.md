---
title: Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Windows 10 aygıtlarını güvenli hale getirmek için Microsoft 365 Business'ta varsayılan ve diğer ayarlar hakkında bilgi edinin.
ms.openlocfilehash: 1846ee7ae09db94575ef27dcf4f5721661f7666d
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715212"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme

## <a name="secure-windows-10-devices"></a>Windows 10 cihazlarının güvenliğini sağlama

Microsoft 365 İş ile Windows 10 cihazlarının güvenliğini sağlama hakkındaki videoyu izleyin:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. 'deki <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine gidin. 
    
2. Sol daki gezinmede, **Aygıt** \> **İlkeleri** \> **Ekle'yi**seçin.
  
3. **İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin. 
    
4. **İlke türü**'nün altında **Windows 10 Cihaz Yapılandırması**'nı seçin.
    
5. Expand **Secure Windows 10 Devices** \> configure the settings how you would like. Daha fazla bilgi için [Kullanılabilir ayarlara](#available-settings)bakın. 
    
    Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
    
7. Son olarak, **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın. 
    
## <a name="available-settings"></a>Kullanılabilir ayarlar

Varsayılan olarak tüm ayarlar **Açık** durumdadır. Aşağıdaki ayarlar kullanılabilir.
  
Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md) 
  
|||
|:-----|:-----|
|Ayar  <br/> |Açıklama  <br/> |
|Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol  <br/> |Bilgisayarları internete bağlı olmanın getirdiği tehlikelerden korumak için Windows Defender Virüsten Koruma programının açık olması gerekir.  <br/> |
|Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol  <br/> |Edge'de, kullanıcıları kötü amaçlı sitelerden ve indirmelerden korumaya yardımcı olan ayarları açar.  <br/> |
|Cihazların saldırı alanını azaltan kuralları kullan  <br/> |Saldırı alanı azaltma özelliği açık olarak ayarlandığında zararlı yazılımlar tarafından cihazlara bulaşmak için tipik olarak kullanılan eylemleri ve uygulamaları engeller. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi edinmek için [Saldırı alanlarını azaltma](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) bölümüne bakın.  <br/> |
|Klasörleri fidye yazılımı gibi tehditlerden koruma  <br/> |Bu ayar, şirket verilerini fidye yazılımı gibi şüpheli veya zararlı uygulamalar tarafından gerçekleştirilen değişikliklere karşı korumak için denetimli klasör erişimini kullanır. Bu türdeki uygulamaların korumalı klasörlerde değişiklik yapması engellenir. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Bkz. Daha fazla bilgi edinmek için [Denetimli klasör erişimine sahip klasörleri koru.](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA)  <br/> |
|İnternetteki olası zararlı içeriklerin ağa erişimini engelle  <br/> |Kimlik avı dolandırıcılığı, yararlanma veya diğer kötü amaçlı içeriklere ev sahipliği yapan düşük itibarlı Internet konumlarına giden kullanıcı bağlantılarını engellemek için bu ayarı kullanın. Bu ayar yalnızca Windows Defender **Antivirus'ün Açık**olarak ayarlanması durumunda kullanılabilir. Daha fazla bilgi için [bkz.](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|BitLocker ile PC'lerdeki dosyaların ve klasörlerin yetkisiz erişime karşı korunmasına yardımcı ol  <br/> |BitLocker bilgisayar sabit sürücülerini şifreleyerek verileri korur ve bilgisayar kaybolduğunda veya çalındığında verilerin açığa çıkma durumuna karşı koruma sağlar. Daha fazla bilgi için [Bitlocker SSS](https://go.microsoft.com/fwlink/?linkid=871000)bölümüne bakın.  <br/> |
|Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver  <br/> |Kullanıcıların Microsoft Store'ndan uygulama indirmesine ve yüklemesine izin verir. Uygulamalar, oyunlardan üretkenlik araçlarına kadar her şeyi içerebilir, dolayısıyla bu ayar **Açık** durumdadır ancak ek güvenlik için kapatabilirsiniz.  <br/> |
|Kullanıcıların Cortana'ya erişmesine izin ver  <br/> |Cortana çok yararlı olabilir! Cortana ayarları sizin için açabilir veya kapatabilir, yol tarifi verebilir ve randevular için zamanında olduğunuzdan emin olabilir, bu nedenle bu ayarı varsayılan olarak **açıktır.**  <br/> |
|Kullanıcıların Microsoft'tan Windows ipucu ve reklam almasına izin ver  <br/> |Windows ipuçları kullanışlı olabilir ve yeni özellikler kullanıma sunulduğunda kullanıcıların yönlendirilmesine yardım edebilir.  <br/> |
|Windows 10 cihazları otomatik olarak güncelleştir  <br/> |Windows 10 cihazların son güncelleştirmeleri otomatik olarak aldığından emin olur.  <br/> |
|Cihaz şu kadar süre boşta kaldığında ekranı kapat  <br/> |Kullanıcı cihaz başında olmadığında şirket verilerinin korunmasını sağlar. Kullanıcı bir kafe gibi herkese açık bir konumda çalışıyorken kısa süreliğine uzaklaşabilir veya başka bir şeyle ilgilenebilir ve bu sırada diğer kişiler cihazdaki bilgilere bakabilir. Bu ayar sayesinde, ekran kapanmadan önce kullanıcının ne kadar süre boşta olabileceğini denetleyebilirsiniz.  <br/> |
