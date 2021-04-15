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
ms.openlocfilehash: f2b7962918186f4a1063c5a66596135c2972ec71
ms.sourcegitcommit: 07dea2aa98daf0c4086f8590375167830027c802
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51750010"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="070bf-103">Office 365 E3'den Microsoft 365 İş Ekstra'yamama</span><span class="sxs-lookup"><span data-stu-id="070bf-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="070bf-104">Microsoft 365 İş Ekstra, sınıf için en iyi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle bir araya getiren küçük işletmeniz için ihtiyacınız olan her şeye sahip.</span><span class="sxs-lookup"><span data-stu-id="070bf-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="070bf-105">Şu anda bir Office 365 E3 aboneliğiniz varsa ancak 300'den fazla çalışan yoksa, ek güvenlik özellikleri için Microsoft 365 İş Ekstra'ya geçmeyi göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="070bf-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="070bf-106">Geçiş yapmak kolaydır: Önce lisansları değiştirersiniz ve geçerli aboneliğinizin tüm verileriyle kullanıcı bilgileri korunur.</span><span class="sxs-lookup"><span data-stu-id="070bf-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="070bf-107">Geçiş sonrasında, Microsoft 365 İş Ekstra'ya eklenen özellikleri ayarlaym gerekir.</span><span class="sxs-lookup"><span data-stu-id="070bf-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="070bf-108">Office 365 E3 ile Microsoft 365 İş Ekstra arasındaki farklar</span><span class="sxs-lookup"><span data-stu-id="070bf-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="070bf-109">Bu tabloda, Microsoft 365 İş Ekstra ile Office 365 E3 arasındaki farklar gösterir.</span><span class="sxs-lookup"><span data-stu-id="070bf-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="070bf-110">Özellik</span><span class="sxs-lookup"><span data-stu-id="070bf-110">Feature</span></span>    | <span data-ttu-id="070bf-111">Microsoft 365 İş Ekstra desteği</span><span class="sxs-lookup"><span data-stu-id="070bf-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="070bf-112">Office 365 E3'te destek</span><span class="sxs-lookup"><span data-stu-id="070bf-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="070bf-113">**Şirket içi**</span><span class="sxs-lookup"><span data-stu-id="070bf-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="070bf-114">Office uygulamaları<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="070bf-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="070bf-115">İş için Microsoft 365 Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="070bf-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="070bf-116">Microsoft 365 Kurumsal Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="070bf-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="070bf-117">**Bulut üretkenlik uygulamaları**</span><span class="sxs-lookup"><span data-stu-id="070bf-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="070bf-118">Exchange Online ve Outlook</span><span class="sxs-lookup"><span data-stu-id="070bf-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="070bf-119">Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="070bf-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="070bf-120">Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="070bf-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="070bf-121">Teams</span><span class="sxs-lookup"><span data-stu-id="070bf-121">Teams</span></span>    | ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) | 
| <span data-ttu-id="070bf-124">OneDrive İş</span><span class="sxs-lookup"><span data-stu-id="070bf-124">OneDrive for Business</span></span>    | <span data-ttu-id="070bf-125">Kullanıcı başına 1 TB depolama sınırı</span><span class="sxs-lookup"><span data-stu-id="070bf-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="070bf-126">Sınırsız</span><span class="sxs-lookup"><span data-stu-id="070bf-126">Unlimited</span></span> | 
| <span data-ttu-id="070bf-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="070bf-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) | 
| <span data-ttu-id="070bf-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="070bf-130">StaffHub</span></span>    | ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png) | 
| <span data-ttu-id="070bf-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="070bf-133">MileIQ</span></span>    | ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | | 
| <span data-ttu-id="070bf-135">**Tehdit Koruması**</span><span class="sxs-lookup"><span data-stu-id="070bf-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="070bf-136">Office 365 için Defender Plan 1</span><span class="sxs-lookup"><span data-stu-id="070bf-136">Defender for Office 365 Plan 1</span></span> | ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | <span data-ttu-id="070bf-138">Dahil değildir, ancak</span><span class="sxs-lookup"><span data-stu-id="070bf-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="070bf-139">**Kimlik yönetimi**</span><span class="sxs-lookup"><span data-stu-id="070bf-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="070bf-140">Karma Azure Active Directory (Azure AD) hesapları için self servis parola sıfırlama, Azure AD multi-factor authentication (MFA), Koşullu Erişim, şirket içi kimlikler için parola geri yazma</span><span class="sxs-lookup"><span data-stu-id="070bf-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    |  | 
| <span data-ttu-id="070bf-142">**Cihaz ve uygulama yönetimi**</span><span class="sxs-lookup"><span data-stu-id="070bf-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="070bf-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="070bf-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    |  |
| <span data-ttu-id="070bf-145">Paylaşılan bilgisayar etkinleştirmesi</span><span class="sxs-lookup"><span data-stu-id="070bf-145">Shared computer activation</span></span>|     ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    | ![Office 365 E3'e dahil](../media/check-mark.png)| 
| <span data-ttu-id="070bf-148">Win 7/8.1 Pro lisanslarından Windows 10 Pro'ya yükseltme hakları</span><span class="sxs-lookup"><span data-stu-id="070bf-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)    || 
| <span data-ttu-id="070bf-150">**Bilgi koruması**</span><span class="sxs-lookup"><span data-stu-id="070bf-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="070bf-151">Office 365 Veri Kaybını Önleme</span><span class="sxs-lookup"><span data-stu-id="070bf-151">Office 365 Data Loss Prevention</span></span>|    ![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)|![Office 365 E3'e dahil](../media/check-mark.png)|
|<span data-ttu-id="070bf-154">Azure Information Protection Plan 1, BitLocker zorlaması</span><span class="sxs-lookup"><span data-stu-id="070bf-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)||
|<span data-ttu-id="070bf-156">Azure Information Protection Plan 1, Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="070bf-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Microsoft 365 İş Ekstra'ya dahil](../media/check-mark.png)||
|<span data-ttu-id="070bf-158">**İstemci Erişimi Lisansı (CAL hakları)**</span><span class="sxs-lookup"><span data-stu-id="070bf-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="070bf-159">Kurumsal CAL Paketi (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="070bf-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Office 365 E3'e dahil](../media/check-mark.png)|

<span data-ttu-id="070bf-161"><sup>1</sup> Office uygulamalarının Microsoft 365 İş Ekstra sürümü Grup İlkesi, uygulama telemetrisi, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya İş Zekası aracılığıyla toplu etkinleştirmeyi içermemektedir.</span><span class="sxs-lookup"><span data-stu-id="070bf-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="070bf-162">Geçiş</span><span class="sxs-lookup"><span data-stu-id="070bf-162">Migration</span></span>

<span data-ttu-id="070bf-163">Aboneliğinizi geçirmek için, [yalnızca birkaç](../commerce/subscriptions/change-plans-manually.md) kişiyi Microsoft 365 İş Ekstra'ya taşımak istediğiniz yönergeler için bkz. Planları el ile değiştirme.</span><span class="sxs-lookup"><span data-stu-id="070bf-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="070bf-164">Ayrıca, E3 [aboneliğinizi](../commerce/subscriptions/upgrade-to-different-plan.md)ve lisanslarınızı Microsoft 365 İş Ekstra aboneliğine taşımak için herkesi otomatik olarak yükseltebilirsiniz veya bir iş ortağıyla çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="070bf-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="070bf-165">Aşağıdaki bölümlerde, varsa yapmak için ihtiyacınız olan değişiklikler ve geçiş sonrasında neler yapabilirsiniz açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="070bf-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="070bf-166">Office 365 E3 abonelik yapılandırması ve verileri</span><span class="sxs-lookup"><span data-stu-id="070bf-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="070bf-167">Şu gibi değişikliklerden önce geçerli aboneliğiniz veya verilerinizde değişiklik yapmak zorunda değilsiniz:</span><span class="sxs-lookup"><span data-stu-id="070bf-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="070bf-168">Dns kayıtları ve etki alanı adları gibi abonelik yapılandırması.</span><span class="sxs-lookup"><span data-stu-id="070bf-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="070bf-169">Çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ile kimlik doğrulama ayarları.</span><span class="sxs-lookup"><span data-stu-id="070bf-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="070bf-170">Teams, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive İş klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve bunların verileri.</span><span class="sxs-lookup"><span data-stu-id="070bf-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="070bf-171">Office uygulamaları otomatik olarak ölçeklendirilir.</span><span class="sxs-lookup"><span data-stu-id="070bf-171">Office applications will scale automatically.</span></span> <span data-ttu-id="070bf-172">Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte bir kontrol edin ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.</span><span class="sxs-lookup"><span data-stu-id="070bf-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="070bf-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="070bf-173">Windows 10</span></span>

<span data-ttu-id="070bf-174">Windows'uz henüz Windows Pro Creator Update'i üzerinde değilken [Windows Pro Creators Update sürümüne yükseltin.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="070bf-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="070bf-175">Kullanıcı cihazlarını ve dosyalarını korumak için ilkeler ayarlama</span><span class="sxs-lookup"><span data-stu-id="070bf-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="070bf-176">Office 365 MDM ilkelerini ve cihazlarını ayarsanız, bu  cihazlar Microsoft 365 yönetim merkezinin Cihazlar sayfasında listelenir.</span><span class="sxs-lookup"><span data-stu-id="070bf-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="070bf-177">Ayar her ilke [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="070bf-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="070bf-178">Lisansları Microsoft 365 İş Ekstra'ya atadikten sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="070bf-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="070bf-179">Kurumuzdan herkesi Microsoft 365 İş Ekstra'ya yükselttiysanız, Giriş sayfasında kurulum sihirbazını görebilirsiniz ve dosyaları ve mobil cihazları korumak için kurulum sihirbazı adımlarında [Microsoft 365 İş Ekstra'nın](set-up.md) kurulumu adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="070bf-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="070bf-180">Şu adımları Cihazlar sayfasında da tamamabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="070bf-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="070bf-181">Yönetim merkezinde, sol gezintide Cihaz **İlkeleri'ne** \> **gidin.**</span><span class="sxs-lookup"><span data-stu-id="070bf-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="070bf-182">Cihaz ilkeleri **sayfasında Ekle'yi** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="070bf-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="070bf-183">İlke **ekle bölmesinde** ilkeye bir ad verin ve sonra açılan açılan seçim **listesinden** İlke türü seçin.</span><span class="sxs-lookup"><span data-stu-id="070bf-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="070bf-184">Android ve iPhone cihazlarının yanı sıra Windows 10'da da dosyaları korumak için uygulama ilkeleri kurabilirsiniz ve şirkete ait Windows 10 cihazları için cihaz yapılandırma ilkeleri kurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="070bf-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="070bf-185">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="070bf-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="070bf-186">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="070bf-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="070bf-187">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="070bf-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="070bf-188">Windows 10 pc'ler için cihaz koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="070bf-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="070bf-189">İlkeleri ayar defa siz ve çalışanlarınız cihazları kurabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="070bf-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="070bf-190">Windows [cihazlarına ilgili adımlar için bkz. Microsoft 365 İş Ekstra](set-up-windows-devices.md) kullanıcıları için Windows cihazlarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="070bf-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="070bf-191">Android [telefonlar ve iPhone'lar için adımlar için bkz. Microsoft 365](set-up-mobile-devices.md) İş Ekstra kullanıcıları için mobil cihazları ayarlama.</span><span class="sxs-lookup"><span data-stu-id="070bf-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="070bf-192">Posta Kutusu Boyutu</span><span class="sxs-lookup"><span data-stu-id="070bf-192">Mailbox Size</span></span>

<span data-ttu-id="070bf-193">Exchange Online Plan 1'i kullandığı için Microsoft 365 İş Ekstra'nın 50 GB depolama sınırı vardır.</span><span class="sxs-lookup"><span data-stu-id="070bf-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="070bf-194">Microsoft 365 İş Ekstra'ya geçen kullanıcılardan herhangi biri 50 GB'lık posta kutusu depolama alanını aşarsa, bu kullanıcıya Exchange Online Plan 2 atamanız ve Exchange Online Plan 1'i kaldırmanız önerilir çünkü her ikisini de atamak uygun değildir.</span><span class="sxs-lookup"><span data-stu-id="070bf-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="070bf-195">Tehdit koruması</span><span class="sxs-lookup"><span data-stu-id="070bf-195">Threat protection</span></span>

<span data-ttu-id="070bf-196">Microsoft 365 İş Ekstra'ya katıldıktan sonra Office 365 için Defender'a sahipsiniz.</span><span class="sxs-lookup"><span data-stu-id="070bf-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="070bf-197">Genel [bir bakış için bkz. Office 365](../security/office-365-security/defender-for-office-365.md) için Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="070bf-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="070bf-198">Ayarlamak için [bkz.](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)Güvenli Bağlantıları [ayarlama,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)Güvenli Ekleri ayarlama ve Office 365 için Defender'da Kimlik avı [önleme'i ayarlama.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="070bf-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="070bf-199">Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="070bf-199">Sensitivity labels</span></span>

<span data-ttu-id="070bf-200">Duyarlılık etiketlerini kullanmaya başlamak için bkz. [Duyarlılık etiketlerine genel bakış](../compliance/sensitivity-labels.md) ve duyarlılık etiketleri videosu oluşturma ve [yönetme.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="070bf-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
