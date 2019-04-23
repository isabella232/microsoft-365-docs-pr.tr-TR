---
title: Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Varsayılan Windows 10 aygıtları güvenliğini sağlamak için Microsoft 365 işletmede bulunan diğer ayarlar hakkında bilgi edinin.
ms.openlocfilehash: f9e890cde7a8290a9a8e81720d32a6a2889c312f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32285940"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="74325-103">Windows 10 PC'lere yönelik cihaz koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="74325-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="74325-104">Windows 10 cihazlarının güvenliğini sağlama</span><span class="sxs-lookup"><span data-stu-id="74325-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="74325-105">Microsoft 365 İş ile Windows 10 cihazlarının güvenliğini sağlama hakkındaki videoyu izleyin:</span><span class="sxs-lookup"><span data-stu-id="74325-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="74325-106">[Yönetim Merkezi](https://go.microsoft.com/fwlink/p/?linkid=837890) genel yönetim kimlik bilgileri ile oturum açın.</span><span class="sxs-lookup"><span data-stu-id="74325-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="74325-107">**Aygıtlar** üzerinde sol nav, seçim \> **ilkeleri** \> **Ekle**.</span><span class="sxs-lookup"><span data-stu-id="74325-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="74325-108">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="74325-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="74325-109">**İlke türü**'nün altında **Windows 10 Cihaz Yapılandırması**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="74325-109">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="74325-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span><span class="sxs-lookup"><span data-stu-id="74325-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span></span> 
    
    <span data-ttu-id="74325-112">Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="74325-112">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="74325-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="74325-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="74325-116">Son olarak, **Bitti**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="74325-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="74325-117">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="74325-117">Available settings</span></span>

<span data-ttu-id="74325-p103">Varsayılan olarak tüm ayarlar **Açık** durumdadır. Aşağıdaki ayarlar kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="74325-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="74325-120">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="74325-120">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="74325-121">Ayar</span><span class="sxs-lookup"><span data-stu-id="74325-121">Setting</span></span>  <br/> |<span data-ttu-id="74325-122">Açıklama</span><span class="sxs-lookup"><span data-stu-id="74325-122">Description</span></span>  <br/> |
|<span data-ttu-id="74325-123">Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="74325-123">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="74325-124">Bilgisayarları internete bağlı olmanın getirdiği tehlikelerden korumak için Windows Defender Virüsten Koruma programının açık olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="74325-124">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="74325-125">Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="74325-125">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="74325-126">Edge'de, kullanıcıları kötü amaçlı sitelerden ve indirmelerden korumaya yardımcı olan ayarları açar.</span><span class="sxs-lookup"><span data-stu-id="74325-126">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="74325-127">Cihazların saldırı alanını azaltan kuralları kullan</span><span class="sxs-lookup"><span data-stu-id="74325-127">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="74325-p104">Saldırı alanı azaltma özelliği açık olarak ayarlandığında zararlı yazılımlar tarafından cihazlara bulaşmak için tipik olarak kullanılan eylemleri ve uygulamaları engeller. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi edinmek için [Saldırı alanlarını azaltma](https://go.microsoft.com/fwlink/?linkid=870417) bölümüne bakın.  </span><span class="sxs-lookup"><span data-stu-id="74325-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="74325-131">Klasörleri fidye yazılımı gibi tehditlerden koruma</span><span class="sxs-lookup"><span data-stu-id="74325-131">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="74325-p105">Bu ayar, şirket verilerini fidye yazılımı gibi şüpheli veya zararlı uygulamalar tarafından gerçekleştirilen değişikliklere karşı korumak için denetimli klasör erişimini kullanır. Bu türdeki uygulamaların korumalı klasörlerde değişiklik yapması engellenir. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi almak için [Denetimli klasör erişimi ile klasörleri koruma](https://go.microsoft.com/fwlink/?linkid=870418) bölümüne bakın.  </span><span class="sxs-lookup"><span data-stu-id="74325-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="74325-136">İnternetteki olası zararlı içeriklerin ağa erişimini engelle</span><span class="sxs-lookup"><span data-stu-id="74325-136">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="74325-p106">Kimlik avı dolandırıcılığı, açıkları kötüye kullanan yazılımlar veya diğer zararlı içerikleri barındırabilecek, güvenilirliği düşük İnternet konumlarına yönelik giden kullanıcı bağlantılarını engellemek için bu ayarı kullanın. Bu ayar yalnızca Windows Defender Virüsten Koruma yazılımı Açık olarak ayarlandığında kullanılabilir. Daha fazla bilgi için [Ağınızı koruma](https://go.microsoft.com/fwlink/?linkid=870419) bölümüne bakın.  </span><span class="sxs-lookup"><span data-stu-id="74325-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="74325-140">BitLocker ile PC'lerdeki dosyaların ve klasörlerin yetkisiz erişime karşı korunmasına yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="74325-140">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="74325-p107">BitLocker bilgisayar sabit sürücülerini şifreleyerek verileri korur ve bilgisayar kaybolduğunda veya çalındığında verilerin açığa çıkma durumuna karşı koruma sağlar. Daha fazla bilgi için [Bitlocker SSS](https://go.microsoft.com/fwlink/?linkid=871000) bölümüne bakın.  </span><span class="sxs-lookup"><span data-stu-id="74325-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="74325-143">Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver</span><span class="sxs-lookup"><span data-stu-id="74325-143">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="74325-p108">Kullanıcıların Microsoft Store'ndan uygulama indirmesine ve yüklemesine izin verir. Uygulamalar, oyunlardan üretkenlik araçlarına kadar her şeyi içerebilir, dolayısıyla bu ayar **Açık** durumdadır ancak ek güvenlik için kapatabilirsiniz.  </span><span class="sxs-lookup"><span data-stu-id="74325-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="74325-146">Kullanıcıların Cortana'ya erişmesine izin ver</span><span class="sxs-lookup"><span data-stu-id="74325-146">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="74325-p109">Cortana çok yararlı olabilir! Cortana sizin yerinize ayarları açıp kapatabilir, yol tarif edebilir ve randevularınıza zamanında gitmenizi sağlayabilir; dolayısıyla bu ayar varsayılan olarak **Açık** durumdadır.  </span><span class="sxs-lookup"><span data-stu-id="74325-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="74325-149">Kullanıcıların Microsoft'tan Windows ipucu ve reklam almasına izin ver</span><span class="sxs-lookup"><span data-stu-id="74325-149">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="74325-150">Windows ipuçları kullanışlı olabilir ve yeni özellikler kullanıma sunulduğunda kullanıcıların yönlendirilmesine yardım edebilir.</span><span class="sxs-lookup"><span data-stu-id="74325-150">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="74325-151">Windows 10 cihazları otomatik olarak güncelleştir</span><span class="sxs-lookup"><span data-stu-id="74325-151">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="74325-152">Windows 10 cihazların son güncelleştirmeleri otomatik olarak aldığından emin olur.</span><span class="sxs-lookup"><span data-stu-id="74325-152">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="74325-153">Cihaz şu kadar süre boşta kaldığında ekranı kapat</span><span class="sxs-lookup"><span data-stu-id="74325-153">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="74325-p110">Kullanıcı cihaz başında olmadığında şirket verilerinin korunmasını sağlar. Kullanıcı bir kafe gibi herkese açık bir konumda çalışıyorken kısa süreliğine uzaklaşabilir veya başka bir şeyle ilgilenebilir ve bu sırada diğer kişiler cihazdaki bilgilere bakabilir. Bu ayar sayesinde, ekran kapanmadan önce kullanıcının ne kadar süre boşta olabileceğini denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="74325-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

