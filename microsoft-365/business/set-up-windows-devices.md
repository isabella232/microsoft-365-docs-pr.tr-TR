---
title: Mobil Windows cihazları Microsoft 365 İş Ekstra ayarlama
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Kullanıcı Windows çalışan Windows 10 Pro cihazlarını Microsoft 365 İş Ekstra ve merkezi yönetim ve güvenlik denetimlerini etkinleştirebilirsiniz.
ms.openlocfilehash: 0a38a244ca997cfadb46c3833c0587e0c4f79fe3d32b90c6d92f08069b352bd3
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837870"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Mobil Windows cihazları Microsoft 365 İş Ekstra ayarlama

## <a name="before-you-begin"></a>Başlamadan önce

Microsoft 365 İş Ekstra için Windows cihazları ayarlamadan önce tüm Windows 1703 sürümü (Creators Update) Windows 10 Pro çalıştıran cihazlardan emin olun. Windows 10 Pro, Windows 10 Business'i tamamlayıcı nitelikte olan ve Windows 10 Pro'un merkezi yönetim ve güvenlik denetimlerini etkinleştiren bulut hizmetleri ve cihaz yönetimi özellikleri kümesi olan Microsoft 365 İş Ekstra.
  
Windows 7 Windows, Pro, Windows 8 Pro veya Windows 8.1 Pro çalıştıran Microsoft 365 İş Ekstra cihazlarınız varsa, Microsoft 365 İş Ekstra aboneliğiniz size Windows 10 verir.
  
Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltme hakkında daha fazla bilgi için bu konudaki adımları izleyin: [Windows cihazları Windows Pro Creators Update sürümüne yükseltme](upgrade-to-windows-pro-creators-update.md).
  
Yükseltmeye [sahip olduğunuzdan emin olmak veya yükseltmenin](#verify-the-device-is-connected-to-azure-ad) çalıştığını doğrulamak için bkz. Cihazın Azure AD'ye bağlı olduğunu doğrulama.

## <a name="watch-connect-your-pc-to-microsoft-365-business"></a>İzle: Bağlan İş'e Microsoft 365 izleyin

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Kuruluşunuzun Azure AD'sine Windows 10 cihazlarını ekleme

Tüm Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltildikten sonra veya Windows 10 Pro Creators Update'i zaten çalıştırıyorsa, bu cihazları kuruluş kuruluşlarının Azure Active Directory. Cihazlar katıldıktan sonra, otomatik olarak Microsoft 365 İş Ekstra aboneliğinizin bir parçası olan Windows 10 Business'e Microsoft 365 İş Ekstra yükseltilir.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Yeni yükseltilmiş veya yeni bir Windows 10 Pro cihaz için

Windows 10 Pro Creators Update çalıştıran yeni bir cihaz için ya da Windows 10 Pro Creators Update sürümüne yükseltilmiş ancak Windows 10 cihaz kurulumu henüz tamamlanmamış bir cihaz için bu adımları izleyin.
  
1. **Nasıl ayarlamak istersiniz?** sayfasına gelene kadar Windows 10 cihaz kurulumu adımlarını tamamlayın. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Burada, Kuruluş **için ayarla'ya tıklayın** ve kuruluş için kullanıcı adınızı ve parolanızı Microsoft 365 İş Ekstra. 
    
3. Windows 10 cihazı kurulumunu tamamlayın.
    
   İşiniz bittiğinde kullanıcı, kuruluşunuzun Azure AD'sine bağlanmış olur. Emin olmak için bkz. [Cihazın Azure AD'ye bağlı olduğunu doğrulama](#verify-the-device-is-connected-to-azure-ad). 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Önceden ayarlanmış ve Windows 10 Pro çalıştıran bir cihaz için

 **Kullanıcıları Azure AD'ye bağlama:**
  
1. Kullanıcınızın Windows 10 Pro sürüm 1703 (Creators Update) (bkz. [önkoşullar](pre-requisites-for-data-protection.md)) çalıştıran Windows bilgisayarında, Windows logosuna ve ardından Ayarlar simgesine tıklayın.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. **Ayarlar**'da **Hesaplar**'a gidin.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. **Bilgileriniz** sayfasında **İş yeri veya okula erişim** \> **Bağlan**'a tıklayın.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. **İş veya okul hesabı ayarlama** iletişim kutusunda **Diğer eylemler**'in altında **Bu cihazı Azure Active Directory'ye ekleyin**'i seçin.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Bunun **sizin kuruluş bağlantınız olduğundan emin olun** sayfasında, bilgilerin doğru olduğundan emin olun ve Katıl'ı **seçin.**
  
   **Hazırsınız!** page, chosse **Done .**
  
   ![Bunun sizin kuruluş ekranınız olduğundan emin olun ekranında Katıl'ı seçin](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
OneDrive İş'e dosya yüklediyseniz, bunları tekrar eşitleyin. Profil ve dosyaları geçirmek için üçüncü taraf bir araç kullandıysanız, bu dosyaları da yeni profile eşitlenin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Cihazın Azure AD'ye bağlı olduğunu doğrulama

Eşitlemenizin durumunu doğrulamak için, Ayarlar'daki İş veya okula **erişim** sayfasında **Bağlı** _ _ alanı öğesini seçerek Bilgi ve Bağlantıyı Kes \<organization name\> düğmelerini **gösterebilirsiniz.**  Eşitlemenizin **durumunu** almak için Bilgi'yi seçin. 
  
En son **mobil cihaz yönetim** ilkelerini bilgisayara **almak** için Eşitleme durumu sayfasında Eşitle'yi seçin.
  
Microsoft 365 İş Ekstra kullanmaya başlamak için, Başlangıç Windows gidin, geçerli  hesap resminize sağ tıklayın ve Ardından Hesap **değiştir'e tıklayın.** Kurumsal e-postanız ve parolanızla oturum açın.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Pc'nin Şu sürüme yükseltildikten Windows 10 Business

Azure AD'ye katılmış Windows 10 cihazlarınızı Windows 10 Business aboneliğinizin bir parçası olarak Microsoft 365 İş Ekstra doğrulayın.
  
1. **Ayarlar** \> **Sistem** \> **Hakkında**'ya gidin.
    
2. **Sürüm** bölümünde **Windows 10 Business** ifadesinin bulunduğunu doğrulayın.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Sonraki adımlar

Mobil cihazlarınızı ayarlamak için bkz. Microsoft 365 İş Ekstra kullanıcıları için mobil cihazları ayarlama [,](set-up-mobile-devices.md)Cihaz koruma veya uygulama koruma ilkelerini ayarlamak için bkz. [Microsoft 365 yönetme](manage.md).
  
## <a name="related-content"></a>İlgili içerik

[Microsoft 365 eğitim videoları için giriş](../business-video/index.yml) (bağlantı sayfası)
