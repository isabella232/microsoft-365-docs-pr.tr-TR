---
title: Microsoft 365 İş için tehdit korumasını artırma
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
description: Office 365 için Microsoft Defender'ı ayarlayın ve kimlik avı, kötü amaçlı yazılım ve diğer tehditlere karşı hassas verileri koruyun.
ms.openlocfilehash: 8fb2c3881876cabea6d8907a85bc9397212126dc
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580204"
---
# <a name="increase-threat-protection"></a>Tehdit korumasını artırma

Bu makale kimlik avına, kötü amaçlı yazılıma ve diğer tehditlere karşı korumak için Microsoft 365 aboneliğinizin korumasını artırmanıza yardımcı olur. Bu öneriler, hukuk ofisleri ve sağlık hizmetleri klinisleri gibi güvenlik ihtiyacı artan kuruluşlara uygundur.

Başlamadan önce Office 365 Güvenli Puanınızı kontrol edin. Office 365 Güvenli Puan, normal etkinliklerinize ve güvenlik ayarlarınıza göre kuruluş güvenliğini analiz eder ve bir puan atar. Başlangıç olarak geçerli puanınızı not alarak başlayabilirsiniz. Puanınızı artırmak için, bu makalede önerilen eylemleri gerçekleştirin. Amaç maksimum puanı elde etmek değil, kullanıcılarınız için üretkenliği olumsuz etkilemeden ortamınızı koruma fırsatlarına dikkat etmektir.

Daha fazla bilgi için [Microsoft Güvenli Puan'a bakın.](../security/defender/microsoft-secure-score.md)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Postada kötü amaçlı yazılıma karşı koruma düzeyini yükseltme

Office 365 veya Microsoft 365 ortamınız kötü amaçlı yazılıma karşı koruma içerir. Kötü amaçlı yazılım için yaygın olarak kullanılan dosya türlerine sahip ekleri engelleyerek bu korumayı artırabilirsiniz. E-postada kötü amaçlı yazılımdan korunmayı artırmak için:

1. Yönetici hesabı [https://protection.office.com](https://protection.office.com) kimlik bilgilerinize gidin ve bu kimlik bilgileriyle oturum açın.

2. Güvenlik Uyumluluk Merkezi'nin sol gezinti bölmesinde, Tehdit yönetimi altında, İlke Kötü Amaçlı &amp; Yazılımdan   \> **Koruma'ya tıklayın.**

3. Şirket genelindeki bu ilkeyi düzenlemek için varsayılan ilkeye çift tıklayın.

4. **Ayarlar'ı seçin.**

5. Ortak **Ek Türleri Filtresi'nin altında,** Aç'ı **seçin.** Engellenen dosya türleri bu denetimin hemen altındaki pencerede listelenir. Şu dosya türlerini ekley mutlaka:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Gerekirse, daha sonra dosya türlerini ekleyebilir veya silebilirsiniz.

6. **Kaydet'i seçin.**

Daha fazla bilgi için bkz. [EOP'de kötü amaçlı yazılımdan koruma.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Fidye yazılımlarına karşı koruma

Fidye yazılımları, dosyaları şifreleyerek veya bilgisayar ekranlarını kilitleyerek verilere erişimi kısıtlar. Ardından, verilere erişim için genellikle Bitcoin gibi şifreleme paraları şeklinde olan "her tür şifreleme" talep eden bir ifadeyle, kabul etmek zorunda olduğu paraların ekseriyetten yararlanmaya çalışır.

Fidye yazılımlarına karşı korumak için, fidye yazılımları için yaygın olarak kullanılan dosya uzantılarını engellemek için bir veya daha fazla posta akışı kuralı oluşturun. (Posta adımlarında bu kuralları [kötü amaçlı yazılıma karşı koruma düzeyini yükseltmek için eklediniz.)](#raise-the-level-of-protection-against-malware-in-mail) Bu ekleri e-postayla alan kullanıcıları da uyarabilirsiniz.

Önceki adımda engelley istediğiniz dosyalara ek olarak, makro içeren Office dosya eklerini açmadan önce kullanıcıları uyaran bir kural oluşturmak iyi bir yöntemdir. Fidye yazılımları makroların içinde gizlenmiş olabilir, bu nedenle kullanıcıları bu dosyaları kendiıldıklarından açmamalarını uyarın.

Posta aktarım kuralı oluşturmak için:

1. Yönetim merkezine gidin ve <https://admin.microsoft.com> Exchange Yönetim **merkezleri'ni** \> **seçin.**

2. Posta **akışı kategorisinde** kuralları **seçin.**

3. Seçin **+** ve ardından Yeni kural **oluştur'a seçin.**

4. Tüm **seçenek kümelerini** görmek için iletişim kutusunun en altındaki Diğer seçenekler'i seçin.

5. Kural için aşağıdaki tabloda yer alan ayarları uygulama. Ayarları değiştirmek istemiyorsanız, diğer ayarlar için varsayılan değerleri kullanın.

6. **Kaydet**'i seçin.

|Ayar|Office dosyalarının eklerini açmadan önce kullanıcıları uyar||
|---|---|---|
|Name|Fidye yazılımıyla mücadele kuralı: kullanıcıları uyar|
|Bu kuralı şu durumda uygula: . .|Herhangi bir ek . . . dosya uzantısı eşleşmeleri. . .|
|Sözcükleri veya tümcecikleri belirtme|Şu dosya türlerini ekleyin:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Aşağıdakini yapın. . .|Alıcıya bir iletiyle bildirme|
|İleti metni sağlama|Bu tür dosyaları, kötü amaçlı kod içeren makrolar içere olabileceğinden, sizin olmadığınız kişilerden açmayın.|

Daha fazla bilgi için bkz.:

- [Fidye yazılımı: riski azaltma](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [OneDrive'larınızı geri yükleme](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-posta için otomatik iletmeyi durdurma

Kullanıcının posta kutusuna erişim elde eden bilgisayar korsanları, posta kutusunu otomatik olarak e-postayı iletacak şekilde ayarerek posta çalmak zorunda olabilir. Bu durum, kullanıcının farkında olmadan da olabilir. Bunun önüne geçmek için, posta akışı kuralını yapılandırabilirsiniz.

Posta aktarım kuralı oluşturmak için bu kısa [videoyu izleyin veya](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) şu adımları izleyin:

1. Microsoft 365 yönetim merkezinde Exchange Yönetim **merkezleri'ni** \> **seçin.**

2. Posta **akışı kategorisinde** kuralları **seçin.**

3. Seçin **+** ve ardından Yeni kural **oluştur'a seçin.**

4. Tüm seçenekleri görmek için, iletişim **kutusunun en** altındaki Diğer seçenekler'i seçin.

5. Aşağıdaki tabloda yer alan ayarları uygulama. Ayarları değiştirmek istemiyorsanız, diğer ayarlar için varsayılan değerleri kullanın.

6. **Kaydet**'i seçin.

|Ayar|Office dosyalarının eklerini açmadan önce kullanıcıları uyar|
|---|---|
|Name|E-postanın dış etki alanlarına otomatik iletmesini önleme|
|Şu durumda bu kuralı uygula:|Gönderen . . . dış/iç . . . Kuruluşun içinde|
|Koşul ekle|İleti özellikleri. . . ileti türünü de içerir. . . Otomatik iletme|
|Aşağıdakini yapın ...|İletiyi engelin. . . iletiyi reddedin ve bir açıklama yazın.|
|İleti metni sağlama|Güvenlik nedeniyle e-postanın bu kuruluş dışında otomatik olarak ilet organizasyonun dışından iletebilirsiniz.|


## <a name="protect-your-email-from-phishing-attacks"></a>E-postanızı kimlik avı saldırılarından koruma

Office 365 veya Microsoft 365 ortamınız için bir veya birden çok özel etki alanı yapılandırdıysanız, hedefli kimlik avı önleme korumasını yapılandırabilirsiniz. Office 365 için Microsoft Defender'ın bir parçası olan kimlik avı koruma, organizasyonlarınızı kimliğe bürünme tabanlı kimlik avı saldırılarına ve diğer kimlik avı saldırılarına karşı korumaya yardımcı olabilir. Özel etki alanını yapılandırmadıysanız, bunu yapmak zorunda değildir.

En önemli kullanıcılarınızı ve özel etki alanınızı korumak için bir ilke oluşturarak bu korumayla çalışmaya başlamanızı öneririz.

Office 365 için Microsoft Defender'da kimlik avı önleme ilkesi oluşturmak için bu kısa eğitim  [videosunu](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)izleyin veya aşağıdaki adımları tamamlayın:

1. [https://protection.office.com](https://protection.office.com) adımına gidin.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit yönetimi altında **İlke'yi** **seçin.**

3. İlke **sayfasında** Kimlik avı **önleme'yi seçin.**

4. Kimlik avı **önleme sayfasında +** **Oluştur'a tıklayın.** Kimlik avı önleme ilkenizi tanımlamanız için size yol belirleyen bir sihirbaz başlatır.

5. İlkenizin adını, açıklamasını ve ayarlarını aşağıdaki tabloda önerilen şekilde belirtin. Daha fazla ayrıntı için, [Office 365 için Microsoft Defender](../security/office-365-security/set-up-anti-phishing-policies.md)seçeneklerinde kimlik avıyla mücadele ilkesi hakkında bilgi edinebilirsiniz.

6. Ayarlarınızı gözden geçirdikten sonra, Uygun şekilde Bu **ilkeyi oluştur veya** **Kaydet'i** seçin.

|Ayarlama veya seçenek|Önerilen ayar|
|---|---|
|Name|Etki alanı ve en değerli kampanya personeli|
|Açıklama|En önemli personelin ve etki alanımızın kimliğine bürünülmemelerini sağlar.|
|Korumak için kullanıcı ekleme|Select **+ Koşul ekle, Alıcı**. Kullanıcı adlarını yazın veya adayın, kampanya yöneticisinin ve diğer önemli personel üyelerinin e-posta adresini girin. Kimliğe bürünülmelerden korumak istediğiniz en çok 20 iç ve dış adres ebilirsiniz.|
|Korumak için etki alanları ekleme|Select **+ Koşul ekle, Alıcı etki alanı**. Microsoft 365 aboneliğiniz ile ilişkilendirilmiş özel etki alanını (tanımladıysanız) girin. Birden çok etki alanı girebilirsiniz.|
|Eylemleri seçme|E-posta kimliğine bürünülen bir kullanıcı tarafından gönderilirse: **İletiyi** başka bir e-posta adresine yeniden yönlendir'i seçin ve güvenlik yöneticisinin e-posta adresini yazın; örneğin, *Ali <span> <span> @contoso.com.* E-posta kimliğine bürünülen bir etki alanı tarafından gönderilirse: karantina **iletisi seçin.**|
|Posta kutusu zekası|Yeni bir kimlik avı önleme ilkesi oluşturmanız, posta kutusu zekası varsayılan olarak seçilidir. En iyi sonuçları elde **etmek için bu** ayarı Açık bırakın.|
|Güvenilen gönderenleri ve etki alanlarını ekleme|Buradan kendi etki alanlarınızı veya güvenilen diğer etki alanlarınızı eklemeye devam edersiniz.|
|Uygulama|Alıcı **etki alanı öğesini seçin.** Bunların **herhangi biri altında, Seç'i** **seçin.** Select **+ Add**. Etki alanının adının yanındaki onay kutusunu (örneğin, *contoso) seçin. <span> <span> com'da,* listede ve Ekle'yi **seçin.** **Bitti'yi seçin.**|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Güvenli Ekler ile kötü amaçlı eklere ve dosyalara karşı koruma

Kişiler belgeler, sunular, elektronik tablolar ve daha fazlası gibi ekleri düzenli olarak gönderir, alır ve paylaşır. Yalnızca e-posta iletisine bakarak ekin güvenli mi yoksa kötü amaçlı mı olduğunu söylemek her zaman kolay değildir. Office 365 için Microsoft Defender Güvenli Ek koruması içerir, ancak bu koruma varsayılan olarak açık değildir. Bu korumayı kullanmaya başlamak için yeni bir kural oluşturmanızı öneririz. Bu koruma SharePoint, OneDrive ve Microsoft Teams'de dosyalara kadar genişler.

Güvenli Ek ilkesi oluşturmak için bu kısa [videoyu izleyin veya](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)aşağıdaki adımları tamamlayın:

1. 'a [https://protection.office.com](https://protection.office.com) gidin ve yönetici hesabınızla oturum açın.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit yönetimi altında **İlke'yi** **seçin.**

3. İlke sayfasında Güvenli **Ekler'i seçin.**

4. Güvenli ekler sayfasında, **SharePoint, OneDrive** ve Microsoft Teams için ATP'yi aç onay kutusunu seçerek bu korumayı kapsamlı olarak uygulayabilirsiniz.

5. Yeni **+** bir ilke oluşturmak için seçin.

6. Aşağıdaki tabloda yer alan ayarları uygulama.

7. Ayarlarınızı gözden geçirdikten sonra, Uygun şekilde Bu **ilkeyi oluştur veya** **Kaydet'i** seçin.

|Ayarlama veya seçenek|Önerilen ayar|
|---|---|
|Name|Kötü amaçlı yazılım algılandığında geçerli ve gelecek e-postaları engelin.|
|Açıklama|Kötü amaçlı yazılım algılandığında mevcut ve gelecek e-postaları ve ekleri engelin.|
|Bilinmeyen kötü amaçlı yazılım yanıtını kaydetme|Engelle **-Algılandı kötü amaçlı yazılımla geçerli ve gelecekteki e-postaları ve ekleri engelle'yi seçin.**|
|Algılamada eki yeniden yönlendirme|Yeniden yönlendirmeyi etkinleştir (bu kutuyu seçin) Yönetici hesabını veya karantina için bir posta kutusu kurulumu girin.          Kötü amaçlı yazılım ekleri tararsa veya hata oluşursa yukarıdaki seçimi uygulama (bu kutuyu seçin).|
|Uygulama|Alıcı etki alanı . . . etki alanınızı seçin.|

Daha fazla bilgi için Bkz. [Office 365](../security/office-365-security/set-up-anti-phishing-policies.md)için Microsoft Defender'da kimlik avı önleme ilkelerini ayarlama.

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Güvenli Bağlantılar ile kimlik avı saldırılarına karşı koruma

Bilgisayar korsanları bazen e-posta veya diğer dosyalarda bağlantılarda kötü amaçlı web sitelerini gizler. Office 365 için Microsoft Defender'ın bir parçası olan Güvenli Bağlantılar, e-posta iletilerinde ve Office belgelerinde web adreslerinin (URL'ler) tıklanması için zamanında doğrulama sağlayarak organizasyonlarınızı korumaya yardımcı olabilir. Koruma, Güvenli Bağlantılar ilkeleri aracılığıyla tanımlanır.

Şunları yapmanizi öneririz:

- Korumayı artırmak için varsayılan ilkeyi değiştirme.

- Etki alanınız içinde yer alan tüm alıcılara hedeflenen yeni bir ilke ekleyin.

Güvenli Bağlantıları ayarlamak için bu [kısa eğitim videosunu izleyin](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)veya aşağıdaki adımları tamamlayın:

1. 'a [https://protection.office.com](https://protection.office.com) gidin ve yönetici hesabınızla oturum açın.

2. Güvenlik Uyumluluk &amp; Merkezi'nin sol gezinti bölmesinde, Tehdit yönetimi altında **İlke'yi** **seçin.**

3. İlke sayfasında Güvenli **Bağlantılar'ı seçin.**

Varsayılan ilkeyi değiştirmek için:

1. Güvenli bağlantılar sayfasında, kuruluşun **tamamına uygulanacak İlkeler'in** altında Varsayılan **ilkeyi** seçin.

2. **E-posta dışındaki içeriğe uygulanacak Ayarlar'ın** altında, kurumsal **Microsoft 365 Uygulamaları, iOS ve Android için Office'i seçin.**

3. **Kaydet**'i seçin.

Etki alanınız içinde yer alan tüm alıcılara yönelik yeni bir ilke oluşturmak için:

1. Güvenli bağlantılar sayfasında, kuruluşun **tamamına uygulanacak İlkeler'in** altında yeni **+** bir ilke oluşturmak için seçin.

2. Aşağıdaki tabloda listelenen ayarları uygulama.

3. **Kaydet**'i seçin.

|Ayarlama veya seçenek|Önerilen ayar|
|---|---|
|Name|Etki alanındaki tüm alıcılar için güvenli bağlantılar ilkesi|
|İletilerde bilinmeyen kötü amaçlı olabilecek URL'ler için eylemi seçme|Açık **- URL'ler yeniden yazılır ve kullanıcı** bağlantıya tıkladığında bilinen kötü amaçlı bağlantılar listesinde denetlenir.|
|İndirilebilir içeriği taramak için Güvenli Ekler'i kullanma|Bu kutuyu seçin.|
|Uygulama|Alıcı etki alanı . . . etki alanınızı seçin.|

Daha fazla bilgi için Güvenli [Bağlantılar'a bakın.](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Intune yönetim merkezine gitme

1. Azure portalında [oturum açın.](https://portal.azure.com/)

2. Tüm **hizmetleri seçin** ve Arama Kutusuna *Intune* **yazın.**

3. Sonuçlar görüntüden sonra, Microsoft **Intune'un** yanındaki başlangıç öğesini seçerek sık kullanılanlara ve daha sonra kolayca bulunabilirsiniz.

Yönetim merkezine ek olarak, Intune'u kullanarak kurum cihazlarınızı da kaydedecek ve yönetebilirsiniz. Daha fazla bilgi için Windows [cihazları için kayıt yöntemine göre](/intune/enrollment/enrollment-method-capab) özelliklere ve Intune tarafından yönetilen cihazlar için Kayıt [seçeneklerine bakın.](/intune/enrollment-options)
