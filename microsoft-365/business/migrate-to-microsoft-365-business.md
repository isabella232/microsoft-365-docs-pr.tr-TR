---
title: Office 365 Business Premium'dan Microsoft 365 Business'a yükseltme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: İşletmenizi Office 365 Business Premium'dan Microsoft 365 Business'a yükselten adımlar.
ms.openlocfilehash: 95c4504d7e6e33bdededee0cfca7add0cb5f7204
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640571"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a>Office 365 Business Premium'dan Microsoft 365 Business'a yükseltme

İş aboneliği için bir [Office 365'iniz](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)varsa (örneğin, Office 365 Business Premium), Microsoft 365 Business'a kolayca yükseltebilirsiniz. Eklemek isterseniz Microsoft 365 Business'a yükseltin: 
- Windows 10 Pro (Windows 8 veya sonraki çalıştıran bilgisayarlarına)
- Aygıtlarda iş verilerini yöneten basit denetimler
- Gelişmiş güvenlik yetenekleri.
[Microsoft.com'da](https://www.microsoft.com/microsoft-365/business) Microsoft 365 Business hakkında daha fazla bilgi edinin

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a>Office 365 Business Premium ile Microsoft 365 Business arasındaki fark nedir?
Bu iki planın yan yana karşılaştırmasını [Microsoft 365 İş Hizmeti Açıklaması'na](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)ekledik. 

## <a name="before-you-get-started"></a>Başlamadan önce

- **Yükseltmeyi ne zaman seçmeliyim?** Yükseltme, tek bir plana atanan **tüm kullanıcıları** yükseltmek istediğinizde doğru seçimdir. Yükseltmeyi seçtiğinizde, tüm plan kullanıcıları aynı anda başka bir plana geçer. Tek bir plana atanan herkesi yükseltmek istemiyorsanız, yeni plan için lisans satın alın (bu durumda Microsoft 365 Business) ve bu lisansları yükseltmek istediğiniz her kullanıcıya [ayrı ayrı atayın.](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) 
- **Bazı eklentiler yükseltmeyi engelleyebilir** Bir yükseltme başlatmaya çalışırsanız ve devam etmenizi engelleyen bir eklentiniz varsa, önce eklentiyi kaldırabilir ve daha sonra gerekirse yeniden ekleyebilirsiniz. 
- **Planınızı ön ödemeniz varsa** Ön ödemeli planlar için basit bir yükseltme yolu yoktur. Planınızı bir mağazadan satın almış olabileceğiniz bir ürün kimliği kullanarak ayarladığınızdan ön ödemeli bir planınız olup olmadığını anlarsınız. Bir iş ortağına başvurun, Microsoft Mağazası'na gidin veya yeni bir plana geçmek için ön ödemeli planınızın süresinin dolmasını bekleyin.

## <a name="upgrade-to-microsoft-365-business"></a>Microsoft 365 Business'a yükseltme
[Yeni yönetici merkezinde](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)aşağıdaki adımları izleyerek lisanslarınızı satın alın:
1. 'de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine giriş
2. Gezinti bölmesine gidin ve **Faturalama** \> Ürünleri **& Hizmetleri'ni**seçin. Office 365 aboneliğinizi bulun ve ayrıntıları görüntülemek için bu aboneliği seçin. 

    ![Ekran görüntüsü, yönetici merkezinde aboneliğinizi nasıl bulabileceğinizi ve seçileceksiniz.](media/FindYourSubscription.png)

3. Sonraki sayfada **Yükseltme'yi**seçin. 

      ![Ekran görüntüsü, yönetici merkezinde Yükseltme'nin nerede seçilen olduğunu gösterir.](media/SelectUpgrade.png)

  > [!NOTE]
  > **Aboneliğinizi Yükseltmenin Azure Active Directory'de grup tabanlı lisanslamayla desteklenmediğini**belirten bir ileti görürseniz, çok büyük bir kuruluşunuz yoksa bunu güvenle göz ardı edebilirsiniz. Bu seçeneği seçen kuruluşlar, grup tabanlı lisanslama kullandıklarının farkında olurlar.

4. Ardından, yükseltebileceğiniz Office planlarının listesini görüntüleyebilirsiniz. Bu durumda, Microsoft 365 İş planını bulun. Bu plana dahil olan tüm Office uygulamalarını ve hizmetlerini görmek istiyorsanız aşağı kaydırabilirsiniz. **Microsoft 365 Business**altında, microsoft 365 Business'ı sepetinize eklemek için **Yükseltme'yi** seçin.
5. Arabada:
    1. Tüm mevcut kullanıcılarınız için otomatik olarak lisansları dahil edeceğiz. Daha fazla veya daha az lisansa ihtiyacınız varsa, [bu lisansları tek tek satın almanız ve atamalısınız.](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)  
    2. Aylık veya yıllık ödeme yapmak istediğiniz ibareleri ayarlayabilirsiniz. Seçiminizi yapmak için açılır menüyü seçin.
6. Bu hesabın ödeme yöntemi de dahil olmak üzere satın alma işleminizin özetini göreceğiniz **Kullanıma Git'i** seçin. Ayrıca varsa buraya bir promosyon kodu ekleyebilirsiniz.
7. Satın alma işlemini tamamlamak için **Sipariş'i Yerleştir'i** seçin.
Microsoft'un yeni hizmet planlarınızı ayarlaması birkaç dakika sürer. İlerlemeyi denetlemek için **yükseltme durumunu denetle'yi**seçin. 
1. Planınız hazır olduğunda, yönetici merkezinde bazı ek kurulum adımlarını tamamlamanız gerekebilir. Gezinti bölmesinde, ek kurulum adımlarını tamamlamak için **Ana Sayfa'yı** seçin.

> [!NOTE]
> Artık ihtiyacınız olmayan Ofifce 365 lisansları için eşit olarak geri ödeme alırsınız. Yeni planı ayarladıktan yaklaşık iki gün sonra banka hesabınız veya kredi kartınızdan ücret tahsil edilecektir.
  
## <a name="protect-user-devices-and-files"></a>Kullanıcı cihazlarını ve dosyalarını koruma

Microsoft 365 İşletme lisansları atandığı için, aygıtları ve dosyaları korumaya başlamak için tüm adımları niçin tamamlayın. Yönetici merkezi gezinti bölmesinde yer alan bazı yeni seçenekleri kullanırsınız.
  
1. Yönetici merkezinde, gezinti bölmesinde AygıtLar **** \> **İlkeleri'ne**gidin.
    
2. Aygıt **ilkeleri** sayfasında **Ekle'yi**seçin.
    
3. **İlke Ekle** bölmesinde ilke ye bir ad verin (örneğin, çalışma dosyalarını koruyun) ve ardından açılan listeden bir **İlke türü** seçin. 
    
    Android ve iPhone aygıtlarının yanı sıra Windows 10'daki dosyaları korumak için uygulama ilkeleri ayarlayabilir ve şirkete ait Windows 10 aygıtları için aygıt yapılandırma ilkeleri ayarlayabilirsiniz. Ayrıntılar için aşağıdaki bağlantılara bakın:
    
  - [Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme](app-protection-settings-for-android-and-ios.md)
    
  - [Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme](protection-settings-for-windows-10-devices.md)
    
  - [Windows 10 bilgisayarların aygıt koruma ayarlarını ayarlama](protection-settings-for-windows-10-pcs.md)
    
  
4. İlkeleri ayarladıktan sonra, siz ve çalışanlarınız aygıtlar ayarlayabilirsiniz:
    
  - Windows aygıtlarınız Windows Pro Creator güncelleştirmesini zaten kullanmıyorsa, [bunları Windows Pro Creators Update'e yükseltmeniz](upgrade-to-windows-pro-creators-update.md)gerekir.
    
  - Bkz. Windows aygıtları için adımlar [için Microsoft 365 İş kullanıcıları için Windows aygıtları ayarlama.](set-up-windows-devices.md) 
    
  - Bkz. Android telefonlar ve iPhone'lar için adımlar için [Microsoft 365 Business kullanıcıları](set-up-mobile-devices.md) için mobil cihazlar ayarlama. 
