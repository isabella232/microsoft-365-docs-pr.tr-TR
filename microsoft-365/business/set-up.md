---
title: Microsoft 365 Business Premium 'u ayarlama
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Etki alanı ve Kullanıcı ekleme, güvenlik ilkelerini ayarlama gibi Microsoft 365 Iş ekstra için kurulum adımlarını keşfedin.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324506"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Kurulum sihirbazında Microsoft 365 Business Premium 'u ayarlama

Microsoft 365 Business Premium kurulumuna genel bir bakış için bu videoyu izleyin.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>Etki alanınızı, kullanıcılarınızı ve kurulum ilkelerini ekleme

Microsoft 365 Business Premium satın aldığınızda, sahip olduğunuz bir etki alanını kullanma veya [kayıt](sign-up.md)sırasında satın alma seçeneğiniz vardır.

- Kaydolduğunuzda yeni bir etki alanı satın aldıysanız, etki alanınızın tümü ayarlanır ve [Kullanıcı ekleme ve lisans atama](#add-users-and-assign-licenses)'ya taşıyabilirsiniz.

### <a name="add-your-domain-to-personalize-sign-in"></a>Kişiselleştirme oturum açma

1. Genel yönetici kimlik bilgilerinizi kullanarak [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com) 'nde oturum açın. 

2. Sihirbazı başlatmak için **Kuruluma git** 'i seçin.

    ![Kuruluma git 'i seçin.](../media/gotosetupinadmincenter.png)

3. **Office uygulamalarınızı yükleyin** sayfasında isteğe bağlı olarak uygulamaları kendi bilgisayarınıza yükleyebilirsiniz.
    
4. **Etki alanı Ekle** adımında, kullanmak istediğiniz etki alanı adını girin (contoso.com gibi).

    > [!IMPORTANT]
    > Kayıt sırasında bir etki alanı satın aldıysanız, burada **etki alanı adımı ekle** seçeneğini görmezsiniz. Bunun yerine [Kullanıcı ekleme](#add-users-and-assign-licenses) bölümüne gidin.

    ![Oturum açma sayfanızı kişiselleştirin sayfasının ekran görüntüsü.](../media/adddomain.png)

    
4. [Microsoft 365 için herhangi BIR DNS barındırma sağlayıcısında](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) etki alanının sahibi olduğunuzu doğrulayan DNS kayıtlarını oluşturmak için sihirbazdaki adımları izleyin. Etki alanı konağını biliyorsanız, ayrıca [ana bilgisayara özgü yönergelere](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)bakın.

    Barındırma sağlayıcınız GoDaddy veya [etki alanı Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)ile başka bir ana bilgisayar etkinleştirilmişse, süreç kolaydır ve oturum açmanız ve Microsoft.

    ![GoDaddy erişimini Onayla sayfasında Yetkilendir 'i seçin.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Kullanıcı ekleme ve lisans atama

Sihirbazda kullanıcı ekleyebilirsiniz, ancak bunları [daha sonra](add-users-m365b.md) Yönetim merkezinde ekleyebilirsiniz. Ayrıca, yerel bir etki alanı denetleyiciniz varsa, [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ile kullanıcı ekleyebilirsiniz.

#### <a name="add-users-in-the-wizard"></a>Sihirbazda Kullanıcı ekleme

Sihirbaza eklediğiniz tüm kullanıcılara otomatik olarak Microsoft 365 Business Premium Lisansı atanır.

![Sihirbazdaki yeni kullanıcılar Ekle sayfasının ekran görüntüsü](../media/addnewuserspage.png)

1. Microsoft 365 Business Premium aboneliğiniz var olan kullanıcılara sahipse (örneğin, Azure AD Connect kullandıysanız), onlara şimdi lisans atama seçeneğini kullanabilirsiniz. Bu kullanıcılara da lisans ekleyerek işleme devam edin.

2. Kullanıcıları ekledikten sonra, eklediğiniz yeni kullanıcılarla kimlik bilgilerini paylaşma seçeneği de alırsınız. Bunları yazdırabilir, e-posta ile gönderebilir veya indirebilirsiniz.

### <a name="connect-your-domain"></a>Etki alanınızı bağlama

> [!NOTE]
> Kullanıcıları ayarlamak için. adımmicrosoft etki alanını kullanmayı seçtiyseniz veya Azure AD Connect 'i kullandıysanız, bu adımı görmezsiniz.
  
Hizmetleri ayarlamak için DNS ana bilgisayarınızda veya etki alanı kayıt şirketinizde bazı kayıtları güncelleştirmeniz gerekir.
  
1. Kurulum sihirbazı, genellikle kayıt şirketinizi algılar ve kayıt şirketinin web sitesinde NS kayıtlarınızı güncelleştirmek için adım adım yönergelere ulaşabileceğiniz bir bağlantı verir. Desteklemiyorsa, [ad sunucularını değiştirerek etki alanı kayıt kaydediciyle Microsoft 365 'i ayarlayın](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Var olan bir Web sitesi gibi DNS kayıtlarınız varsa ancak DNS ana bilgisayarı [etki alanı bağlantısı](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)için etkinleştirilmişse, **benim için kayıt Ekle**'yi seçin. **Çevrimiçi hizmetler 'ı seçin** sayfasında tüm varsayılanları kabul edin ve ileri 'Yi ve **ardından**DNS ana bilgisayarınızın sayfasında **Yetkilendir** 'i seçin.
    - Başka DNS ana bilgisayarlarıyla (etki alanı bağlantısı için etkinleştirilmemiş) DNS kayıtlarınız varsa, var olan hizmetlerin bağlı kalmasını sağlamak için kendi DNS kayıtlarınızı yönetmek isteyeceksiniz. Daha fazla bilgi için [etki alanı temel](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) bilgilerine bakın.

        ![Kayıtları etkinleştir sayfası.](../media/activaterecords.png)

2. Sihirbazdaki ve e-postadaki adımları izleyin ve diğer hizmetler sizin için ayarlanır.

### <a name="protect-your-organization"></a>Kuruluşunuzu koruma 

Sihirbazda ayarladığınız ilkeler, *tüm kullanıcılar*adındaki bir [güvenlik grubuna](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) otomatik olarak uygulanır. Yönetim merkezinde ilke atamak için ek gruplar da oluşturabilirsiniz.

1. **Gelişmiş siber tehditlerden korunma koruması**üzerinde, [Office 365 öncelikli tehdit koruması](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Office uygulamalarında dosya ve bağlantıları taratmak için varsayılanları kabul etmeniz önerilir.

    ![Korumayı arttır sayfasının ekran görüntüsü.](../media/increasetreatprotection.png)


2. **Hassas verileri sızıntıları önle** sayfasında, Office uygulamalarında hassas verileri izlemek ve kuruluşunuzun dışından bunları yanlışlıkla paylaşmayı önleyen Office 365 veri kaybı önleme (DLP) özelliğini açmak için varsayılanları kabul edin.

3. **Mobil Için Office 'te verileri koruyarak** sayfasında mobil uygulama yönetimi 'nden çıkın, ayarlar 'ı genişletin ve ardından **mobil uygulama yönetim ilkesi oluştur**'u seçin.

    ![Mobil için Office 'te verileri korumama ekran görüntüsü.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10 bilgisayarlarında güvenli

Sol gezintide, **Kurulum 'u** seçin ve ardından **oturum açma ve güvenlik**altında **Windows 10 bilgisayarlarınızı güvenli**'ı seçin. Başlamak için **görüntüle** 'yi seçin. Tüm yönergeler için [Windows 10 bilgisayarlarınızın güvenliğini sağlama](secure-win-10-pcs.md) konusuna bakın.

## <a name="deploy-office-365-client-apps"></a>Office 365 istemci uygulamalarını dağıtma

Kurulum sırasında Office uygulamalarını otomatik olarak yüklemeyi seçtiyseniz, kullanıcılar Windows cihazlarında Azure AD 'de oturum açtıktan sonra iş kimlik bilgilerini kullanarak uygulamalar Windows 10 aygıtlarına yüklenir.

Office 'i mobil iOS veya Android cihazlarda yüklemek için, [Microsoft 365 Business Premium kullanıcıları için mobil cihazları ayarlama](set-up-mobile-devices.md)bölümüne bakın.

Ayrıca Office 'i tek tek da yükleyebilirsiniz. Yönergeler için [PC veya Mac 'e Office yükleme](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) konusuna bakın.

## <a name="see-also"></a>Ayrıca bkz.

[Microsoft 365 iş eğitim videoları](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
