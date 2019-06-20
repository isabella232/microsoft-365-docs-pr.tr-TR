---
title: Microsoft 365 iş için tehdit koruma artırın
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
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş tehdit koruma sisteminizi kurma ve hassas verilerinizi korumak.
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086413"
---
# <a name="increase-threat-protection"></a>Tehdit koruması artırın

Bu makalede, kimlik avı, kötü amaçlı yazılımlara ve diğer tehditlere karşı korumak için Microsoft 365 aboneliğinizi korumayı artırmak yardımcı olur. Bu öneriler, kuruluşlar için uygun olan hukuk ofisleri ve Klinikler sağlık gibi güvenlik gereksinimi artmaktadır.

Başlamadan önce Office 365 güvenli puanını denetleyin. Office 365 puan güvenli Office 365 kuruluşunuzun güvenlik düzenli etkinlikler ve güvenlik ayarlarına göre çözümler ve bir puan verir. Puanınız geçerli not alarak başlayın. Bu makalede önerilen eylemleri yaptıktan puanınız artar. Amaç en yüksek skoru elde değil ancak kullanıcılarınız için verimliliği olumsuz yönde etkilemez ortamınızı korumak için fırsatlar haberdar olmasını sağlamaktır. 

Daha fazla bilgi için bkz: [Microsoft Güvenli puanı](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Postada zararlı yazılımlara karşı koruma düzeyini Yükselt

Office 365 veya Microsoft 365 ortamınızı kötü amaçlı yazılımlara karşı koruma içerir ancak bu koruma, kötü amaçlı yazılım için yaygın olarak kullanılan dosya türlerini engelleme eklerle tarafından artırabilirsiniz. E-postadaki zararlı yazılımlara karşı koruma artırmak için:
  
1. Git [https://protection.office.com](https://protection.office.com) ve, yönetici hesabı kimlik bilgileri ile oturum açın. 
    
2. Office 365 güvenlik &amp; Uyumluluk Merkezi, sol gezinti bölmesinde, **tehdit Yönetimi**, seçim **İlkesi** \> **Zararlı yazılımlara karşı**.
    
3. Bu şirket genelinde ilkesini düzenlemek için varsayılan ilkeyi çift tıklatın.
    
4. **Ayarlar**' ı tıklatın.
    
5. ** **Ortak ek türleri süzgeç**seçin.** Engellenen dosya türleri penceresinde doğrudan bu denetim altında listelenir.  Bu dosya türü eklemek emin olun:
   - ade, adp, anı, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, INF, bileşenleri, ISS, işi, js, jse, lnk, mda, mdb, mde, mdz, msc, MSI, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, PIF  <br/> Gerekirse daha sonra dosya türlerini silmek ya da ekleyin.
    
6. ' I **Kaydet.**
    
Daha fazla bilgi için bkz: [zararlı yazılımlara karşı koruma](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ransomware karşı koruma

Dosyaları şifreleme veya bilgisayar ekranları kilitleme Ransomware verilere erişimi kısıtlar. Onu daha sonra "ransom için" isteyerek kurbanların para extort genellikle verilere erişim karşılığında gibi Bitcoin, cryptocurrencies biçiminde çalışır. 
  
Bir veya daha fazla posta akışı kuralları (bunlar [postada zararlı yazılımlara karşı koruma düzeyini yükseltmek](#raise-the-level-of-protection-against-malware-in-mail) adımda eklenen) ransomware için yaygın olarak kullanılan dosya uzantılarını engelleyecek veya bunlar alacak kullanıcıları uyarmak oluşturarak ransomware karşı koruyabilirsiniz. e-posta ekleri.

Önceki adımda engellenen dosyaların yanı sıra, makroları içeren Office dosya eklerini açmadan önce kullanıcıları uyarmak için bir kural oluşturmak için yararlı da olur. Biz bu dosyaları biliyor musunuz kişilerden açmamak üzere kullanıcıları uyarmak böylece Ransomware makrolar gizlenebilir.

Posta Aktarım kuralı oluşturmak için:
  
1. Gidin Yönetim Merkezi'nde <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ve **Yönetim Merkezleri** seçin \> **Exchange**.
    
2. **Posta akışı** kategorisinde **kurallar**' ı tıklatın.
    
3. ' I **+**, **Yeni bir kural oluştur**' ı tıklatın.
    
4. Seçenekler kümesini görmek için **diğer seçenekler** iletişim kutusunun alt'ı tıklatın. 
    
5. Ayarlar aşağıdaki tabloda kural uygulanır. Bunlar değiştirmek istemediğiniz sürece varsayılan ayarları geri kalanı bırakın.
    
6. **Kaydet**'i tıklatın.
    
|**Ayar**|**Office dosya eklerini açmadan önce kullanıcıları uyarın.**||
|:-----|:-----|:-----|
|Name  <br/> |Anti-ransomware kural: kullanıcıları uyarın  <br/>  |
|Bu kural uygulayın. . .  <br/> |Herhangi bir ek. . . Dosya uzantısı ile eşleşir. . .  <br/> |
|Sözcükleri veya tümceleri belirtin  <br/> |Bu dosya türleri ekleyin:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Aşağıdakileri yapın. . .  <br/> |Alıcı bir iletiyle bildirmek  <br/> |
|İleti metni sağlamak  <br/> |Kötü amaçlı kod içeren makrolar içerebileceğinden tanımadığınız kişilerden gelen bu tür dosyaları açmayın.  <br/> |
   
Daha fazla bilgi için bkz.
  
- [Ransomware ile başa çıkma](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [OneDrive, geri yükleme](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Durdurmak için e-posta otomatik iletme

Bir kullanıcının posta kutusuna erişim saldırganlar posta posta kutusu otomatik olarak e-posta iletmek için ayarlayarak çalınacak. Bu kullanıcının tanınmasını bile ortaya çıkabilir. Bu posta akışı kural yapılandırılarak oluşmasını engelleyebilir. 
  
Posta Aktarım kuralı oluşturmak için [Bu kısa videoyu](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) izleyin veya şu adımları izleyin:
  
1. Microsoft 365 Yönetim Merkezi'nde **Yönetim Merkezleri** ' ı \> **Exchange**.
    
2. **Posta akışı** kategorisinde **kurallar**' ı tıklatın.
    
3. ' I **+**, **Yeni bir kural oluştur**' ı tıklatın.
    
4. Seçenekler kümesini görmek için **diğer seçenekler** iletişim kutusunun alt'ı tıklatın. 
    
5. Aşağıdaki tabloda ayarlar uygulanır. Bunlar değiştirmek istemediğiniz sürece varsayılan ayarları geri kalanı bırakın.
    
6. **Kaydet**'i tıklatın.
    
|**Ayar**|**Office dosya eklerini açmadan önce kullanıcıları uyarın.**|
|:-----|:-----|
|Name  <br/> |Dış etki alanlarına e-posta otomatik iletilmesini engellemek  <br/> |
|Bu kural, Uygula...  <br/> |Gönderen. . . Dış/iç olduğunu. . . Kuruluş içinde  <br/> |
|Koşul Ekle  <br/> |İleti özellikleri. . . ileti türünü içerir. . . Otomatik iletme  <br/> |
|Aşağıdakileri yapın...  <br/> |İletiyi engeller. . . iletiyi reddeder ve bir açıklama içerir.  <br/> |
|İleti metni sağlamak  <br/> |Bu kuruluş dışından otomatik iletme e-posta güvenlik nedeniyle engellenir.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>E-posta adresiniz sızdırma saldırılarına karşı koruma

Office 365 veya Microsoft 365 ortamınız için bir veya daha fazla özel etki alanı yapılandırmışsanız, hedeflenen anti-phishing koruması yapılandırabilirsiniz. ATP Sızdırma Koruması, Office 365 Gelişmiş tehdit koruması, parçası, kuruluşunuzun amaçlı kimliğe bürünme tabanlı kimlik avı saldırılarından ve diğer kimlik avı saldırılarından korunmasına yardımcı olabilir. Bir özel etki alanı yapılandırıldığında, bunu yapmanız gerekmez.
  
Kullanıcılarınızın en önemli ve özel etki alanınızı korumak için bir ilkesi oluşturarak bu koruma ile başlamak öneririz. 

  
Bir ATP anti-phishing ilkesi oluşturmak için [Bu kısa eğitim video](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)izlemek veya aşağıdaki adımları izleyin:
  
1. [https://protection.office.com](https://protection.office.com) adresine gidin. 
    
2. Office 365 güvenlik &amp; Uyumluluk Merkezi, sol gezinti bölmesinde, **tehdit Yönetimi**, seçim **İlkesi**.
    
3. **ATP anti-phishing** **Policy** sayfasında seçin.
    
4. **Anti-phishing** sayfasında **+ oluşturma**seçeneğini belirleyin. Size anti-phishing ilkeniz tanımlama yoluyla adım adım yol gösteren bir sihirbaz başlatır.
    
5. Ad, açıklama ve grafikte önerildiği gibi ilke ayarlarını belirtin. [ATP anti-phishing ilkesi seçenekleri hakkında bilgi edinin](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) daha fazla ayrıntı için bkz. 
    
6. Ayarlarınızı gözden geçirdikten sonra **Bu ilke oluşturma** veya **kaydetme**uygun olanını seçin.
    

|**Ayar veya seçenek**<br/>|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Etki alanı ve en değerli kampanya personeli  <br/> |
|Açıklama  <br/> |Personel ve bizim etki alanı olmayan özellikleri alınan en önemli emin olun.  <br/> |
|Korumak için kullanıcı ekleme  <br/> |**+ Alıcı bir koşul Ekle**seçeneğini belirleyin. Kullanıcı adlarını yazın veya aday, kampanya Yöneticisi ve diğer önemli Personel e-posta adresini girin. Kimliğe bürünme korumak istediğiniz en fazla 20 iç ve dış adresler de ekleyebilirsiniz.  <br/> |
|Korumak için etki alanları ekleme  <br/> |**+ Koşulu, alıcı etki alanına Ekle**seçeneğini belirleyin. Bir tane tanımladıysanız Microsoft 365 aboneliğinizle ilgili özel etki alanını girin. Birden fazla etki alanına girebilirsiniz.  <br/> |
|Eylemleri seçin  <br/> |Kimliğine bürünülen bir kullanıcı tarafından e-posta gönderirse: **ileti başka bir e-posta adresine yönlendir**' i seçin ve sonra güvenlik yöneticisinin; e-posta adresini yazın Örneğin, *Gamze<span><span>@contoso.com*.          Kimliğine bürünülen bir etki alanı tarafından e-posta gönderirse: **Karantina iletiyi**seçin.  <br/> |
|Posta kutusu gösterimi  <br/> |Yeni bir kimlik avından koruma ilkesi oluşturduğunuzda, varsayılan olarak, posta kutusu akıl seçilir. **Bu ayarı en iyi sonuçları almak için** bırakın.  <br/> |
|Güvenilir Gönderenler ve etki alanları ekleme  <br/> |Burada, kendi etki alanı veya diğer güvenilen etki alanları ekleyebilirsiniz.  <br/> |
|Uygulanan  <br/> |**Alıcının etki alanı**seçin. **Bunların hiçbirini**altında **Seç**seçin. **+ Ekle**seçeneğini belirleyin. Örneğin, *contoso etki alanı adının yanındaki onay kutusunu seçin.<span> <span>com*, listede tıklatın ve sonra seçin **Ekle**. **Bitti**' yi seçin.  <br/> |
   
Daha fazla bilgi için bkz: [Office 365 KM anti-phishing ilkelerini kurun](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Koruma amaçlı ekleri ve dosyaları ile ATP güvenli ekler

İnsanlar düzenli olarak gönderme, alma ve belgeleri, sunumları, elektronik tablolar ve ekleri paylaşın. Her zaman bir ek e-posta iletisine bakarak güvenli veya kötü amaçlı olup olmadığını söylemek kolay değildir. Gelişmiş tehdit koruması Office 365 KM güvenli ek koruma içerir, ancak bu Koruması varsayılan olarak açıktır. Bu koruma kullanmaya başlamak için yeni bir kural oluşturmanızı öneririz. Bu koruma, Microsoft Teams, OneDrive ve SharePoint dosyaları için genişletir.
  
Bir ATP güvenli ek ilke oluşturmak için [Bu kısa videoyu](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)izleyin veya aşağıdaki adımları izleyin:
  
1. Git [https://protection.office.com](https://protection.office.com) ve yönetici hesabınız ile oturum açın. 
    
2. Office 365 güvenlik &amp; Uyumluluk Merkezi, sol gezinti bölmesinde, **tehdit Yönetimi**, seçim **İlkesi**.
    
3. **ATP güvenli ekler**Policy sayfasında seçin.
    
4. Güvenli ekler sayfasında, **SharePoint, OneDrive, ve Microsoft ekipleri KM Aç** onay kutusunu seçerek bu koruma geniş ölçüde geçerlidir. 
    
5. Seçin **+** yeni bir ilke oluşturmak için. 
    
6. Aşağıdaki tabloda ayarlar uygulanır. 
    
7. Ayarlarınızı gözden geçirdikten sonra **Bu ilke oluşturma** veya **kaydetme**uygun olanını seçin.
    

|**Ayar veya seçenek**|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Algılanan kötü amaçlı yazılım içeren geçerli ve gelecekteki e-postaları engelleyin.  <br/> |
|Açıklama  <br/> |Güncel ve gelecek e-postalar ve ekleri ile Algılanan kötü amaçlı yazılımın engelleyin.  <br/> |
|Bilinmeyen zararlı yazılımlara karşı yanıt Ekleri Kaydet  <br/> |**Blok - güncel ve gelecek e-postalar ve ekleri ile Algılanan kötü amaçlı yazılımın engelleme**seçin.  <br/> |
|Ek algılama üzerinde yönlendir  <br/> |Yeniden yönlendirmeyi etkinleştir (Bu kutuyu seçin) karantina için yönetici hesabını veya posta kutusu ayarı girin.          Zararlı yazılımlara karşı tarama ekler için zaman aşımına uğradı ya da hata oluşur yukarıdaki seçim uygulanır (Bu kutusunu işaretleyin).  <br/> |
|Uygulanan  <br/> |Alıcı etki alanıdır. . . etki alanınızı seçin.  <br/> |
   
Daha fazla bilgi için bkz: [Office 365 KM anti-phishing ilkelerini kurun](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>ATP güvenli bağlantıları olan kimlik avı saldırılarına karşı koruma

Bilgisayar korsanları, bazen kötü amaçlı Web sitelerine bağlantılar'e-posta veya diğer dosyaları gizleyin. Office 365 KM güvenli bağlantılar (ATP güvenli bağlantılar), Office 365 Gelişmiş tehdit koruması, parçası, kuruluşunuzun web adresleri (URL'ler) tıklatın zaman doğrulanmasını sağlayarak e-posta iletileri ve Office belgelerine korunmasına yardımcı olabilir. Koruma ATP güvenli bağlantılar ilkeleri tanımlanır.
  
Aşağıdakileri yapmanızı öneririz:
  
- Koruma artırmak için varsayılan ilkeyi değiştirmek.
    
- Etki alanınızdaki tüm alıcılara hedefleyen yeni bir ilke ekleyin.
    
ATP güvenli bağlantıları ayarlarken [Bu kısa eğitim video](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)izlemek veya aşağıdaki adımları izleyin:
  
1. Git [https://protection.office.com](https://protection.office.com) ve yönetici hesabınız ile oturum açın. 
    
2. Office 365 güvenlik &amp; Uyumluluk Merkezi, sol gezinti bölmesinde, **tehdit Yönetimi**, seçim **İlkesi**.
    
3. **ATP güvenli bağlantılar**Policy sayfasında seçin.
    
Varsayılan ilkeyi değiştirmek için:
  
1. Güvenli bağlantılar sayfasında, **kuruluşun tamamı için geçerli ilkeleri**, **Varsayılan** ilkesi seçin. 
    
2. **E-posta dışında içerik için geçerli olan ayarları**altında **Office 365 ProPlus, Office IOS ve Android için**seçin.
    
3. **Kaydet**'i tıklatın. 
    
Etki alanınızdaki tüm alıcılara hedefleyen yeni bir ilke oluşturmak için:
  
1. Güvenli bağlantılar sayfası, **kuruluşun tamamı için geçerli ilkeleri**altında tıklatın **+** yeni bir ilke oluşturmak için. 
    
2. Aşağıdaki tabloda listelenen ayarları uygulanır.
    
3. **Kaydet**'i tıklatın. 

|**Ayar veya seçenek**|**Önerilen ayar** <br/>|
|:-----|:-----|
|Name  <br/> |Güvenli bağlantı ilkesi etki alanındaki tüm alıcılar için  <br/> |
|Bilinmeyen zararlı URL'leri için eylem iletileri seçin  <br/> |**-URL'leri yeniden yazan ve kullanıcı bağlantısını tıklattığında bilinen kötü amaçlı bağlantıların listesini karşılaştırılarak**seçin.  <br/> |
|Karşıdan yüklenebilir içeriği taramak için güvenli ekler  <br/> |Bu kutuyu seçin.  <br/> |
|Uygulanan  <br/> |Alıcı etki alanıdır. . . etki alanınızı seçin.  <br/> |
   
Daha fazla bilgi için [Office 365 KM güvenli bağlantılara](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)bakın.

## <a name="go-to-intune-admin-center"></a>Intune Yönetim Merkezine gidin

1. [Azure portal](https://portal.azure.com/)oturum açın.

2. **Arama kutusu** *Intune* **tüm hizmetleri** ve türünü seçin.

3. Sonuçları görüntüledikten sonra sık yapmak için **Microsoft Intune** için İleri ve kolayca bulabilmek için Başlat'ı tıklatın.

Yönetim Merkezi yanı sıra, kaydolmak ve kuruluşunuzun aygıtları yönetmek için Intune kullanabilirsiniz. Daha fazla bilgi için bkz: [Windows aygıtları için kayıt yöntemi tarafından yetenekleri](https://docs.microsoft.com/intune/enrollment-method-capabs) ve [Intune tarafından yönetilen aygıtlar için kayıt seçenekleri](https://docs.microsoft.com/intune/enrollment-options).
