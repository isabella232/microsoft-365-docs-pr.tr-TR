---
title: Iş için Microsoft 365 tehdit korumasını arttırın
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş tehdit korumasını ayarlayın ve sızdırma, kötü amaçlı yazılım ve diğer tehditlere karşı hassas verileri güvenceye alın.
ms.openlocfilehash: d56a5371bc5fc4da22f4625024769cc0325a25ca
ms.sourcegitcommit: dffb9b72acd2e0bd286ff7e79c251e7ec6e8ecae
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/17/2020
ms.locfileid: "47948598"
---
# <a name="increase-threat-protection"></a>Tehdit korumasını arttırma

Bu makale, sızdırma, kötü amaçlı yazılım ve diğer tehditlere karşı korunmak amacıyla Microsoft 365 aboneliğinizdeki korumayı artırmanıza yardımcı olur. Bu öneriler, yasalar, yasalar ve sağlık hizmetleri Kliniği gibi güvenlik için artış artışı olan kuruluşlar için uygundur.

Başlamadan önce, Office 365 güvenli Puanını denetleyin. Office 365 güvenli puanı, kuruluşunuzun güvenliğini düzenli etkinliklerinizi ve Güvenlik ayarlarınıza göre çözümler ve bir puan atar. Geçerli puanınızın notunu almayı başlatın. Puanınızı büyütmek için bu makalede önerilen eylemleri tamamlayın. Amaç en fazla puanı elde etmeyin, ancak iş fırsatlarınızı, kullanıcılarınız için üretkenliği olumsuz etkilemeyecek şekilde korumamak için fırsatlar

Daha fazla bilgi için bkz: [Microsoft güvenli skor](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Posta 'da kötü amaçlı yazılıma karşı koruma düzeyini yükseltme

Office 365 veya Microsoft 365 ortamınız, kötü amaçlı yazılımlara karşı koruma içerir. Sık kullanılan kişilerle sık kullanılan dosyaları engelleyerek bu korumayı artırabilirsiniz. E-postadaki kötü amaçlı yazılım korumasını yükseltmek için:

1. [https://protection.office.com](https://protection.office.com)Yönetici hesabı kimlik bilgilerinizle gidin ve oturum açın.

2. Güvenlik &amp; Uyumluluk merkezinde, sol gezinti bölmesinde, **tehdit yönetimi**'nin altında, **ilke** \> **önleme önleme**'yı seçin.

3. Bu şirket çapındaki ilkeyi düzenlemek için varsayılan ilkeyi çift tıklatın.

4. **Ayarlar**'ı seçin.

5. **Ortak ek türleri filtresi**altında **Açık**öğesini seçin. Engellenen dosya türleri, bu denetimin hemen altındaki pencerede listelenir. Bu dosya türlerini eklediğinizden emin olun:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Gerekirse, daha sonra dosya türlerini ekleyebilir veya silebilirsiniz.

6. Kaydet 'i seçin **.**

Daha fazla bilgi için [EOP 'de kötü amaçlı yazılımdan koruma](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection)konusuna bakın.

## <a name="protect-against-ransomware"></a>Fidye aşamalarına karşı korunma

Fidye yazılımı, dosyaları şifreleyerek veya bilgisayar ekranlarını kilitleyerek verilere erişimi kısıtlar. Ardından, "ransoırlar" ("ransolar", "ransolar" ("ransolar" (

Fidye kurallarına karşı korunmak için, fidye kuralları için yaygın olarak kullanılan dosya uzantılarını engellemek üzere bir veya daha fazla posta akış kuralı oluşturun. (Bu kuralları, [posta adımında kötü amaçlı yazılımlara karşı koruma düzeyini artırdır](#raise-the-level-of-protection-against-malware-in-mail) .) Ayrıca, e-postada bu ekleri alan kullanıcıları uyarabilirsiniz.

Önceki adımda engellediğiniz dosyaların yanı sıra, makro içeren Office dosya eklerini açmadan önce kullanıcıları uyarmak için bir kural oluşturmak iyi bir yöntemdir. Fidye, makrolar içinde gizlenebilir, bu nedenle kullanıcılara bilmediğiniz kişilerin bu dosyaları açmasını sağlayın.

Posta aktarım kuralı oluşturmak için:

1. Yönetim Merkezi 'ne gidin <https://admin.microsoft.com> ve **Yönetim Merkezleri** \> **Exchange**'i seçin.

2. **Posta akışı** kategorisinde **kurallar**'ı seçin.

3. **+** Öğesini seçin ve sonra **Yeni kural oluştur**'u seçin.

4. Tüm seçenekleri görmek için iletişim kutusunun en altındaki **diğer seçenekler** 'i seçin.

5. Kural için aşağıdaki tabloda yer alan ayarları uygulayın. Ayarları değiştirmek istemiyorsanız, kalan ayarların varsayılan değerlerini kullanın.

6. **Kaydet**'i seçin.

|Ayar|Office dosyalarının eklerini açmadan önce kullanıcıları uyarma||
|---|---|---|
|Name|Önleme kuralı: kullanıcıları uyarma|
|Bu kuralı uygulayın. . .|Herhangi bir ek. . . Dosya Uzantısı eşleşiyor. . .|
|Sözcükleri veya tümceleri belirtme|Bu dosya türlerini ekleyin:  <br/> dotm, docm, xlsm, sltm, xla, xlam, XLL, PPTM, potm, PPAM, PPSM, SLDM|
|Aşağıdakileri yapın. . .|Alıcıya iletiyle bildirme|
|İleti metni sağlama|Tanımadığınız kişilerden bu tür dosyaları, kötü amaçlı kod içeren makrolar içerebileceğinden açmayın.|

Daha fazla bilgi için bkz.:

- [Fidye yöntemleri: riski azaltma](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [OneDrive 'ı geri yükleme](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-posta için otomatik yönlendirmeyi durdurma

Bir kullanıcının posta kutusuna erişimi olan saldırganlar, posta kutusunu e-postayı otomatik olarak iletecek şekilde ayarlayarak posta çalabilir. Bu, Kullanıcı tanıma olmadan da gerçekleşebilir. Bunu önlemek için, posta akış kuralı yapılandırın.

Posta aktarım kuralı oluşturmak için [Bu kısa videoyu](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) izleyin veya şu adımları izleyin:

1. Microsoft 365 Yönetim merkezinde, **Yönetim Merkezleri** \> **Exchange**'i seçin.

2. **Posta akışı** kategorisinde **kurallar**'ı seçin.

3. **+** Öğesini seçin ve sonra **Yeni kural oluştur**'u seçin.

4. Tüm seçenekleri görmek için iletişim kutusunun en altındaki **diğer seçenekler** 'i seçin.

5. Aşağıdaki tabloda yer alan ayarları uygulayın. Ayarları değiştirmek istemiyorsanız, kalan ayarların varsayılan değerlerini kullanın.

6. **Kaydet**'i seçin.

|Ayar|Office dosyalarının eklerini açmadan önce kullanıcıları uyarma|
|---|---|
|Name|E-postanın dış etki alanlarına otomatik olarak iletilmesini önle|
|Bu kuralı uygula...|Gönderen. . . dış/iç. . . Kuruluş içindeki|
|Koşul ekleme|İleti özellikleri. . . ileti türünü ekleyin. . . Otomatik ilet|
|Aşağıdakileri yapın...|İletiyi engelleyin. . . iletiyi reddedin ve bir açıklama ekleyin.|
|İleti metni sağlama|E-postayı bu kuruluşun dışına otomatik olarak iletme güvenlik nedenleriyle engellenmiştir.|


## <a name="protect-your-email-from-phishing-attacks"></a>E-postanızı kimlik avı saldırılarından korunma

Office 365 veya Microsoft 365 ortamınız için bir veya daha fazla özel etki alanı yapılandırdıysanız, hedeflenen kimlik avı korumasını yapılandırabilirsiniz. ATP önleme Anti-Office 365 Gelişmiş tehdit koruması, kuruluşunuzun kötü kimliğe bürünme tabanlı kimlik avı saldırılarından ve diğer kimlik avı saldırılarından korunmasına yardımcı olabilir. Özel bir etki alanı belirtmediyseniz, bunu yapmanız gerekmez.

En önemli kullanıcılarınızı ve özel etki alanınızı korumaya yönelik bir ilke oluşturarak bu korumaya başlamanızı öneririz.

ATP Anti-kimlik avı ilkesi oluşturmak için,  [Bu kısa eğitim videosunu](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)izleyin veya aşağıdaki adımları tamamlayın:

1. [https://protection.office.com](https://protection.office.com) adımına gidin.

2. Güvenlik &amp; Uyumluluk merkezinde, sol gezinti bölmesinde, **tehdit yönetimi**'Nin altında, **ilke**'yi seçin.

3. **İlke** sayfasında **ATP önleme önleme**'yı seçin.

4. **Kimlik avı önleme** sayfasında **+ Oluştur**'u seçin. Bir sihirbaz, kimlik avlama önleme ilkenizi tanımlama adımlarında size yol açar.

5. Aşağıdaki tabloda önerildiği şekilde ilkenizin adını, açıklamasını ve ayarlarını belirtin. Daha fazla bilgi için [ATP önleme önleme ilkesi seçenekleri hakkında bilgi edinin](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

6. Ayarlarınızı inceledikten sonra **Bu Ilkeyi oluştur** veya uygun şekilde **Kaydet**'i seçin.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Etki alanı ve en değerli kampanya personeli|
|Açıklama|Önemli personelin ve etki alanınızın özellikleri alınamaz olmasını sağlayın.|
|Korunacak kullanıcıları ekleme|Select **+ Koşul Ekle, alıcı**. Kullanıcı adlarını yazın veya aday, kampanya yöneticisi ve diğer önemli personel üyelerinin e-posta adresini girin. Özelliklerini almada korunmalarını istediğiniz en çok 20 dahili ve harici adresi ekleyebilirsiniz.|
|Korunacak etki alanları ekleme|Select **+ Koşul Ekle, alıcı etki alanı**. Siz tanımladıysanız, Microsoft 365 aboneliğinizle ilişkili özel etki alanını girin. Birden çok etki alanı girebilirsiniz.|
|Eylemleri seçin|E-posta, kimliğine bürünülen bir kullanıcı tarafından gönderilirse: **iletiyi başka bir e-posta adresine yönlendir**'i seçin ve güvenlik yöneticisinin e-posta adresini yazın; Örneğin, *çiğdem <span> <span> @contoso. com*. E-posta, kimliğine bürünülen etki alanı tarafından gönderilirse: **karantina iletisi**'ni seçin.|
|Posta kutusu bilgileri|Yeni bir kimlik avı ilkesi oluşturduğunuzda, varsayılan olarak, posta kutusu bilgileri seçilidir. Bu ayarı en iyi sonuçlar için **Açık** bırakın.|
|Güvenilir Gönderenler ve etki alanları ekleme|Buraya kendi etki alanınızı veya diğer güvenilen etki alanlarını ekleyebilirsiniz.|
|Uygulanacak|**Alıcı etki alanını**seçin. **Bunlardan herhangi**birinin altında **Seç**'i seçin. **+ Ekle**'yi seçin. Etki alanı adının yanındaki (örneğin, Contoso) yanındaki kutuyu işaretleyin *. <span> <span> *ve **Ekle**'yi seçin. **Bitti**'yi seçin.|

## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>ATP güvenli eki olan kötü niyetli eklere ve dosyalara karşı korunma

İnsanlar belgeler, sunular, elektronik tablolar ve daha fazlası gibi ekleri düzenli olarak gönderirler, alır ve paylaşabilir. Bir e-posta iletisine bakarak bir ekin güvenli veya kötü amaçlı olup olmadığını söylemek her zaman kolaydır. Office 365 Gelişmiş tehdit koruması, ATP güvenli ek korumasını içerir, ancak bu koruma varsayılan olarak açık değildir. Bu korumayı kullanmaya başlamak için yeni bir kural oluşturmanızı öneririz. Bu koruma, SharePoint, OneDrive ve Microsoft ekipte bulunan dosyalar için genişler.

ATP güvenli ek ilkesi oluşturmak için [Bu kısa videoyu](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)izleyin veya aşağıdaki adımları tamamlayın:

1. Adresine gidin [https://protection.office.com](https://protection.office.com) ve Yönetici hesabınızla oturum açın.

2. Güvenlik &amp; Uyumluluk merkezinde, sol gezinti bölmesinde, **tehdit yönetimi**'Nin altında, **ilke**'yi seçin.

3. Ilke sayfasında **ATP güvenli ekleri**'ni seçin.

4. Güvenli ekler sayfasında, **SharePoint, OneDrive ve Microsoft ekipleri IÇIN ATP 'Yi aç** seçeneğini belirleyerek bu korumayı genel kullanıma uygulayın.

5. **+** Yeni ilke oluşturmak için öğesini seçin.

6. Aşağıdaki tabloda yer alan ayarları uygulayın.

7. Ayarlarınızı inceledikten sonra **Bu Ilkeyi oluştur** veya uygun şekilde **Kaydet**'i seçin.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Kötü amaçlı yazılım bulunan güncel ve gelecek e-postaları engelleyin.|
|Açıklama|Kötü amaçlı yazılım bulunan güncel ve gelecekteki e-postaları ve ekleri engelleyin.|
|Ekleri Kaydet bilinmeyen kötü amaçlı yazılım yanıtı|**, Kötü amaçlı yazılım algılanan geçerli ve gelecekteki e-postaları engelle**seçeneğini belirleyin.|
|Eki algılama sırasında yeniden yönlendirme|Yeniden yönlendirmeyi etkinleştir (Bu kutuyu seçin) karantina için yönetici hesabını veya posta kutusu kurulumunu girin.          Ek zaman aşımına uğruyor veya hata oluştuğunda, yukarıdaki seçimi uygulama (Bu kutuyu seçin).|
|Uygulanacak|Alıcı etki alanı. . . etki alanınızı seçin.|

Daha fazla bilgi için [365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)bkz.

## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>ATP güvenli bağlantılarıyla sızdırma saldırılarına karşı korunma

Saldırganlar bazen e-posta veya diğer dosyalardaki bağlantılarda kötü amaçlı Web sitelerini gizler. Office 365 ATP güvenli bağlantılar (ATP güvenli bağlantıları), Office 365 Gelişmiş tehdit koruması 'nın bir parçası olarak, e-posta iletilerinde ve Office belgelerinde Web adresleri (URL 'Ler) için süre sonu doğrulaması sağlayarak kuruluşunuzun korunmasına yardımcı olabilir. Koruma, ATP güvenli bağlantılar ilkeleri aracılığıyla tanımlanır.

Aşağıdakileri yapmanız önerilir:

- Korumayı yükseltmek için varsayılan ilkeyi değiştirin.

- Etki alanınızda tüm alıcılara hedeflenmiş yeni bir ilke ekleyin.

ATP güvenli bağlantılarını ayarlamak için, [Bu kısa eğitim videosunu](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)izleyin veya aşağıdaki adımları tamamlayın:

1. Adresine gidin [https://protection.office.com](https://protection.office.com) ve Yönetici hesabınızla oturum açın.

2. Güvenlik &amp; Uyumluluk merkezinde, sol gezinti bölmesinde, **tehdit yönetimi**'Nin altında, **ilke**'yi seçin.

3. Ilke sayfasında **ATP güvenli bağlantıları**'nı seçin.

Varsayılan ilkeyi değiştirmek için:

1. Güvenli bağlantılar sayfasında, **tüm kuruluşa uygulanan ilkeler**altında, **varsayılan** ilkeyi seçin.

2. **E-posta dışında içeriğe uygulanan ayarlar**'ın altında **kurumsal Için Microsoft 365 uygulamaları, iOS ve Android için Office 'i**seçin.

3. **Kaydet**'i seçin.

Etki alanınızda tüm alıcılara hedeflenmiş yeni bir ilke oluşturmak için:

1. Güvenli bağlantılar sayfasında, **tüm kuruluşa uygulanan ilkeler**altında, **+** Yeni ilke oluşturmak için öğesini seçin.

2. Aşağıdaki tabloda listelenen ayarları uygulayın.

3. **Kaydet**'i seçin.

|Ayar veya seçenek|Önerilen ayar|
|---|---|
|Name|Etki alanındaki tüm alıcılar için güvenli bağlantılar ilkesi|
|İletilerde bilinmeyen kötü amaçlı olabilecek URL 'Ler için eylemi seçin|**URL 'yi seçin-URL 'ler yeniden yazılır ve Kullanıcı bağlantıya tıkladığında bilinen kötü niyetli bir bağlantı listesine karşı denetlenir**.|
|İndirilebilir içeriği taramak için güvenli ekler kullanma|Bu kutuyu seçin.|
|Uygulanacak|Alıcı etki alanı. . . etki alanınızı seçin.|

Daha fazla bilgi için [Office 365 ATP güvenli bağlantılarına](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)bakın.

## <a name="go-to-intune-admin-center"></a>Intune yönetim merkezine gidin

1. [Azure portalında](https://portal.azure.com/)oturum açın.

2. **Tüm hizmetleri** seçin ve **Arama kutusuna** *Intune 'a* yazın.

3. Sonuçlar göründüğünde, **Microsoft Intune** 'un yanındaki Başlat 'ı seçerek bunu sık kullanılanlara koyun ve daha sonra kolayca bulabilirsiniz.

Yönetim merkezinin yanı sıra, kuruluşunuzun cihazlarını kaydettirmek ve yönetmek için Intune 'u kullanabilirsiniz. Daha fazla bilgi için, [Intune tarafından yönetilen cihazların](https://docs.microsoft.com/intune/enrollment-options)Windows cihazları ve kayıt seçenekleri [için kayıt yöntemine göre Capabilities](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) bölümüne bakın.
