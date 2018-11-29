---
title: Microsoft 365 iş CSP abonelik geçiş 
description: Önizleme bir Microsoft 365 iş CSP abonelik İST nasıl geçiş yapabileceğini öğrenmek Bul 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 iş, CSP abonelik Microsoft 365, SMB, geçiş
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982490"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 iş CSP abonelik geçiş

Bir Microsoft 365 iş Önizleme CSP aboneliğiniz varsa, varolan Microsoft 365 iş GA (genel kullanılabilirlik) önizleme aboneliğini nasıl geçiş yapabileceğini öğrenmek bulmak için bu kılavuzu izleyin.

**GA Önizleme aboneliğine geçiş yapma**

1. <a href="https://partnercenter.microsoft.com" target="_blank">Ortağı merkezi</a>oturum açın.
2. Panosundan **Müşteriler**, seçin ve bulmak ve şirket adını seçin.

    Bir şirket için abonelikleri listelenecektir.

    ![Ortağı Merkezi'nde müşterinin abonelikleri](images/pc_customer_subscriptions_1.png)
    
3. Şirketin **abonelikleri** sayfasında, **Abonelik Ekle**seçin.
4. **Yeni Abonelik** sayfası, **küçük işletme** seçin ve sonra **Microsoft 365 iş** listeden seçin.
5. Lisans sayısını ekleyin ve sonra seçin **Sonraki: gözden** abonelik gözden geçirin ve sonra **Gönder**' i seçin.

    ![Yeni Abonelik Microsoft 365 iş için gözden geçirin.](images/pc_customer_reviewnewsubscription.png)

    **Abonelik lisansı tabanlı** **Microsoft 365 iş Önizleme** ve **Microsoft 365 iş**gösterir. Önizleme abonelik sonraki askıya gerekecek.

6. **Microsoft 365 iş Önizleme'yi**seçin.
7. **Microsoft 365 iş Önizleme** sayfasında önizleme abonelik askıya almak için **Beklemede** seçeneğini seçin.

    ![Microsoft 365 iş Önizleme abonelik askıya alma](images/pc_customer_m365bpreview_suspend.png)

8. Onaylamak için **Gönder** ' i seçin.

    **Abonelikleri** sayfasında **Microsoft 365 iş Önizleme** durumu **Beklemede**gösterir onaylayın.

    ![Önizleme abonelik durumunu askıya Onayla](images/pc_customer_m365bpreview_suspend_confirm.png)

9. İsteğe bağlı olarak, Lisans Sözleşmesi'ni de doğrulayabilirsiniz. Bunu yapmak için şu adımları izleyin:
    1. **Kullanıcılar ve lisansları** şirketin **Subscriptions** sayfasını seçin.
    2. **Kullanıcılar ve lisansları** sayfasından bir kullanıcı seçin.
    3. Kullanıcının sayfasında, **lisansları atama** bölümüne bakın ve **Microsoft 365 iş**gösterdiğini doğrulayın.

        ![Microsoft 365 işletme lisansı kullanıcıya atanan Onayla](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Müşteriler ve kullanıcılara sırasında ve sonrasında geçiş etkisi

Geçiş ve posta geçişi sırasında müşteriler ve kullanıcılara etkisi yoktur.

## <a name="impact-to-customers-who-dont-transition"></a>Geçiş yok müşterilere etkisi

Aşağıdaki tablo Microsoft 365 iş Önizleme abonelikten Microsoft 365 iş aboneliğine geçiş olmayan müşterilere etkisini özetlemektedir.

|       | T-0 T + 30     | T + T + 60 30 | T + T + 120 60 | T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Durum** | Yetkisiz kullanım süresi içinde | Süresi dolmuş      | Devre dışı      | Deprovisioned |
| **Hizmet etkileri**                                                        |
| **Microsoft 365 iş Yönetim Portalı** | İşlev etkisi | İşlev etkisi | Kullanıcı Ekle/Sil, abonelik satın alın.</br> Ata/lisansları iptal edilemez. | Müşterinin aboneliğine ve tüm veriler silinir. Admin diğer Ücretli aboneliklerin yönetebilirsiniz. |
| **Office uygulamaları**                         | Son kullanıcı etkisi | Son kullanıcı etkisi | Office, sınırlı işlevsellik moduna girer.</br> Kullanıcılar yalnızca dosyaları görüntüleyebilir. | Office, sınırlı işlevsellik moduna girer.</br> Kullanıcılar yalnızca dosyaları görüntüleyebilir. |
| **Bulut Hizmetleri (SharePoint çevrimiçi Exchange Online, Skype, takımlar ve daha fazla)** | Son kullanıcı etkisi | Son kullanıcı etkisi | Son kullanıcılar ve Yöneticiler için veri buluta erişiminiz yok. | Müşterinin aboneliğine ve tüm veriler silinir. |
| **EM + S bileşenleri** | Admin etkisi</br> Son kullanıcı etkisi | Admin etkisi</br> Son kullanıcı etkisi | Yeteneği yürütülebilmesi durduracak.</br> [Mobil aygıt üzerinde abonelik süresini etkiler](#mobile-device-impacts-upon-subscription-expiration) ve [Windows 10 PC etkileri abonelik sona erme üzerine](#windows-10-pc-impacts-upon-subscription-expiration) daha fazla bilgi için bkz. | Yeteneği yürütülebilmesi durduracak.</br> [Mobil aygıt üzerinde abonelik süresini etkiler](#mobile-device-impacts-upon-subscription-expiration) ve [Windows 10 PC etkileri abonelik sona erme üzerine](#windows-10-pc-impacts-upon-subscription-expiration) daha fazla bilgi için bkz. |
| **Windows 10 iş** | Admin etkisi</br> Son kullanıcı etkisi | Admin etkisi</br> Son kullanıcı etkisi | Yeteneği yürütülebilmesi durduracak.</br> [Mobil aygıt üzerinde abonelik süresini etkiler](#mobile-device-impacts-upon-subscription-expiration) ve [Windows 10 PC etkileri abonelik sona erme üzerine](#windows-10-pc-impacts-upon-subscription-expiration) daha fazla bilgi için bkz. | Yeteneği yürütülebilmesi durduracak.</br> [Mobil aygıt üzerinde abonelik süresini etkiler](#mobile-device-impacts-upon-subscription-expiration) ve [Windows 10 PC etkileri abonelik sona erme üzerine](#windows-10-pc-impacts-upon-subscription-expiration) daha fazla bilgi için bkz. |
| **Bir Windows 10 PC Azure AD oturum açma** | Admin etkisi</br> Son kullanıcı etkisi | Admin etkisi</br> Son kullanıcı etkisi | Admin etkisi</br> Son kullanıcı etkisi | Kiracı silinirse, kullanıcı yalnızca yerel kimlik bilgilerinizle oturum açabilirsiniz. Yerel kimlik bilgileri varsa, aygıtı yeniden görüntü. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobil aygıt abonelik sona erme üzerine etkileri

Mobil cihazlarda uygulama yönetimi ilkeleri etkisini followint tabloda özetlenmiştir.

|                            | Tam lisanslı deneyimi                      | T + 60 gün sonrası süre sonu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Çalışma dosyaları etkin olmayan bir aygıttan sil** | Çalışma dosyaları gün seçtikten sonra kaldırılır. | Kullanıcının kişisel aygıtlarında çalışma dosyaları kalır |
| **Tüm kullanıcıları, iş dosyalarını OneDrive İş üzerine kaydetmeye zorlama** | Çalışma dosyaları yalnızca OneDrive iş için kaydedilebilir | Herhangi bir iş dosyaları kaydedilebilir |
| **İş dosyalarını şifrele** | Çalışma dosyaları şifreli | Artık iş dosyalar şifrelenir.</br> Güvenlik ilkeleri kaldırılır ve Office apps verileri kaldırılır. |
| **Office uygulamaları erişmek için parmak izi ya da PIN iste** | Sınırlı erişim için apps | Uygulama düzeyinde erişimi kısıtlama |
| **Oturum açma başarısız olduğunda PIN'i Sıfırla** | Sınırlı erişim için apps | Uygulama düzeyinde erişimi kısıtlama |
| **Kullanıcıların Office apps boşta sonra yeniden oturum açmanız gerekir** | Gerekli oturumaçma | Hiçbir oturum-apps erişmek için gerekli ' |
| **İşletim sistemi kısıtlamaları kaldırılmış veya kök erişim izni verilmiş cihazlardan iş dosyalarına erişilmesini engelle** | Çalışma dosyaları jailbroken ve kök aygıtlarda erişilemiyor | Çalışma dosyaları jailbroken ve kök aygıtlarda erişilebilir |
| **Kullanıcıların kişisel apps için Office uygulamaları içerik kopyalama** | Kopyala/yapıştır sınırlı uygulamaları için Microsoft 365 İş Abonelik bir parçası olarak | Kopyala/yapıştır tüm uygulamalar için kullanılabilir |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC üzerinde abonelik süresini etkiler.

Aşağıdaki tabloda Windows 10 aygıt yapılandırma ilkeleri etkisini özetlemektedir.

|                            | Tam lisanslı deneyimi                      | T + 60 gün sonrası süre sonu          |
|----------------------------|------------------------------------------------|------------------------------------|
| **PC'ler, Windows Defender'ı kullanma tehditlerinden korunmasını sağlayın** | Kullanıcı denetimi dışında sıranız açık/kapalı | Kullanıcı Windows 10 PC'de Windows Defender açık/kapalı devre |
| **Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol** | Microsoft Edge PC koruma | Kullanıcı Microsoft Edge PC koruma açık/kapalı devre |
| **Boşta iken aygıt ekranı Kapat** | Ekran zaman aşımı aralığı İlkesi Admin tanımlar | Ekran zaman aşımı son kullanıcı tarafından yapılandırılması |
| **Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver** | Bir kullanıcı Microsoft Store apps yükleyebilirsiniz Admin tanımlar | Kullanıcı apps Microsoft Store istediğiniz zaman yükleyebilirsiniz |
| **Kullanıcıların Cortana'ya erişmesine izin ver** | Yönetim İlkesi kullanıcı erişimini Cortana tanımlar. | Aç / Kapat Cortana için kullanıcı aygıtları |
| **Kullanıcıların Microsoft'tan ipuçları ve reklam izin ver** | Admin kullanıcı ilkesi tanımlar Microsoft'tan ipuçları ve reklamlar | Kullanıcı, açık/kapalı ipuçları ve Microsoft'tan reklam kapatabilir |
| **Kullanıcıların Office uygulamalarından kişisel uygulamalara içerik kopyalamasına izin ver** | Yönetim ilkesi Windows 10 aygıtları güncel tutmak için tanımlar. | Kullanıcılar Windows güncelleştirme zamanına karar verebilirsiniz |




