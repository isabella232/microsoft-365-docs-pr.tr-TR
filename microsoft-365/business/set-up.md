---
title: Microsoft 365 Business'ı ayarlama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Microsoft 365 Business'ı nasıl ayarlayın öğrenin.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831313"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Kurulum sihirbazında Microsoft 365 Business'ı ayarlama

Microsoft 365 İş kurulumuna genel bir bakış için bu videoyu izleyin.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Bu videoyu yararlı bulduysanız, [küçük işletmeler ve Microsoft 365'e yeni katılanlar için tam eğitim serisine](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)göz atın.

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanınızı, kullanıcılarınızı ekleyin ve ilkeler ayarlayın

[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Microsoft 365 Business'ı satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında bir etki alanı satın alma seçeneğiniz vardır.

- Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınız tamamen ayarlanmıştır ve [kullanıcı ekle'ye taşınabilir ve lisans atayabilirsiniz.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Oturum açma'yı kişiselleştirmek için etki alanınızı ekleyin

1. Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 yönetici merkezinde](https://admin.microsoft.com) oturum açın. 

2. Sihirbazı başlatmak **için kuruluma git'i** seçin.

    ![Kuruluma Git'i seçin.](media/gotosetupinadmincenter.png)

3. Office **uygulamalarınızı yükle** sayfasında, uygulamaları isteğe bağlı olarak kendi bilgisayarınıza yükleyebilirsiniz.
    
4. Etki **alanı ekle** adımında, kullanmak istediğiniz etki alanı adını girin (contoso.com gibi).

    > [!IMPORTANT]
    > Kayıt sırasında bir etki alanı satın aldıysanız, burada **bir etki alanı** adımı ekle'yi görmezsiniz. Bunun yerine [Kullanıcı Ekle'ye](#add-users-and-assign-licenses) gidin.

    ![Oturum açma sayfanızı Kişiselleştir'in ekran görüntüsü.](media/adddomain.png)

    
4. Etki alanına sahip olduğunuzu doğrulayan [Office 365 için herhangi bir DNS barındırma sağlayıcısında DNS kayıtları oluşturmak için](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) sihirbazdaki adımları izleyin. Etki alanı ana bilgisayarınızı tanıyorsanız, [ana bilgisayara özel yönergeler](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)de bakın.

    Barındırma sağlayıcınız GoDaddy veya etki [alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)yla etkin leştirilmiş başka bir ana bilgisayarsa, işlem kolaydır ve otomatik olarak oturum açmanız ve Microsoft'un sizin adınıza kimliğini belirlemesine izin vermeniz istenir.

    ![GoDaddy Access'i Onayla sayfasında Yetkilendirme'yi seçin.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Kullanıcı ekleme ve lisans atama

Sihirbaza kullanıcı ekleyebilirsiniz, ancak daha sonra yönetici merkezine [de ekleyebilirsiniz.](add-users-m365b.md) Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect'e](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)sahip kullanıcılar ekleyebilirsiniz.

#### <a name="add-users-in-the-wizard"></a>Sihirbaza kullanıcı ekleme

Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak microsoft 365 Business lisansı atanabilir.

![Sihirbazda yeni kullanıcı ekle sayfasının ekran görüntüsü](media/addnewuserspage.png)

1. Microsoft 365 Business aboneliğinizde mevcut kullanıcılar varsa (örneğin, Azure AD Connect'i kullandıysanız), şimdi onlara lisans atama seçeneğine sahip siniz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

2. Kullanıcıları ekledikten sonra, kimlik bilgilerini eklediğiniz yeni kullanıcılarla paylaşma seçeneği de alırsınız. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> .onmicrosoft etki alanını kullanmayı seçtiyseniz veya kullanıcıları ayarlamak için Azure AD Connect'i kullandıysanız, bu adımı görmezsiniz.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Yoksa, [office 365'i herhangi bir etki alanı kayıt şirketiyle ayarlamak için ad sunucularını değiştirin.](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2) 

    - Varolan DNS kayıtlarınız varsa, örneğin varolan bir web sitesi, ancak [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için DNS ana bilgisayarınız etkinse, benim için kayıt **ekle'yi**seçin. Çevrimiçi **hizmetleri seç** sayfasında, tüm varsayılanları kabul edin ve **Sonraki'ni**seçin ve DNS ana bilgisayarınızın sayfasında **Yetkilendirme'yi** seçin.
    - Diğer DNS ana bilgisayarlarıyla varolan DNS kayıtlarınız varsa (etki alanı bağlantısı için etkinleştirildi), varolan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek istersiniz. Daha fazla bilgi için [etki alanı temellerine](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bakın.

        ![Kayıtlar sayfasını etkinleştirin.](media/activaterecords.png)

2. Sihirbazve e-posta ve diğer hizmetler adımları izleyin sizin için ayarlanır.

### <a name="protect-your-organization"></a>Kuruluşunuzu koruyun 

Sihirbazda ayarladığınız *ilkeler, Tüm Kullanıcılar*adlı bir [Güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır. Ayrıca, yönetici merkezinde ilkeler atamak için ek gruplar oluşturabilirsiniz.

1. Gelişmiş **siber tehditlere karşı korumayı**artırın'da, Office [365 Önceden Tehdit Koruması'nın](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Office uygulamalarındaki dosyaları ve bağlantıları taramasına izin verme varsayılanlarını kabul etmeniz önerilir.

    ![Korumayı Artır sayfasının ekran görüntüsü.](media/increasetreatprotection.png)


2. Hassas **veri sayfasının sızıntılarını önlemede,** Office uygulamalarındaki hassas verileri izlemek ve bunların kuruluşunuz dışında yanlışlıkla paylaşılmasını önlemek için Office 365 Veri Kaybı Önleme'yi (DLP) açma varsayılanlarını kabul edin.

3. Mobil sayfa **için Office'teki verileri koru'da** mobil uygulama yönetimini bırakın, ayarları genişletin ve gözden geçirin ve ardından **mobil uygulama yönetimi ilkesi oluştur'u**seçin.

    ![Mobil sayfa için Office'teki verileri koruyun ekran görüntüsü.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Güvenli Windows 10 cd'leri

Sol daki gezinmede **Kurulum'u** seçin ve ardından **Sing-in ve security**altında Windows **10 bilgisayarlarınızı güvenli**olarak seçin. Başlamak için **Görünüm'u** seçin. Tam talimatlar için [Windows 10 bilgisayarlarınızı güvenli olarak](secure-win-10-pcs.md) görün.

## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamalarını dağıtma

Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar iş kimlik bilgilerini kullanarak Windows aygıtlarından Azure AD'ye oturum açtıktan sonra uygulamalar Windows 10 cihazlarına yüklenir.

Office'i mobil iOS veya Android cihazlara yüklemek [için](set-up-mobile-devices.md)bkz.

Office'i tek tek yükleyebilirsiniz. Talimatlar için [Office'i pc'ye veya Mac'e yükleyin'](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) e bakın.

## <a name="see-also"></a>See also

[Microsoft 365 İş eğitim videoları](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
