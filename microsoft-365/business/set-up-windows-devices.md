---
title: Microsoft 365 Business kullanıcıları için Windows cihazlarını ayarlama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Microsoft 365 iş kullanıcıları için Windows 10 Pro çalıştıran Windows aygıtı kurmayı öğrenin. '
ms.openlocfilehash: 482199b175c568bfae420619aa02024303894789
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982860"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Microsoft 365 Business kullanıcıları için Windows cihazlarını ayarlama

## <a name="prerequisites"></a>Önkoşullar

Microsoft 365 Business kullanıcıları için Windows cihazları ayarlamadan önce, tüm Windows cihazların Windows 10 Pro sürüm 1703 (Creators Update) çalıştırdığından emin olun. Windows 10 Pro'yu tamamlayıcı nitelikte bir bulut hizmetleri ve cihaz yönetimi kümesi olan ve Microsoft 365 Business'ın güvenlik denetimlerine ve merkezi olarak yönetilmesine olanak sağlayan Windows 10 Business'in dağıtımı için gerekli önkoşullardan biri Windows 10 Pro'dur.
  
Windows 7 Pro, Windows 8 Pro veya Windows 8.1 Pro çalıştıran Windows cihazlarınız varsa, Microsoft 365 Business aboneliğiniz size bir Windows 10 yükseltmesi hakkı tanır.
  
Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltme hakkında daha fazla bilgi için bu konudaki adımları izleyin: [Windows cihazları Windows Pro Creators Update sürümüne yükseltme](upgrade-to-windows-pro-creators-update.md).
  
Yükseltmeye sahip olduğunuzu doğrulamak veya yükseltmenin çalıştığından emin olmak için bkz. [Cihazın Windows 10 Business'a yükseltildiğini doğrulama](set-up-windows-devices.md#bkmk_verifywin10). 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Kuruluşunuzun Azure AD'sine Windows 10 cihazlarını ekleme

Kuruluşunuzdaki tüm Windows cihazları Windows 10 Pro Creators Update sürümüne yükseltildiyse ya da tüm Windows cihazları zaten Windows 10 Pro Creators Update sürümünü çalıştırıyorsa, bu cihazları kuruluşunuzun Azure Active Directory'sine ekleyebilirsiniz. Eklenen cihazlar, Microsoft 365 Business aboneliğine dahil olan Windows 10 Business'a otomatik olarak yükseltilir.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Yeni yükseltilmiş veya yeni bir Windows 10 Pro cihaz için

Windows 10 Pro Creators Update çalıştıran yeni bir cihaz için ya da Windows 10 Pro Creators Update sürümüne yükseltilmiş ancak Windows 10 cihaz kurulumu henüz tamamlanmamış bir cihaz için bu adımları izleyin.
  
1. **Nasıl ayarlamak istersiniz?** sayfasına gelene kadar Windows 10 cihaz kurulumu adımlarını tamamlayın. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Burada **Kuruluş için ayarlama**'yı seçin ve ardından Microsoft 365 Business kullanıcı adınızı ve parolanızı girin. 
    
3. Windows 10 cihazı kurulumunu tamamlayın.
    
   İşiniz bittiğinde kullanıcı, kuruluşunuzun Azure AD'sine bağlanmış olur. Emin olmak için bkz. [Cihazın Azure AD'ye bağlı olduğunu doğrulama](set-up-windows-devices.md#bkmk_verifyaad). 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Önceden ayarlanmış ve Windows 10 Pro çalıştıran bir cihaz için

 **Kullanıcıları Azure AD'ye bağlama:**
  
1. Kullanıcınızın Windows 10 Pro sürüm 1703 (Creators Update) (bkz. [önkoşullar](pre-requisites-for-data-protection.md)) çalıştıran Windows bilgisayarında, Windows logosuna ve ardından Ayarlar simgesine tıklayın.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. **Ayarlar**'da **Hesaplar**'a gidin.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. **Bilgileriniz** sayfasında **İş yeri veya okula erişim** \> **Bağlan**'a tıklayın.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. **İş veya okul hesabı ayarlama** iletişim kutusunda **Diğer eylemler**'in altında **Bu cihazı Azure Active Directory'ye ekleyin**'i seçin.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. **Diyelim ki, oturum açmanızın Al** sayfasında, iş veya Okul hesabınıza girin \> **sonraki**.
  
   Parolanızı **Parola gir** sayfasında girin \> **oturum açın**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Üzerinde ** kuruluşunuzun bu olduğundan emin olun ** sayfa, bilgilerin doğru olduğundan emin olun ve **Katıl**' ı tıklatın.
  
   **Hazırsınız!** sayfasında **Bitti**'ye tıklayın.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
OneDrive İş'e dosya yüklediyseniz, bunları tekrar eşitleyin. Profil ve dosyaları geçirmek için üçüncü taraf bir aracı kullandıysanız, bunları da yeni profile eşitleyin.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Cihazın Azure AD'ye bağlı olduğunu doğrulama

Eşitleme durumunuzu doğrulamak için, **Ayarlar**'daki **İş yeri veya okula erişim** sayfasında **Bağlanılan yer** _ \<organization name\> _ alanına tıklayarak **Bilgi** ve **Bağlantıyı kes** düğmelerini görüntüleyin. Eşitleme durumunuzu görmek için **Bilgi**'ye tıklayın. 
  
En son mobil cihaz yönetimi ilkelerini bilgisayara aktarmak için, Eşitleme durumu sayfasında Eşitle'ye tıklayın.
  
Microsoft 365 İş hesabınızı kullanmaya başlamak için Windows **Başlat** düğmesine gidip geçerli hesap resminize sağ tıklayın ve **Hesap değiştir**'i seçin. Kurumsal e-postanız ve parolanızla oturum açın.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Cihazın Windows 10 Business'a yükseltildiğini doğrulama

Azure AD'ye eklenmiş Windows 10 cihazlarınızın, Microsoft 365 Business aboneliğinize dahil olan Windows 10 Business'a yükseltildiğini doğrulayın.
  
1. **Ayarlar** \> **Sistem** \> **Hakkında**'ya gidin.
    
2. **Sürüm** bölümünde **Windows 10 Business** ifadesinin bulunduğunu doğrulayın.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Sonraki adımlar

Mobil cihazlarınızı ayarlamak için [Microsoft 365 Business kullanıcıları için mobil cihazları ayarlama](set-up-mobile-devices.md) bölümüne, cihaz koruma veya uygulama koruma ilkelerini ayarlamak içinse [Microsoft 365 Business yönetimi](manage.md) bölümüne bakın.
  
