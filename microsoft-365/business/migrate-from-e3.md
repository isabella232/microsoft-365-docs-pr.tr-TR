---
title: Office 365 E3 'den Microsoft 365 Business 'a geçme
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: İşinizi Office 365 E3 'den Microsoft 365 Business Premium 'a taşımayı öğrenin.
ms.openlocfilehash: b8aa58f1f050ec6247479ed02e142507a2df45fc
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842170"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="c1475-103">Office 365 E3 'den Microsoft 365 Business Premium 'a geçme</span><span class="sxs-lookup"><span data-stu-id="c1475-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="c1475-104">Microsoft 365 Iş ekstra, basit cihaz yönetimi ve güvenliğiyle en iyi sınıf bulut tabanlı verimlilik uygulamalarını birleştiren küçük işletmeniz için gereken her şeyi içerir.</span><span class="sxs-lookup"><span data-stu-id="c1475-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="c1475-105">Şu anda bir Office 365 E3 aboneliğiniz varsa, ancak 300 ' den fazla çalışanı yoksa, ek güvenlik özellikleri için Microsoft 365 Iş Premium 'a geçmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c1475-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="c1475-106">Geçiş kolay: Ilk olarak lisansları değiştirdiğinizde geçerli aboneliğinizde tüm verileriniz ve Kullanıcı bilgileriniz korunur.</span><span class="sxs-lookup"><span data-stu-id="c1475-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="c1475-107">Geçişten sonra, Microsoft 365 Business Premium 'A eklenen özellikleri ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="c1475-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="c1475-108">Office 365 E3 ve Microsoft 365 Iş ekstra arasındaki farklar</span><span class="sxs-lookup"><span data-stu-id="c1475-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="c1475-109">Bu tabloda, Microsoft 365 Business Premium ve Office 365 E3 arasındaki farklılıklar gösterilmektedir.</span><span class="sxs-lookup"><span data-stu-id="c1475-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="c1475-110">Özellik</span><span class="sxs-lookup"><span data-stu-id="c1475-110">Feature</span></span>    | <span data-ttu-id="c1475-111">Microsoft 365 Business Premium 'da destek</span><span class="sxs-lookup"><span data-stu-id="c1475-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="c1475-112">Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="c1475-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="c1475-113">**Şirket içi**</span><span class="sxs-lookup"><span data-stu-id="c1475-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="c1475-114">Office uygulamaları<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="c1475-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="c1475-115">İş için Microsoft 365 uygulamaları</span><span class="sxs-lookup"><span data-stu-id="c1475-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="c1475-116">Microsoft 365 Kurumsal Uygulamaları</span><span class="sxs-lookup"><span data-stu-id="c1475-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="c1475-117">**Bulut üretkenlik uygulamaları**</span><span class="sxs-lookup"><span data-stu-id="c1475-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="c1475-118">Exchange Online ve Outlook</span><span class="sxs-lookup"><span data-stu-id="c1475-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="c1475-119">posta kutusu başına 50 GB depolama alanı ve sınırsız Exchange Online arşivleme</span><span class="sxs-lookup"><span data-stu-id="c1475-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="c1475-120">posta kutusu başına 100 GB depolama alanı ve sınırsız Exchange Online arşivleme</span><span class="sxs-lookup"><span data-stu-id="c1475-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="c1475-121">Teams</span><span class="sxs-lookup"><span data-stu-id="c1475-121">Teams</span></span>    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="c1475-124">OneDrive İş</span><span class="sxs-lookup"><span data-stu-id="c1475-124">OneDrive for Business</span></span>    | <span data-ttu-id="c1475-125">Kullanıcı başına 1 TB depolama sınırı</span><span class="sxs-lookup"><span data-stu-id="c1475-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="c1475-126">Süresiz</span><span class="sxs-lookup"><span data-stu-id="c1475-126">Unlimited</span></span> | 
| <span data-ttu-id="c1475-127">Yammer, SharePoint Online, Planner, akış</span><span class="sxs-lookup"><span data-stu-id="c1475-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="c1475-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="c1475-130">StaffHub</span></span>    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="c1475-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="c1475-133">Outlook Customer Manager, MileIQ</span></span>    | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | | 
| <span data-ttu-id="c1475-135">**Tehdit koruması**</span><span class="sxs-lookup"><span data-stu-id="c1475-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="c1475-136">Office 365 plan 1 için Defender</span><span class="sxs-lookup"><span data-stu-id="c1475-136">Defender for Office 365 Plan 1</span></span> | ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | <span data-ttu-id="c1475-138">Dahil değildir, ancak eklenebilir</span><span class="sxs-lookup"><span data-stu-id="c1475-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="c1475-139">**Kimlik yönetimi**</span><span class="sxs-lookup"><span data-stu-id="c1475-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="c1475-140">Karma Azure Active Directory (Azure AD) hesapları, Azure Multi-Factor Authentication (MFA) için self servis parola sıfırlama, koşullu erişim, şirket içi kimlikler için parola geri yazma</span><span class="sxs-lookup"><span data-stu-id="c1475-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    |  | 
| <span data-ttu-id="c1475-142">**Cihaz ve uygulama yönetimi**</span><span class="sxs-lookup"><span data-stu-id="c1475-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="c1475-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c1475-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    |  |
| <span data-ttu-id="c1475-145">Paylaşılan bilgisayar etkinleştirmesi</span><span class="sxs-lookup"><span data-stu-id="c1475-145">Shared computer activation</span></span>|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| <span data-ttu-id="c1475-148">Win 7/8.1 Pro lisanlarından Windows 10 Pro 'ya yükseltme hakları</span><span class="sxs-lookup"><span data-stu-id="c1475-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)    || 
| <span data-ttu-id="c1475-150">**Bilgi koruması**</span><span class="sxs-lookup"><span data-stu-id="c1475-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="c1475-151">Office 365 veri kaybı önleme</span><span class="sxs-lookup"><span data-stu-id="c1475-151">Office 365 Data Loss Prevention</span></span>|    ![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|<span data-ttu-id="c1475-154">Azure bilgi koruma planı 1, BitLocker zorlaması</span><span class="sxs-lookup"><span data-stu-id="c1475-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)||
|<span data-ttu-id="c1475-156">Azure bilgi koruma planı 1, duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="c1475-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Microsoft 365 Business Premium ile birlikte gelir](../media/check-mark.png)||
|<span data-ttu-id="c1475-158">**İstemci erişim lisansı (CAL hakları)**</span><span class="sxs-lookup"><span data-stu-id="c1475-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="c1475-159">Kurumsal CAL Paketi (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="c1475-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<span data-ttu-id="c1475-161"><sup>1</sup> Office uygulamalarının Microsoft 365 Business Premium sürümü Grup ilkesi, uygulama telemetri, güncelleştirme denetimleri, elektronik tablo karşılaştırma ve sorgulama veya iş zekası aracılığıyla toplu etkinleştirme içermez.</span><span class="sxs-lookup"><span data-stu-id="c1475-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="c1475-162">Geçişte</span><span class="sxs-lookup"><span data-stu-id="c1475-162">Migration</span></span>

<span data-ttu-id="c1475-163">Aboneliğinizi geçirmek için, yalnızca birkaç kişiyi Microsoft 365 Business Premium 'a taşımak isterseniz yönergeleri [El Ile değiştirme](../commerce/subscriptions/change-plans-manually.md) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c1475-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="c1475-164">Ayrıca, E3 aboneliğinizi ve lisanslarınızı bir Microsoft 365 Iş Ekstra aboneliğine taşımak için [herkesi otomatik olarak yükseltebilir](../commerce/subscriptions/upgrade-to-different-plan.md)veya bir iş ortağıyla çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c1475-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="c1475-165">Aşağıdaki bölümlerde, eğer varsa ve geçiş sonrasında yapabileceğiniz değişiklikler açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="c1475-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="c1475-166">Office 365 E3 abonelik yapılandırması ve verileri</span><span class="sxs-lookup"><span data-stu-id="c1475-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="c1475-167">Geçirmeden önce geçerli aboneliğinizde veya verilerinizde değişiklik yapmanız gerekmez, aşağıdakileri içerir:</span><span class="sxs-lookup"><span data-stu-id="c1475-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="c1475-168">DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.</span><span class="sxs-lookup"><span data-stu-id="c1475-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="c1475-169">Kullanıcı ve grup hesapları ve çok faktörlü kimlik doğrulaması veya koşullu erişim ilkeleri gibi kimlik doğrulama ayarları.</span><span class="sxs-lookup"><span data-stu-id="c1475-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="c1475-170">Üretkenlik hizmeti yapılandırmaları ve takımlar, Exchange Online posta kutuları, SharePoint Online siteleri, OneDrive Iş klasörleri ve OneNote Not defterleri gibi verileri.</span><span class="sxs-lookup"><span data-stu-id="c1475-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="c1475-171">Office uygulamaları otomatik olarak ölçeklenir.</span><span class="sxs-lookup"><span data-stu-id="c1475-171">Office applications will scale automatically.</span></span> <span data-ttu-id="c1475-172">Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte denetler ve Office uygulamalarını Kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.</span><span class="sxs-lookup"><span data-stu-id="c1475-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="c1475-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="c1475-173">Windows 10</span></span>

<span data-ttu-id="c1475-174">Windows 'da Windows Pro Creator güncelleştirmesi yoksa, [bunları Windows Pro Creators Update 'e yükseltebilirsiniz](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="c1475-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="c1475-175">Kullanıcı aygıtlarını ve dosyalarını koruyacak ilkeler ayarlama</span><span class="sxs-lookup"><span data-stu-id="c1475-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="c1475-176">Office 365 MDM ilkeleri ve aygıtları ayarlıyorsanız, bu cihazlar Microsoft 365 yönetim merkezindeki **cihazlar** sayfasında listelenir.</span><span class="sxs-lookup"><span data-stu-id="c1475-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="c1475-177">Ayarladığınız tüm ilkeler [Intune portalında](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="c1475-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="c1475-178">Microsoft 365 Business Premium 'a lisans atadıktan sonra, kullanıcıların cihazlarını ve dosyalarını korumaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c1475-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="c1475-179">Kuruluşunuzdaki herkesi Microsoft 365 Business Premium 'a yükselttiyseniz, giriş sayfasında Kurulum Sihirbazı 'nı görürsünüz ve dosyaları ve mobil cihazları koruyan [Kurulum sihirbazındaki Microsoft 365 Business Premium](set-up.md) kurulumunu izleyebilir.</span><span class="sxs-lookup"><span data-stu-id="c1475-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="c1475-180">Bu adımları aygıtlar sayfasında da tamamlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c1475-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="c1475-181">Yönetim merkezinde, sol gezintide, **cihazlar** \> **ilkeleri** 'ne gidin.</span><span class="sxs-lookup"><span data-stu-id="c1475-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="c1475-182">**Cihaz ilkeleri** sayfasında **Ekle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="c1475-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="c1475-183">**Ilke Ekle** bölmesinde ilkeye bir ad verin ve açılan listeden bir **ilke türü** seçin.</span><span class="sxs-lookup"><span data-stu-id="c1475-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="c1475-184">Windows 10 ' da Android ve iPhone cihazlarında dosyaları korumak için uygulama ilkelerini ayarlayabilir ve şirkete ait Windows 10 cihazlarında aygıt yapılandırma ilkelerini ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c1475-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="c1475-185">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="c1475-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="c1475-186">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="c1475-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="c1475-187">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="c1475-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="c1475-188">Windows 10 bilgisayarlarında cihaz koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="c1475-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="c1475-189">İlkeleri ayarladıktan sonra, siz ve çalışanlarınız cihazları ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c1475-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="c1475-190">Windows aygıtlarının adımları için [Microsoft 365 Business Premium kullanıcıları Için Windows cihazlarını ayarlama](set-up-windows-devices.md) bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="c1475-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="c1475-191">Android telefonlar ve IPhone adımları için [Microsoft 365 Business Premium kullanıcıları için mobil cihazları ayarlayın](set-up-mobile-devices.md) bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="c1475-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="c1475-192">Posta kutusu boyutu</span><span class="sxs-lookup"><span data-stu-id="c1475-192">Mailbox Size</span></span>

<span data-ttu-id="c1475-193">Microsoft 365 Business Premium, Exchange Online Plan 1 kullandığı için 50 GB depolama sınırlamasına sahiptir.</span><span class="sxs-lookup"><span data-stu-id="c1475-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="c1475-194">Microsoft 365 Business Premium 'a geçiş yaparken, kullanıcılarınız 50 GB 'lik posta kutusu deposunu aşıyorsa, bu kullanıcıyı bir Exchange Online Plan 2 ' ye atamanız ve her ikisini de atamak uygun olmadığı için Exchange Online Plan 1 ' i kaldırmanız önerilir.</span><span class="sxs-lookup"><span data-stu-id="c1475-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="c1475-195">Tehdit koruması</span><span class="sxs-lookup"><span data-stu-id="c1475-195">Threat protection</span></span>

<span data-ttu-id="c1475-196">Microsoft 365 Business Premium 'a geçtikten sonra, Office 365 için Defender 'ınız vardır.</span><span class="sxs-lookup"><span data-stu-id="c1475-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="c1475-197">Genel bakış için [Office 365 Için Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) 'a bakın.</span><span class="sxs-lookup"><span data-stu-id="c1475-197">See [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="c1475-198">Ayarlamak için, [Office 365 Için](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c) [güvenli bağlantıları ayarlama](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [güvenli ekleri ayarlama](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ve Office.</span><span class="sxs-lookup"><span data-stu-id="c1475-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="c1475-199">Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="c1475-199">Sensitivity labels</span></span>

<span data-ttu-id="c1475-200">Duyarlılık etiketlerini kullanmaya başlamak için, [duyarlılık etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ve [duyarlılık etiketleri oluşturma ve yönetme](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="c1475-200">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
