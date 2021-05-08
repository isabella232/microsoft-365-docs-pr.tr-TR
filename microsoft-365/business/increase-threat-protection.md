---
title: kurumsal iş için Microsoft 365 korumayı artırma
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Microsoft Defender'ı güvenlik için Office 365 kimlik avına, kötü amaçlı yazılıma ve diğer tehditlere karşı hassas verileri korur.
ms.openlocfilehash: 4b5142efbf4392f017cd9b96f6a9c36ef2000bb7
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245154"
---
# <a name="increase-threat-protection"></a>Tehdit korumasını artırma

Bu makale, kimlik avına, kötü amaçlı yazılıma Microsoft 365 diğer tehditlere karşı korumak üzere e-posta aboneliğinizin korumasını artırmanıza yardımcı olur. Bu öneriler, hukuk daireleri ve sağlık hizmetleri gibi güvenlik ihtiyacı daha yüksek olan kuruluşlar için uygundur.

Başlamadan önce Güvenli Puanınızı Office 365 kontrol edin. Office 365 Güvenli Puan, normal etkinliklerinize ve güvenlik ayarlarınıza göre kuruluş güvenliğini analiz eder ve bir puan atar. Geçerli puanınızı not alarak başlama. Puanınızı artırmak için bu makalede önerilen eylemleri gerçekleştirin. Amaç maksimum puanı elde etmek değil, kullanıcılarınız için üretkenliği olumsuz etkilemeyen ortamınızı koruma fırsatlarını da takip etmektir.

Daha fazla bilgi için [bkz. Microsoft Güvenli Puanı](../security/defender/microsoft-secure-score.md).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Postada kötü amaçlı yazılıma karşı koruma düzeyini yükseltme

Sizin Office 365 veya Microsoft 365 ortamınız kötü amaçlı yazılıma karşı koruma içerir. Kötü amaçlı yazılımda yaygın olarak kullanılan dosya türlerine sahip ekleri engelleyerek bu korumayı artırabilirsiniz. E-postada kötü amaçlı yazılıma karşı korumayı artırmak için:

1. Yönetici [https://protection.office.com](https://protection.office.com) hesabı kimlik bilgilerinize gidin ve bu kimlik bilgileriyle oturum açın.

2. Güvenlik Uyumluluk Merkezi'nin sol gezinti bölmesinde, Tehdit yönetimi altında, Kötü Amaçlı &amp; Yazılımdan Koruma   \> **İlkesi'ni seçin.**

3. Şirket çapında bu ilkeyi düzenlemek için varsayılan ilkeye çift tıklayın.

4. **Ayarlar.**

5. Ortak **Ek Türleri Filtresi'nin altında** Aç'ı **seçin.** Engellenmiş dosya türleri, bu denetimin hemen altındaki pencerede listelenir. Şu dosya türlerini de eklemek istediğinizden emin olun:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Gerekirse, daha sonra dosya türlerini ekleyebilir veya silebilirsiniz.

6. **Kaydet'i seçin.**

Daha fazla bilgi için [bkz. EOP'de kötü amaçlı yazılımdan koruma.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Fidye yazılımlarına karşı koruma

Fidye yazılımları, dosyaları şifreleyerek veya bilgisayar ekranlarını kilitleyerek verilere erişimi kısıtlar. Ardından, veriye erişim için genellikle Bitcoin gibi şifreleme şifrelemeleri biçimine sahip "bilgi" talep eden ve ona yardım etmek isteyen bir kaynağın paralarını ödemeye çalışır.

Fidye yazılımlarına karşı korunmak için, fidye yazılımları için yaygın olarak kullanılan dosya uzantılarını engellemek için bir veya daha fazla posta akış kuralı oluşturun. (Bu kuralları posta adımlarında [kötü amaçlı yazılıma karşı koruma düzeyini yükseltmeye eklediniz.)](#raise-the-level-of-protection-against-malware-in-mail) Bu ekleri e-postayla alan kullanıcıları da uyarabilirsiniz.

Önceki adımda engelle dosyalara ek olarak, makro içeren bir dosya eklerini açmadan önce kullanıcıları Office bir kural oluşturmak iyi bir uygulamadır. Fidye yazılımları makroların içine gizlenmiş olabilir, bu nedenle kullanıcıları bu dosyaları kimsenin görene kadar açmamalarını uyarın.

Posta aktarım kuralı oluşturmak için:

1. 'da yönetim merkezine gidin ve <https://admin.microsoft.com> Yönetim merkezleri **'ni Exchange.** \> 

2. Posta **akışı kategorisinde kurallar** öğesini **seçin.**

3. öğesini **+** seçin ve ardından Yeni kural oluştur öğesini **seçin.**

4. Tam **seçenek kümesi** görmek için iletişim kutusunun altındaki Diğer seçenekler'i seçin.

5. Kural için aşağıdaki tabloda yer alan ayarları uygulama. Diğer ayarlar için varsayılan değerleri, değiştirmek istemiyorsanız kullanın.

6. **Kaydet**'i seçin.

|Ayar|Dosya eklerini açmadan önce Office uyar||
|---|---|---|
|Name|Fidye yazılımıyla mücadele kuralı: kullanıcıları uyarın|
|Bu kuralı şu durumda uygula: . . .|Herhangi bir ek. . . dosya uzantısı eşleşmeleri . . .|
|Sözcükleri veya tümcecikleri belirtme|Şu dosya türlerini ekleyin:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Aşağıdakini yapın. . .|Alıcıyı bir iletiyle bilgilendirin|
|İleti metni sağlama|Bu tür dosyaları, kötü amaçlı kod içeren makrolar içere içere bilmleri olduğundan, bu tür dosyaları açmayın.|

Daha fazla bilgi için bkz.:

- [Fidye yazılımı: riski azaltma](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-posta için otomatik iletmeyi durdurma

Bir kullanıcının posta kutusuna erişim elde eden bilgisayar korsanları, posta kutusunu otomatik olarak e-postayı iletacak şekilde ayarerek e-postaları çalmak anlamına gelir. Bu durum, kullanıcının farkında olmadan bile olabilir. Bunun önüne geçmek için bir posta akışı kuralı yapılandırabilirsiniz.

Posta aktarım kuralı oluşturmak için bu kısa [videoyu izleyin veya](../business-video/stop-email-auto-forward.md) şu adımları izleyin:

1. Genel yönetim Microsoft 365 Yönetim merkezleri **'ni Exchange.** \> 

2. Posta **akışı kategorisinde kurallar** öğesini **seçin.**

3. öğesini **+** seçin ve ardından Yeni kural oluştur öğesini **seçin.**

4. Tüm seçenekleri görmek için iletişim **kutusunun altındaki** Diğer seçenekler'i seçin.

5. Aşağıdaki tabloda yer alan ayarları uygulama. Diğer ayarlar için varsayılan değerleri, değiştirmek istemiyorsanız kullanın.

6. **Kaydet**'i seçin.

|Ayar|Dosya eklerini açmadan önce Office uyar|
|---|---|
|Name|E-postanın dış etki alanlarına otomatik olarak ilet ingingsini engelleme|
|Bu kuralı şu durumda uygula:|Gönderen . . . dış/iç . . . Kuruluşun içinde|
|Koşul ekle|İleti özellikleri . . . ileti türünü de içerir. . . Otomatik olarak iletme|
|Aşağıdakini yapın ...|İletiyi engelin. . . iletiyi reddeder ve bir açıklama içerir.|
|İleti metni sağlama|Güvenlik nedeniyle, e-postanın bu kuruluş dışında otomatik olarak ilet organizasyonun dışından ilet önlenmesi.|


## <a name="protect-your-email-from-phishing-attacks"></a>E-postanızı kimlik avı saldırılarından koruma

Kimlik avı ortamınız veya ortamınız için bir veya daha fazla Office 365 Microsoft 365, hedefli kimlik avı korumasını yapılandırabilirsiniz. Office 365 için Microsoft Defender'ın bir parçası olan Kimlik avı koruması, organizasyonlarınızı kötü amaçlı kimliğe bürünme tabanlı kimlik avı saldırılarından ve diğer kimlik avı saldırılarından korumaya yardımcı olabilir. Özel etki alanını yapılandırmadınız, bunu yapmak zorunda değilsiniz.

En önemli kullanıcılarınızı ve özel etki alanınızı korumak için bir ilke oluşturarak, bu korumayla çalışmaya başlamanızı öneririz.

For Office 365 için Microsoft Defender'da kimlik avına karşı koruma ilkesi oluşturmak için bu kısa eğitim [videosunu](../business-video/setup-anti-phishing.md)izleyin veya aşağıdaki adımları tamamlayın:

1. [https://protection.office.com](https://protection.office.com) adımına gidin.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit **yönetimi'nin altında İlke'yi** **seçin.**

3. İlke **sayfasında** Kimlik avından **korunma'ya tıklayın.**

4. Kimlik avı **önleme sayfasında +** Oluştur'a **tıklayın.** Kimlik avına karşı koruma ilkenizi tanımlamanız için size yol belirleyen bir sihirbaz başlatır.

5. İlkenizin adını, açıklamasını ve ayarlarını aşağıdaki tabloda önerilen şekilde belirtin. Daha fazla ayrıntı için bkz. Kimlik avı önleme [seçenekleri için Microsoft Defender'da kimlik Office 365 öğrenin.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Ayarlarınızı gözden geçirmenizin ardından, Uygun şekilde Bu ilkeyi **oluştur'a veya** **Kaydet'e** tıklayın.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Etki alanı ve en değerli kampanya personeli|
|Açıklama|En önemli personelin ve etki alanımızın kimliğine bürünülmemelerini sağlar.|
|Korumak için kullanıcı ekleme|+ **Koşul ekle'yi seçin, Alıcı şudur:**. Kullanıcı adlarını yazın veya aday, kampanya yöneticisi ve diğer önemli personel üyelerinin e-posta adresini girin. Kimliğe bürünmelerden korumak istediğiniz en çok 20 iç ve dış adres ebilirsiniz.|
|Korumak için etki alanı ekleme|+ **Koşul ekle'yi seçin, Alıcı etki alanı şudur:**. Tanımladıysanız, Microsoft 365 aboneliğiniz ile ilişkili özel etki alanını girin. Birden çok etki alanı girebilirsiniz.|
|Eylemleri seçme|E-posta kimliğine bürünülen bir kullanıcı tarafından gönderilirse: İletiyi başka bir e-posta adresine yeniden yönlendir'i seçin ve güvenlik yöneticisinin e-posta adresini yazın; örneğin, *<span> <span> Çiğdem @contoso.com.* E-posta kimliğine bürünülen bir etki alanı tarafından gönderilirse: İletiyi **karantinaya alın'ı seçin.**|
|Posta kutusu zekası|Yeni bir kimlik avı önleme ilkesi oluşturmak, posta kutusu zekası varsayılan olarak seçilidir. En iyi sonuçları elde **etmek için bu** ayarı Açık bırakın.|
|Güvenilen gönderenleri ve etki alanlarını ekleme|Buradan kendi etki alanlarınızı veya diğer güvenilen etki alanlarınızı eklemeye devam edersiniz.|
|Uygulamanın uygulandığı yer|Alıcı **etki alanı' öğesini seçin.** Bu **seçeneklerden herhangi biri altında** Seç öğesini **seçin.** **+ Ekle öğesini seçin.** Etki alanı adının yanındaki onay kutusunu işaretleyin; örneğin, *contoso. <span> <span> com*'a tıklayın ve ardından Ekle'yi **seçin.** Bitti **öğesini seçin.**|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Dosya Ekleriyle kötü amaçlı eklere ve Kasa koruma

Kişiler belge, sunu, elektronik tablo gibi ekleri düzenli aralıklarla gönderir, alır ve paylaşır. Yalnızca bir e-posta iletisine bakarak eklerin güvenli mi yoksa kötü amaçlı mı olduğunu söylemek her zaman kolay değildir. Office 365 için Microsoft Defender Kasa Koruması içerir, ancak bu koruma varsayılan olarak açık değildir. Bu korumayı kullanmaya başlamak için yeni bir kural oluşturmanızı öneririz. Bu koruma dosya, dosya SharePoint OneDrive dosyaları Microsoft Teams.

Ek Kasa ilkesi oluşturmak için bu kısa [videoyu izleyin](../business-video/safe-attachments.md)veya aşağıdaki adımları tamamlayın:

1. 'a [https://protection.office.com](https://protection.office.com) gidin ve yönetici hesabınızla oturum açın.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit **yönetimi'nin altında İlke'yi** **seçin.**

3. İlke sayfasında Ekleri **Ekle'Kasa seçin.**

4. Ekleri Kasa bu korumayı daha geniş bir şekilde uygulamak için **SharePoint,** OneDrive ve Microsoft Teams'i aç onay kutusunu seçin.

5. Yeni **+** bir ilke oluşturmak için öğesini seçin.

6. Aşağıdaki tabloda yer alan ayarları uygulama.

7. Ayarlarınızı gözden geçirmenizin ardından, Uygun şekilde **Bu ilkeyi oluştur'a veya** **Kaydet'e** tıklayın.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Kötü amaçlı yazılım algılandı olarak mevcut ve gelecekteki e-postaları engelin.|
|Açıklama|Kötü amaçlı yazılım algılandı olarak mevcut ve gelecek e-postaları ve ekleri engelin.|
|Bilinmeyen kötü amaçlı yazılım yanıtını kaydetme|Engelle **- Geçerli ve gelecekteki e-postaları ve kötü amaçlı yazılım algılandı olan ekleri engelle'yi seçin.**|
|Eki algılamada yeniden yönlendirme|Yeniden yönlendirmeyi etkinleştir (bu kutuyu seçin) Yönetici hesabını veya karantina için posta kutusu kurulumunu girin.          Kötü amaçlı yazılım ekleri tarayanın zaman dışında veya hata oluştuğunda yukarıdaki seçimi uygula (bu kutuyu seçin).|
|Uygulamanın uygulandığı yer|Alıcı etki alanı: . . . etki alanınızı seçin.|

Daha fazla bilgi için bkz. Kimlik avı için [Microsoft Defender'da kimlik avı ilkelerini Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Yeni Bağlantılar ile kimlik avı saldırılarına Kasa koruyun

Bilgisayar korsanları bazen e-posta veya diğer dosyalarda bağlantılarda kötü amaçlı web sitelerini gizler. Kasa Office 365 için Microsoft Defender'ın bir parçası olan bağlantılar, e-posta iletilerinde ve belgelerinde web adreslerinin (URL'ler) tıklamayla doğrulanması yoluyla, Office yardımcı olabilir. Koruma, Bağlantı İlkeleri Kasa tanımlanır.

Şunları yapmanizi öneririz:

- Korumayı artırmak için varsayılan ilkeyi değiştirme.

- Etki alanınız içinde yer alan tüm alıcılara hedeflenen yeni bir ilke ekleyin.

Bağlantılar'Kasa ayarlamak için bu [kısa eğitim videosunu izleyin](../business-video/safe-links.md)veya aşağıdaki adımları tamamlayın:

1. 'a [https://protection.office.com](https://protection.office.com) gidin ve yönetici hesabınızla oturum açın.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit **yönetimi'nin altında İlke'yi** **seçin.**

3. İlke sayfasında, **Bağlantılar'ı Kasa seçin.**

Varsayılan ilkeyi değiştirmek için:

1. Yeni Kasa sayfasında, Kuruluşun **tamamına uygulanacak ilkeler'in altında** Varsayılan **ilke'yi** seçin.

2. **E Ayarlar dışında içeriğe uygun içerik için geçerli olan e-posta** altında, iOS Kurumlar için Microsoft 365 Uygulamaları Android için **Office'yi seçin.**

3. **Kaydet**'i seçin.

Etki alanınız içinde yer alan tüm alıcılara hedeflenen yeni bir ilke oluşturmak için:

1. Yeni Kasa tüm kuruluşa uygulanacak **ilkeler altında,** yeni bir **+** ilke oluşturmak için öğesini seçin.

2. Aşağıdaki tabloda listelenen ayarları uygulama.

3. **Kaydet**'i seçin.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Kasa etki alanındaki tüm alıcılar için bağlantı ilkesi ekleme|
|İletilerde kötü amaçlı olabilecek bilinmeyen URL'lerin eylemlerini seçme|Açık Olarak Seç - KULLANıCı bağlantıya tıkladığında URL'ler yeniden yazılır ve bilinen kötü **amaçlı bağlantılar listesinde denetlenir.**|
|İndirilebilir Kasa taramak için Ekleri Kullanma|Bu kutuyu seçin.|
|Uygulamanın uygulandığı yer|Alıcı etki alanı: . . . etki alanınızı seçin.|

Daha fazla bilgi için [bağlantılara Kasa bakın.](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Intune yönetim merkezine gitme

1. [Azure portalda oturum açın.](https://portal.azure.com/)

2. Tüm **hizmetler'i** seçin ve *Arama Kutusuna Intune* **yazın.**

3. Sonuçlar görüntüden sonra, daha sonra kolayca **bulmak Microsoft Intune** yanındaki başlangıç öğesini seçin.

Yönetim merkezine ek olarak, Intune'u kullanarak kuruluşun cihazlarını kaydolarak yönetebilirsiniz. Daha fazla bilgi için [bkz.](/intune/enrollment/enrollment-method-capab) Farklı cihazlar için kayıt Windows ve [Intune](/intune/enrollment-options)tarafından yönetilen cihazlar için Kayıt seçenekleri.
