---
title: Microsoft 365 Business için tehdit korumayı artırın
f1.keywords:
- NOCSH
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş Tehdit Koruması'nı ayarlayın ve hassas verileri kimlik avı, kötü amaçlı yazılım ve diğer tehditlere karşı koruyun.
ms.openlocfilehash: 17425de3f6e0022945899a559cf88575b6315a56
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561620"
---
# <a name="increase-threat-protection"></a>Tehdit korumayı artırın

Bu makale, kimlik avı, kötü amaçlı yazılım ve diğer tehditlere karşı koruma sağlamak için Microsoft 365 aboneliğinizdeki korumayı artırmanıza yardımcı olur. Bu öneriler, hukuk büroları ve sağlık klinikleri gibi güvenlik ihtiyacı artan kuruluşlar için uygundur.

Başlamadan önce Office 365 Güvenli Puanınızı kontrol edin. Office 365 Secure Score, düzenli etkinliklerinize ve güvenlik ayarlarınıza göre Office 365 kuruluşunuzun güvenliğini analiz eder ve bir puan atar. Geçerli puanınızı dikkate alarak başlayın. Puanınızı artırmak için bu makalede önerilen eylemleri tamamlayın. Amaç maksimum puanı elde etmek değil, çevrenizi korumak için kullanıcılarınızın üretkenliğini olumsuz etkilemeyen fırsatların farkında olmaktır. 

Daha fazla bilgi için [Microsoft Secure Score'a](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)bakın.

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Postadaki kötü amaçlı yazılıma karşı koruma düzeyini yükseltin

Office 365 veya Microsoft 365 ortamınız kötü amaçlı yazılıma karşı koruma içerir. Kötü amaçlı yazılımlar için yaygın olarak kullanılan dosya türleri ile ekleri engelleyerek bu korumayı artırabilirsiniz. E-postada kötü amaçlı yazılımların korunmasını artırmak için:
  
1. Yönetici [https://protection.office.com](https://protection.office.com) hesap kimlik bilgilerinizle oturum açın. 
    
2. Office 365 Güvenlik &amp; Uyumluluk Merkezi'nde, sol navigasyon bölmesinde, **Tehdit yönetimi**altında, **Politika** \> **Anti-Malware**seçin.
    
3. Şirket genelinde ki bu ilkeyi yeniden yapmak için varsayılan ilkeyi çift tıklatın.
    
4. **Ayarlar'ı**seçin.
    
5. **Ortak Ek Türleri Filtresi**altında, **Açık'ı**seçin. Engellenen dosya türleri bu denetimin hemen altındaki pencerede listelenir. Bu dosya türlerini eklediğinizden emin olun:
   - ade, adp, ani, bas, yarasa, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, iş, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, ws, p  <br/> 
   
   Gerekirse, daha sonra dosya türleri ekleyebilir veya silebilirsiniz.
    
6. **Kaydet'i seçin.**
    
Daha fazla bilgi için [bkz.](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409)
  
## <a name="protect-against-ransomware"></a>Fidye yazılımlarına karşı koruyun

Ransomware dosyaları şifreleyerek veya bilgisayar ekranlarını kilitleyerek verilere erişimi kısıtlar. Daha sonra verilere erişim karşılığında genellikle Bitcoin gibi kripto para birimleri şeklinde "fidye" isteyerek kurbanlardan para koparmaya çalışır. 
  
Ransomware karşı korumak için, yaygın ransomware için kullanılan dosya uzantıları engellemek için bir veya daha fazla posta akışı kuralları oluşturun. (Bu [kuralları, posta adımında kötü amaçlı yazılıma karşı koruma düzeyini yükseltmek için eklediniz.)](#raise-the-level-of-protection-against-malware-in-mail) Ayrıca, bu ekleri e-posta yla alan kullanıcıları da uyarabilirsiniz.

Önceki adımda engellediğiniz dosyalara ek olarak, makroları içeren Office dosya eklerini açmadan önce kullanıcıları uyarmak için bir kural oluşturmak iyi bir uygulamadır. Ransomware makrolar içinde gizli olabilir, bu yüzden onlar bilmiyorum insanlardan bu dosyaları açmak için kullanıcıları uyarmak.

Posta aktarım kuralı oluşturmak için:
  
1. Yönetici <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>merkezine gidin ve **Yönetici merkezleri** \> **Exchange'i**seçin.
    
2. Posta **akışı** **kategorisinde, kuralları**seçin.
    
3. Seçin **+** ve sonra **yeni bir kural oluştur'u**seçin.
    
4. Tüm seçenekleri görmek için iletişim kutusunun altındaki **diğer seçenekleri** seçin. 
    
5. Kural için aşağıdaki tablodaki ayarları uygulayın. Değiştirmek istemediğiniz sürece, ayarların geri kalanı için varsayılan değerleri kullanın.
    
6. **Kaydet**'i seçin.
    
|**Ayar**|**Office dosyalarının eklerini açmadan önce kullanıcıları uyarma**||
|:-----|:-----|:-----|
|Name  <br/> |Anti-ransomware kural: kullanıcıları uyarmak  <br/>  |
|Bu kuralı uygulayın eğer . . .  <br/> |Herhangi bir eki . . . dosya uzantısı eşleşir. . .  <br/> |
|Sözcükleri veya tümcecikleri belirtin  <br/> |Bu dosya türlerini ekleyin:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Aşağıdakileri yapın. . .  <br/> |Alıcıya bir ileti bildirme  <br/> |
|İleti metni sağlama  <br/> |Kötü amaçlı kodiçeren makrolar içerebileceğinden tanımadığınız kişilerden bu tür dosyaları açmayın.  <br/> |
   
Daha fazla bilgi için bkz.
  
- [Nasıl ransomware ile başa çıkmak için](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [OneDrive'ınızı Geri Yükleme](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-posta için otomatik yönlendirmeyi durdurma

Bir kullanıcının posta kutusuna erişen bilgisayar korsanları, posta kutusunu otomatik olarak e-posta iletecek şekilde ayarlayarak postaları çalabilir. Bu kullanıcının farkındalığı olmadan bile gerçekleşebilir. Bunun olmasını önlemek için bir posta akışı kuralını yapılandırın. 
  
Posta aktarım kuralı oluşturmak için [bu kısa videoyu](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) izleyin veya aşağıdaki adımları izleyin:
  
1. Microsoft 365 yönetici merkezinde, **Yönetici merkezleri** \> **Exchange'i**seçin.
    
2. Posta **akışı** **kategorisinde, kuralları**seçin.
    
3. Seçin **+** ve sonra **yeni bir kural oluştur'u**seçin.
    
4. Tüm seçenekleri görmek için iletişim kutusunun altındaki **diğer seçenekleri** seçin. 
    
5. Aşağıdaki tablodaki ayarları uygulayın. Değiştirmek istemediğiniz sürece, ayarların geri kalanı için varsayılan değerleri kullanın.
    
6. **Kaydet**'i seçin.
    
|**Ayar**|**Office dosyalarının eklerini açmadan önce kullanıcıları uyarma**|
|:-----|:-----|
|Name  <br/> |E-postanın harici etki alanına otomatik olarak iletilmesinin engellenmesi  <br/> |
|Bu kuralı uygulayın eğer ...  <br/> |Gönderen. . . harici/dahilidir. . . Kuruluş içinde  <br/> |
|Koşul ekleme  <br/> |İleti özellikleri . . . ileti türünü ekleyin. . . Otomatik iletme  <br/> |
|Aşağıdaki leri yapın ...  <br/> |İletiyi engelleme. . . iletiyi reddedin ve bir açıklama ekleyin.  <br/> |
|İleti metni sağlama  <br/> |Bu kuruluş dışında otomatik yönlendirme e-postagüvenlik nedenleriyle engellenir.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>E-postanızı kimlik avı saldırılarına karşı koruyun

Office 365 veya Microsoft 365 ortamınız için bir veya daha fazla özel etki alanı yapılandırmışsanız, hedeflenen kimlik avı önleme koruması yapılandırabilirsiniz. Office 365 Gelişmiş Tehdit Koruması'nın bir parçası olan ATP kimlik avı önleme koruması, kuruluşunuzun kötü amaçlı kimliğe bürünme tabanlı kimlik avı saldırılarından ve diğer kimlik avı saldırılarından korunmasına yardımcı olabilir. Özel bir etki alanı yapılandırmadıysanız, bunu yapmanız gerekmez.
  
En önemli kullanıcılarınızı ve özel etki alanınızı korumak için bir ilke oluşturarak bu korumaya başlamanızı öneririz. 

Bir ATP kimlik avı önleme ilkesi oluşturmak için [bu kısa eğitim videosunu](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)izleyin veya aşağıdaki adımları tamamlayın:
  
1. [https://protection.office.com](https://protection.office.com) adresine gidin. 
    
2. Office 365 Güvenlik &amp; Uyumluluk Merkezi'nde, sol navigasyon bölmesinde, **Tehdit yönetimi**altında, **İlke'yi**seçin.
    
3. **İlke** **sayfasında, ATP anti-phishing'i**seçin.
    
4. Kimlik **avı önleme** sayfasında + **Oluştur'u**seçin. Bir sihirbaz, kimlik avı önleme ilkenizi tanımlamada size gereken adımları başlatıyor.
    
5. Aşağıdaki tabloda önerilen ilkenizin adını, açıklamasını ve ayarlarını belirtin. Daha fazla bilgi için [ATP kimlik avı önleme ilkesi seçenekleri hakkında bilgi](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options)edinin. 
    
6. Ayarlarınızı inceledikten sonra, uygun şekilde **bu ilkeyi oluştur** veya **Kaydet'i**seçin.
    

|**Ayar veya seçenek**<br/>|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Etki alanı ve en değerli kampanya personeli  <br/> |
|Açıklama  <br/> |En önemli personelin ve etki alanımızın taklit edilmediğinden emin olun.  <br/> |
|Korumak için kullanıcı ekleme  <br/> |Select **+ Bir koşul ekle, alıcı**. Kullanıcı adlarını yazın veya adayın, kampanya yöneticisinin ve diğer önemli personelin e-posta adresini girin. Kimliğe bürünmekten korumak istediğiniz en fazla 20 dahili ve harici adres ekleyebilirsiniz.  <br/> |
|Korumak için etki alanları ekleme  <br/> |Select **+ Bir koşul ekle, alıcı etki alanı**. Tanımladıysanız, Microsoft 365 aboneliğinizle ilişkili özel etki alanını girin. Birden fazla etki alanı girebilirsiniz.  <br/> |
|Eylemleri seçme  <br/> |E-posta kimliği takılmış bir kullanıcı tarafından gönderiliyorsa: **İletiyi başka bir e-posta adresine yönlendirmeyi**seçin ve ardından güvenlik yöneticisinin e-posta adresini yazın; örneğin, *Alice<span><span>@contoso.com*. E-posta, kimliği taklit edilmiş bir etki alanı tarafından gönderiliyorsa: **Karantina iletisini**seçin.  <br/> |
|Posta kutusu zekası  <br/> |Varsayılan olarak, yeni bir kimlik avı önleme ilkesi oluşturduğunuzda posta kutusu zekası seçilir. En iyi sonuçlar için bu ayarı **açık** bırakın.  <br/> |
|Güvenilir gönderenler ve etki alanları ekleme  <br/> |Buraya kendi etki alanınızı veya diğer güvenilen etki alanlarını ekleyebilirsiniz.  <br/> |
|Uygulanan  <br/> |**Alıcı etki alanı seçin.** **Bunların herhangi birinin**altında, **Seç'i**seçin. Seçin **+ Ekle**. Etki alanının adının yanındaki onay kutusunu seçin( örneğin, *contoso.<span> com <span>*, listede ve sonra **Ekle'yi**seçin. **Bitti'yi**seçin.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>ATP Güvenli Ekleri ile kötü amaçlı eklere ve dosyalara karşı koruma

Kişiler belgeler, sunular, elektronik tablolar ve daha fazlası gibi ekleri düzenli olarak gönderir, alır ve paylaşır. Bir eki sadece bir e-posta iletisine bakarak güvenli veya kötü niyetli olup olmadığını söylemek her zaman kolay değildir. Office 365 Gelişmiş Tehdit Koruması ATP Güvenli Eki koruması içerir, ancak bu koruma varsayılan olarak açık değildir. Bu korumayı kullanmaya başlamak için yeni bir kural oluşturmanızı öneririz. Bu koruma SharePoint, OneDrive ve Microsoft Teams'deki dosyaları genişletir.
  
BIR ATP güvenli eki ilkesi oluşturmak [için, bu kısa videoyu](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)izleyin veya aşağıdaki adımları tamamlayın:
  
1. Yönetici [https://protection.office.com](https://protection.office.com)hesabınıza gidin ve oturum açın. 
    
2. Office 365 Güvenlik &amp; Uyumluluk Merkezi'nde, sol navigasyon bölmesinde, **Tehdit yönetimi**altında, **İlke'yi**seçin.
    
3. İlke **sayfasında, ATP güvenli ekleri**seçin.
    
4. Güvenli ekler sayfasında, **SharePoint, OneDrive ve Microsoft Teams** onay kutusunu açmak için ATP'yi seçerek bu korumayı geniş ölçüde uygulayın. 
    
5. Yeni **+** bir ilke oluşturmak için seçin. 
    
6. Aşağıdaki tablodaki ayarları uygulayın. 
    
7. Ayarlarınızı inceledikten sonra, uygun şekilde **bu ilkeyi oluştur** veya **Kaydet'i**seçin.
    

|**Ayar veya seçenek**|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Algılanan kötü amaçlı yazılımla mevcut ve gelecekteki e-postaları engelleyin.  <br/> |
|Açıklama  <br/> |Algılanan kötü amaçlı yazılımla mevcut ve gelecekteki e-postaları ve ekleri engelleyin.  <br/> |
|Ekleri bilinmeyen kötü amaçlı yazılım yanıtını kaydetme  <br/> |Blok 'u seçin **- Algılanan kötü amaçlı yazılımla mevcut ve gelecekteki e-postaları ve ekleri engelleyin.**  <br/> |
|Algılama da eki yönlendirme  <br/> |Yeniden yönlendirmeyi etkinleştirin (bu kutuyu seçin) Karantina için yönetici hesabını veya posta kutusu kurulumünü girin.          Ekler için kötü amaçlı yazılım taraması zaman ları doluyorsa veya hata oluşuyorsa yukarıdaki seçimi uygulayın (bu kutuyu seçin).  <br/> |
|Uygulanan  <br/> |Alıcı etki alanı. . . etki alanınızı seçin.  <br/> |
   
Daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>ATP Güvenli Bağlantıları ile kimlik avı saldırılarına karşı koruma

Bilgisayar korsanları bazen kötü amaçlı web sitelerini e-posta veya diğer dosyalardaki bağlantılarda gizler. Office 365 Gelişmiş Tehdit Koruması'nın bir parçası olan Office 365 ATP Güvenli Bağlantılar (ATP Güvenli Bağlantılar), e-posta iletilerinde ve Office belgelerinde web adreslerinin (URL'ler) tıklattıka doğrulanmasını sağlayarak kuruluşunuzun korunmasına yardımcı olabilir. Koruma, ATP Güvenli Bağlantılar ilkeleri yle tanımlanır.
  
Aşağıdakileri yapmanızı öneririz:
  
- Korumayı artırmak için varsayılan ilkeyi değiştirin.
    
- Etki alanınızdaki tüm alıcılara yönelik yeni bir ilke ekleyin.
    
ATP Güvenli Bağlantılar'ı kurmak için [bu kısa eğitim videosunu](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)izleyin veya aşağıdaki adımları tamamlayın:
  
1. Yönetici [https://protection.office.com](https://protection.office.com)hesabınıza gidin ve oturum açın. 
    
2. Office 365 Güvenlik &amp; Uyumluluk Merkezi'nde, sol navigasyon bölmesinde, **Tehdit yönetimi**altında, **İlke'yi**seçin.
    
3. İlke **sayfasında, ATP Güvenli Bağlantılar'ı**seçin.
    
Varsayılan ilkeyi değiştirmek için:
  
1. Güvenli bağlantılar sayfasında, **tüm kuruluş için geçerli olan İlkeler**altında **Varsayılan** ilkeyi seçin. 
    
2. **E-posta dışındaki içeriğe uygulanan Ayarlar**altında, **iOS ve Android için Office, Office 365 ProPlus'ı**seçin.
    
3. **Kaydet**'i seçin. 
    
Etki alanınızdaki tüm alıcılara yönelik yeni bir ilke oluşturmak için:
  
1. Güvenli bağlantılar sayfasında, **tüm kuruluş için geçerli olan** **+** İlkeler altında, yeni bir ilke oluşturmak için seçin. 
    
2. Aşağıdaki tabloda listelenen ayarları uygulayın.
    
3. **Kaydet**'i seçin. 

|**Ayar veya seçenek**|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Etki alanında tüm alıcılar için güvenli bağlantılar ilkesi  <br/> |
|İletilerde bilinmeyen kötü amaçlı URL'ler için eylemi seçme  <br/> |Select **On - URL'ler, kullanıcı bağlantıyı tıklattığında bilinen kötü amaçlı bağlantılar listesiyle karşılaştırılır ve kontrol edilir.**  <br/> |
|İndirilebilir içeriği tetmek için Güvenli Ekler'i kullanma  <br/> |Bu kutuyu seçin.  <br/> |
|Uygulanan  <br/> |Alıcı etki alanı. . . etki alanınızı seçin.  <br/> |
   
Daha fazla bilgi için Bkz. [Office 365 ATP güvenli bağlantıları.](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)

## <a name="go-to-intune-admin-center"></a>Intune yönetici merkezine git

1. [Azure portalında](https://portal.azure.com/)oturum açın.

2. **Tüm hizmetleri** seçin ve Arama **Kutusu'nda** *Intune* yazın.

3. Sonuçlar göründükten sonra, microsoft **intune'un** yanındaki başlatı seçerek sık kullanılan ve daha sonra bulması kolay hale getirin.

Yönetici merkezine ek olarak, kuruluşunuzun aygıtlarını kaydetmek ve yönetmek için Intune'u kullanabilirsiniz. Daha fazla bilgi için Windows [aygıtları için kayıt yöntemine göre Yetenekler](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) ve [Intune tarafından yönetilen aygıtlar için Kayıt seçeneklerine](https://docs.microsoft.com/intune/enrollment-options)bakın.
