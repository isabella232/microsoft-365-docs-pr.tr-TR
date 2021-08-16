---
title: Algılanan tehditleri gözden geçirme ve önlem alma
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Mobil cihazlarınıza güvenlik tarafından algılanan tehditleri Microsoft Defender Virüsten Koruma ve yönetmeyi Windows 10 öğrenin.
ms.openlocfilehash: f2edd27c527cc2b9fd8c986191a0bad5c0844da68880f8d8d775491e3480babd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53882103"
---
# <a name="review-detected-threats-and-take-action"></a>Algılanan tehditleri gözden geçirme ve önlem alma

Kötü amaçlı bir dosya veya yazılım algılandığında, Microsoft Defender Virüsten Koruma bu dosyayı engeller ve çalıştırmasını engeller. Bulut teslimi koruması açıksa, virüsten koruma ve kötü amaçlı yazılımdan koruma altyapısına yeni algılanan tehditler eklenir ve böylelikle diğer cihazlarınız ve kullanıcılarınız da korunur.

Microsoft Defender Virüsten Koruma tehditlere karşı şunları algılar ve korur:

- Virüsler, kötü amaçlı yazılımlar ve cihazlara yönelik web tabanlı tehditler
- Kimlik avı girişimleri
- Veri hırsızlığı girişimleri

Bir IT uzmanı/yöneticisi olarak, aynı anda [intune'a Windows 10](/mem/intune/enrollment/device-enrollment) cihazlarında tehdit algılamaları ile ilgili bilgileri Microsoft 365 yönetim merkezi. Aşağıdakiler gibi özet bilgileri burada görüyorsunuz:

- Virüsten koruma yazılımına ihtiyaç kaç cihaz gerekiyor?
- Kaç cihaz güvenlik ilkeleriyle uyumlu değil
- Şu anda etkin, risk azaltmaya yönelik veya çözümlenmiş durumda kaç tehdit var

Tehdit algılamaları ve cihazlar hakkında belirli bilgileri görüntülemek için çeşitli seçenekleriniz vardır:

- Sayfanın **Etkin** cihazlar <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 yönetim merkezi.</a> Bu [makalenin Etkin cihazlarda tehdit algılamalarını yönetme](#manage-threat-detections-on-the-active-devices-page) sayfasına bakın.
- Sayfanın **üzerinde** Etkin tehdit <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 yönetim merkezi.</a> Bu [makalenin Etkin tehdit algılamalarını yönetme sayfasındaki](#manage-threat-detections-on-the-active-threats-page) Tehdit algılamalarını yönetme makalesine bakın.
- 'da Virüsten <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Koruma Microsoft Endpoint Manager.</a>  Bu [makaledeki Yeni E-posta Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) algılamalarını yönetme makalesine bakın.

Daha fazla bilgi için bkz. [Güvenlik tarafından algılanan Microsoft Defender Virüsten Koruma.](threats-detected-defender-av.md)

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Etkin cihazlar sayfasında tehdit **algılamalarını** yönetme

Aşağıdaki yordam, iş veya hizmet Microsoft 365 İş Ekstra.

1. Oturum Microsoft 365 yönetim merkezi <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> gidin.

2. Gezinti sayfasında Cihazlar Etkin **cihazlar'ı**  >  **seçin.** Koruma durumu, virüsten koruma (AV) koruma durumu ve algılanan etkin tehdit sayısı gibi etkin cihazların ve ayrıntıların listesini görüntülenir.

3. Bir cihaz ve kullanılabilir eylemler hakkında daha fazla ayrıntı görüntülemek için o cihazı seçin. Öneriler ve İlkeyi güncelleştir, Virüsten koruma yazılımını **güncelleştir,** Hızlı tarama **çalıştır,** Tam tarama çalıştır ve daha fazlası gibi eylemlerin yer olduğu **bir** açılır pencere açılır. 

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Etkin tehdit sayfasında tehdit **algılamalarını** yönetme

Aşağıdaki yordam, iş veya hizmet Microsoft 365 İş Ekstra. [Windows 10 güvenli olmalı ve](./secure-win-10-pcs.md) [Intune'a kaydolmaları gerekir.](/mem/intune/enrollment/windows-enrollment-methods)

> [!NOTE]
> Yeni **Microsoft Defender Virüsten Koruma** ve Etkin  tehdit sayfası aşamalar içinde yuvarlanıyor, dolayısıyla bu karta hemen erişiminiz yok olabilir.

1. Oturum Microsoft 365 yönetim merkezi <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> gidin.

2. Güvenlik **kartında Microsoft Defender Virüsten Koruma** tehditleri **görüntüle'yi seçin.** (Alternatif olarak, gezinti bölmesinde Durum'ı **seçin**  >  **Tehdit & virüsten koruma**.)

3. Etkin **tehditler sayfasında,** bu konuda daha fazla bilgi edinmek için algılanan bir tehdit seçin. Bu tehditle ilgili ayrıntıların ve etkilenen cihazların bulunduğu bir açılır pencere açılır.

4. Çıkışta, İlkeyi güncelleştir , Virüsten koruma **güncelleştirme,** Hızlı taramayı çalıştır ve daha fazlası gibi kullanılabilir eylemleri görüntülemek  **için** bir cihaz seçin.

## <a name="actions-you-can-take"></a>Gerçekleştir işlemler

Belirli tehdit veya cihazlarla ilgili ayrıntıları görüntüde, önerileri ve gerçekleştirebilirsiniz. Aşağıdaki tabloda, gördüğünüz eylemler açık almaktadır.<br><br>

| Eylem | Açıklama |
|--|--|
| Korumayı yapılandırma | Tehdit koruması ilkelerinizin yapılandırılması gerekir. İlke yapılandırma sayfanıza gitmek için bağlantıyı seçin.<br><br>Yardıma mı ihtiyacınız var? Bkz. [Microsoft Intune'da uç nokta güvenlik ilkeleriyle cihaz Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| İlkeyi güncelleştirme | Virüsten koruma ve gerçek zamanlı koruma ilkelerinizin güncelleştirilmiş veya yapılandırılmış olması gerekir. İlke yapılandırma sayfasına gitmek için bağlantıyı seçin.<br><br>Yardıma mı ihtiyacınız var? Bkz. [Microsoft Intune'da uç nokta güvenlik ilkeleriyle cihaz Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| Hızlı taramayı çalıştırma | Cihazda hızlı bir virüsten koruma taraması başlatır, kayıt defteri anahtarları ve bilinen veya başlangıç klasörleri gibi kötü amaçlı yazılımların kaydedildiği yaygın Windows odaklanarak. |
| Tam taramayı çalıştır | Cihazda tam virüsten koruma taraması başlatır, kötü amaçlı yazılımların kaydedil olduğu yaygın konumlara odaklanarak ve cihaza her dosya ve klasörü dahil edin. Sonuçlar [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Virüsten koruma yazılımını güncelleştirme | Virüsten koruma ve kötü [amaçlı yazılımlardan koruma için](https://go.microsoft.com/fwlink/?linkid=2149926) güvenlik zekası güncelleştirmelerini almak için cihazı gerektirir. |
| Cihazı yeniden başlat | Bir Windows 10 dakika içinde yeniden başlatılmasını gerektirir.<br><br>**ÖNEMLİ:** Cihaz sahibine veya kullanıcıya yeniden başlatma işlemi otomatik olarak bildirilir ve bu, kaydedilirken yapılan çalışmaları kaybedebilir. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Tehdit algılamalarını yeni Microsoft Endpoint Manager

Tehdit algılamalarını Microsoft Endpoint Manager için bu özelliği kullanabilirsiniz. Windows 10 Cihazlar [Intune'a (diğer bir](/mem/intune/enrollment/windows-enrollment-methods) parçası) Microsoft Endpoint Manager.

1. Microsoft Endpoint Manager yönetim merkezine gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> ve oturum açma.

2. Gezinti bölmesinde Uç nokta güvenliği **öğesini seçin.**

3. Yönet altında **Virüsten** Koruma öğesini **seçin.** Özet, Sağlıksız uç noktalar ve **kötü** **amaçlı yazılım Windows 10** gibi Windows 10 **sekmeler vardır.**

4. Kullanılabilir sekmelerde yer alan bilgileri gözden geçirin ve sonra gerekli eylemi yapın.

Örneğin, cihazların kötü amaçlı yazılım algılandı **sekmesinde Windows 10 olduğunu varsayalım.** Bir cihaz seçin; Yeniden Başlat , Hızlı **Tarama,** Tam **Tarama,** Eşitle **veya** İmzaları güncelleştir **gibi** bazı **eylemleri gerçekleştirebilirsiniz.** Bu cihaz için bir eylem seçin.

Aşağıdaki tabloda, e-Microsoft Endpoint Manager.<br><br>

| Eylem | Açıklama |
|--|--|
| Yeniden Başlat | Bir Windows 10 dakika içinde yeniden başlatılmasını gerektirir.<br><br>**ÖNEMLİ:** Cihaz sahibine veya kullanıcıya yeniden başlatma işlemi otomatik olarak bildirilir ve bu, kaydedilirken yapılan çalışmaları kaybedebilir. |
| Hızlı Tarama | Cihazda hızlı bir virüsten koruma taraması başlatır, kayıt defteri anahtarları ve bilinen veya başlangıç klasörleri gibi kötü amaçlı yazılımların kaydedildiği yaygın Windows odaklanarak. Sonuçlar [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Tam Tarama | Cihazda tam virüsten koruma taraması başlatır, kötü amaçlı yazılımların kaydedil olduğu yaygın konumlara odaklanarak ve cihaza her dosya ve klasörü dahil edin. Sonuçlar [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Eşitle | Intune ile birlikte (uygulamanın bir parçası) iade etmek için bir cihaz Microsoft Endpoint Manager. Cihaz iade geldiğinde, cihaza atanmış bekleyen eylemleri veya ilkeleri alır. |
| İmzaları güncelleştirme | Virüsten koruma ve kötü [amaçlı yazılımlardan koruma için](https://go.microsoft.com/fwlink/?linkid=2149926) güvenlik zekası güncelleştirmelerini almak için cihazı gerektirir. |

> [!TIP]
> Daha fazla bilgi için [bkz. Cihazlar için uzak eylemler](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices).

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Kötü amaçlı yazılım çözümlemesi için dosya gönderme

Kaçırılmış olduğunu ya da yanlış olarak kötü amaçlı yazılım olarak sınıflandırılmış olduğunu bildiğiniz bir dosyanız varsa, kötü amaçlı yazılım çözümlemesi yapmak için bu dosyayı Microsoft'a gönderebilirsiniz. Kullanıcılar ve IT yöneticileri çözümleme için dosya gönderebilirsiniz. 'ı ziyaret [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) edin.