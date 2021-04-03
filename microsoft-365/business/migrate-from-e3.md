---
title: Office 365 E3'den Microsoft 365 İş'e geçiş
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: İşletmenizi Office 365 E3'te Microsoft 365 İş Ekstra'ya taşımayı öğrenin.
ms.openlocfilehash: ffb82fa40f05383260ac1b97ed0bdf5f2f30c1df
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578337"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="76391-103">Office 365 E3'den Microsoft 365 İş Ekstra'ya</span><span class="sxs-lookup"><span data-stu-id="76391-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="76391-104">Microsoft 365 İş Ekstra, sınıfı en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahip.</span><span class="sxs-lookup"><span data-stu-id="76391-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="76391-105">Şu anda bir Office 365 E3 aboneliğiniz varsa ancak 300'den fazla çalışan yoksa, ek güvenlik özellikleri için Microsoft 365 İş Ekstra'ya geçmeyi göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="76391-106">Geçiş kolaydır: İlk olarak lisansları değiştirebilirsiniz ve geçerli aboneliğinizin tüm verileri ve kullanıcı bilgileri korunur.</span><span class="sxs-lookup"><span data-stu-id="76391-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="76391-107">Geçiş sonrasında, Microsoft 365 İş Ekstra'ya eklenen özellikleri ayarlamalısiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="76391-108">Office 365 E3 ile Microsoft 365 İş Ekstra arasındaki farklar</span><span class="sxs-lookup"><span data-stu-id="76391-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="76391-109">Bu tablo, Microsoft 365 İş Ekstra ile Office 365 E3 arasındaki farkları gösterir.</span><span class="sxs-lookup"><span data-stu-id="76391-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="76391-110">Özellik</span><span class="sxs-lookup"><span data-stu-id="76391-110">Feature</span></span>    | <span data-ttu-id="76391-111">Microsoft 365 İş Ekstra desteği</span><span class="sxs-lookup"><span data-stu-id="76391-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="76391-112">Office 365 E3'te destek</span><span class="sxs-lookup"><span data-stu-id="76391-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="76391-113">**Şirket içi**</span><span class="sxs-lookup"><span data-stu-id="76391-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="76391-114">Office uygulamaları<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="76391-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="76391-115">İş için Microsoft 365 Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="76391-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="76391-116">Microsoft 365 Kurumsal Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="76391-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="76391-117">**Bulut üretkenlik uygulamaları**</span><span class="sxs-lookup"><span data-stu-id="76391-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="76391-118">Exchange Online ve Outlook</span><span class="sxs-lookup"><span data-stu-id="76391-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="76391-119">Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="76391-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="76391-120">Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="76391-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="76391-121">Teams</span><span class="sxs-lookup"><span data-stu-id="76391-121">Teams</span></span>    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="76391-124">OneDrive İş</span><span class="sxs-lookup"><span data-stu-id="76391-124">OneDrive for Business</span></span>    | <span data-ttu-id="76391-125">Kullanıcı başına 1 TB depolama sınırı</span><span class="sxs-lookup"><span data-stu-id="76391-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="76391-126">Sınırsız</span><span class="sxs-lookup"><span data-stu-id="76391-126">Unlimited</span></span> | 
| <span data-ttu-id="76391-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="76391-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="76391-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="76391-130">StaffHub</span></span>    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="76391-133">Outlook Customer Manager</span><span class="sxs-lookup"><span data-stu-id="76391-133">Outlook Customer Manager</span></span>    | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | | 
| <span data-ttu-id="76391-135">**Tehdit Koruması**</span><span class="sxs-lookup"><span data-stu-id="76391-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="76391-136">Office 365 için Defender Plan 1</span><span class="sxs-lookup"><span data-stu-id="76391-136">Defender for Office 365 Plan 1</span></span> | ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | <span data-ttu-id="76391-138">Dahil değildir, ancak</span><span class="sxs-lookup"><span data-stu-id="76391-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="76391-139">**Kimlik yönetimi**</span><span class="sxs-lookup"><span data-stu-id="76391-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="76391-140">Karma Azure Active Directory (Azure AD) hesapları için self servis parola sıfırlama, Azure AD çok faktörlü kimlik doğrulaması (MFA), Koşullu Erişim, şirket içi kimlikler için parola geri yazma</span><span class="sxs-lookup"><span data-stu-id="76391-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    |  | 
| <span data-ttu-id="76391-142">**Cihaz ve uygulama yönetimi**</span><span class="sxs-lookup"><span data-stu-id="76391-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="76391-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="76391-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    |  |
| <span data-ttu-id="76391-145">Paylaşılan bilgisayar etkinleştirmesi</span><span class="sxs-lookup"><span data-stu-id="76391-145">Shared computer activation</span></span>|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| <span data-ttu-id="76391-148">Win 7/8.1 Pro lisanslarından Windows 10 Pro'ya yükseltme hakları</span><span class="sxs-lookup"><span data-stu-id="76391-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)    || 
| <span data-ttu-id="76391-150">**Bilgi koruması**</span><span class="sxs-lookup"><span data-stu-id="76391-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="76391-151">Office 365 Veri Kaybını Önleme</span><span class="sxs-lookup"><span data-stu-id="76391-151">Office 365 Data Loss Prevention</span></span>|    ![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|<span data-ttu-id="76391-154">Azure Information Protection Plan 1, Bitlocker zorlaması</span><span class="sxs-lookup"><span data-stu-id="76391-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)||
|<span data-ttu-id="76391-156">Azure Information Protection Plan 1, Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="76391-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Microsoft 365 İş Ekstra ile birlikte](../media/check-mark.png)||
|<span data-ttu-id="76391-158">**İstemci Erişim Lisansı (CAL hakları)**</span><span class="sxs-lookup"><span data-stu-id="76391-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="76391-159">Kurumsal CAL Paketi (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="76391-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<span data-ttu-id="76391-161"><sup>1</sup> Office uygulamalarının Microsoft 365 İş Ekstra sürümü Grup İlkesi, uygulama telemetrisi, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya İş Zekası aracılığıyla toplu etkinleştirmeyi içermemektedir.</span><span class="sxs-lookup"><span data-stu-id="76391-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="76391-162">Geçiş</span><span class="sxs-lookup"><span data-stu-id="76391-162">Migration</span></span>

<span data-ttu-id="76391-163">Aboneliğinizi geçirmek için, yalnızca birkaç kişiyi Microsoft 365 İş Ekstra'ya taşımak istediğiniz yönergeleri el ile değiştirme yönergelerine bakın. [](../commerce/subscriptions/change-plans-manually.md)</span><span class="sxs-lookup"><span data-stu-id="76391-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="76391-164">Ayrıca, E3 [aboneliğinizi](../commerce/subscriptions/upgrade-to-different-plan.md)ve lisanslarınızı Microsoft 365 İş Ekstra aboneliğine taşımak için herkesi otomatik olarak yükseltebilirsiniz veya bir iş ortağıyla çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="76391-165">Aşağıdaki bölümlerde, varsa, yapmak için gereken değişiklikler ve geçiş sonrasında neler yapabilirsiniz açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="76391-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="76391-166">Office 365 E3 abonelik yapılandırması ve verileri</span><span class="sxs-lookup"><span data-stu-id="76391-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="76391-167">Geçerli aboneliğiniz veya verilerinizde, şu değişikliklerden önce değişiklik yapmak zorunda değildir:</span><span class="sxs-lookup"><span data-stu-id="76391-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="76391-168">DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.</span><span class="sxs-lookup"><span data-stu-id="76391-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="76391-169">Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.</span><span class="sxs-lookup"><span data-stu-id="76391-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="76391-170">Teams, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve bunların verileri.</span><span class="sxs-lookup"><span data-stu-id="76391-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="76391-171">Office uygulamaları otomatik olarak ölçeklendirilir.</span><span class="sxs-lookup"><span data-stu-id="76391-171">Office applications will scale automatically.</span></span> <span data-ttu-id="76391-172">Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte bir kontrol edin ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.</span><span class="sxs-lookup"><span data-stu-id="76391-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="76391-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="76391-173">Windows 10</span></span>

<span data-ttu-id="76391-174">Windows'uz henüz Windows Pro Creator güncelleştirmesi üzerinde değilse, bunları [Windows Pro Creators Update'e yükseltin.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="76391-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="76391-175">Kullanıcı cihazlarını ve dosyalarını korumak için ilkeler ayarlama</span><span class="sxs-lookup"><span data-stu-id="76391-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="76391-176">Office 365 MDM ilkelerini ve cihazlarını kursanız, bu  cihazlar Microsoft 365 yönetim merkezinin Cihazlar sayfasında listelenir.</span><span class="sxs-lookup"><span data-stu-id="76391-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="76391-177">Ayar her ilke [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="76391-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="76391-178">Lisansları Microsoft 365 İş Ekstra'ya atadikten sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="76391-179">Kuruluşta yer alan herkesi Microsoft 365 İş Ekstra'ya yükselttiyebilirsiniz. Kurulum sihirbazını Giriş sayfasında görebilirsiniz ve dosyaları ve mobil cihazları korumak için kurulum sihirbazı adımlarında [Microsoft 365 İş Ekstra'nın](set-up.md) kurulumu adımlarını takip edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="76391-180">Bu adımları Cihazlar sayfasında da tamamabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="76391-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="76391-181">Yönetim merkezinde, sol gezintide Cihazlar **İlkeleri'ne** \> **gidin.**</span><span class="sxs-lookup"><span data-stu-id="76391-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="76391-182">Cihaz ilkeleri **sayfasında Ekle'yi** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="76391-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="76391-183">İlke **ekle bölmesinde** ilkeye bir ad verin ve ardından açılan **listelerden bir** İlke türü seçin.</span><span class="sxs-lookup"><span data-stu-id="76391-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="76391-184">Android ve iPhone cihazlarının yanı sıra Windows 10'da da dosyaları korumak için uygulama ilkeleri ayarlarken, şirkete ait Windows 10 cihazları için cihaz yapılandırma ilkelerini de kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="76391-185">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="76391-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="76391-186">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="76391-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="76391-187">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="76391-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="76391-188">Windows 10 bilgisayarlar için cihaz koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="76391-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="76391-189">İlkeleri ayar defa siz ve çalışanlarınız cihazları kurabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="76391-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="76391-190">Windows [cihazları için adımlar için Bkz. Microsoft 365 İş Ekstra](set-up-windows-devices.md) kullanıcıları için Windows cihazlarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="76391-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="76391-191">Android telefonlar ve iPhone'lar için adımlar için [Bkz. Microsoft 365](set-up-mobile-devices.md) İş Ekstra kullanıcıları için mobil cihazları ayarlama.</span><span class="sxs-lookup"><span data-stu-id="76391-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="76391-192">Posta Kutusu Boyutu</span><span class="sxs-lookup"><span data-stu-id="76391-192">Mailbox Size</span></span>

<span data-ttu-id="76391-193">Exchange Online Plan 1'i kullandığı için Microsoft 365 İş Ekstra'nın 50 GB depolama sınırı vardır.</span><span class="sxs-lookup"><span data-stu-id="76391-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="76391-194">Microsoft 365 İş Ekstra'ya geçen kullanıcılardan herhangi biri 50 GB'lık posta kutusu depolama alanını aşarsa, bu kullanıcıya Exchange Online Plan 2 atamanız ve Exchange Online Plan 1'i kaldırmanız önerilir çünkü her ikisini de atamak uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="76391-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="76391-195">Tehdit koruması</span><span class="sxs-lookup"><span data-stu-id="76391-195">Threat protection</span></span>

<span data-ttu-id="76391-196">Microsoft 365 İş Ekstra'ya katıldıktan sonra Office 365 için Defender'a sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="76391-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="76391-197">Genel [bakış için Office 365 için Microsoft Defender'a](../security/office-365-security/defender-for-office-365.md) bakın.</span><span class="sxs-lookup"><span data-stu-id="76391-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="76391-198">Ayarlamak için Güvenli [Bağlantılar'ı](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [ayarlama,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)Güvenli Ekleri ayarlama ve [Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)için Defender'da Kimlik avı önlemeyi ayarlama.</span><span class="sxs-lookup"><span data-stu-id="76391-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="76391-199">Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="76391-199">Sensitivity labels</span></span>

<span data-ttu-id="76391-200">Duyarlılık etiketlerini kullanmaya başlamak için, duyarlılık etiketlerine [genel bakış](../compliance/sensitivity-labels.md) videosunu izleyin ve duyarlılık etiketleri videosu oluşturun [ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="76391-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
