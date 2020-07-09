---
title: Office 365 E3'ten Microsoft 365 Business'a geçiş
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
description: İşinizi Office 365 E3'ten Microsoft 365 Business Premium'a nasıl taşıyabildiğiniöğrenin.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081924"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="7ad23-103">Office 365 E3'ten Microsoft 365 Business Premium'a geçiş</span><span class="sxs-lookup"><span data-stu-id="7ad23-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="7ad23-104">Microsoft 365 Business Premium, sınıfının en iyisi bulut tabanlı üretkenlik uygulamalarını basit cihaz yönetimi ve güvenlikle birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahiptir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="7ad23-105">Şu anda bir Office 365 E3 aboneliğiniz varsa, ancak 300'den fazla çalışanın yoksa, ek güvenlik özellikleri için Microsoft 365 Business Premium'a geçmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="7ad23-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="7ad23-106">Geçiş kolaydır: Önce lisansları değiştirirsiniz ve geçerli aboneliğinizdeki tüm verileriniz ve kullanıcı bilgileriniz korunur.</span><span class="sxs-lookup"><span data-stu-id="7ad23-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="7ad23-107">Geçişten sonra Microsoft 365 Business Premium'a eklenen özellikleri ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="7ad23-108">Office 365 E3 ile Microsoft 365 Business Premium arasındaki farklar</span><span class="sxs-lookup"><span data-stu-id="7ad23-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="7ad23-109">Bu tablo, Microsoft 365 Business Premium ve Office 365 E3 arasındaki farkları gösterir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="7ad23-110">Özellik</span><span class="sxs-lookup"><span data-stu-id="7ad23-110">Feature</span></span>    | <span data-ttu-id="7ad23-111">Microsoft 365 Business Premium desteği</span><span class="sxs-lookup"><span data-stu-id="7ad23-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="7ad23-112">Office 365 E3'te destek</span><span class="sxs-lookup"><span data-stu-id="7ad23-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="7ad23-113">**Şirket içi**</span><span class="sxs-lookup"><span data-stu-id="7ad23-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="7ad23-114">Office uygulamaları<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="7ad23-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="7ad23-115">Microsoft 365 İş uygulamaları</span><span class="sxs-lookup"><span data-stu-id="7ad23-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="7ad23-116">Kurumsal uygulamalar için Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7ad23-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="7ad23-117">**Bulut üretkenliği uygulamaları**</span><span class="sxs-lookup"><span data-stu-id="7ad23-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="7ad23-118">Exchange Online ve Outlook</span><span class="sxs-lookup"><span data-stu-id="7ad23-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="7ad23-119">Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="7ad23-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="7ad23-120">Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online Arşivleme</span><span class="sxs-lookup"><span data-stu-id="7ad23-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="7ad23-121">Takım</span><span class="sxs-lookup"><span data-stu-id="7ad23-121">Teams</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="7ad23-124">OneDrive İş</span><span class="sxs-lookup"><span data-stu-id="7ad23-124">OneDrive for Business</span></span>    | <span data-ttu-id="7ad23-125">Kullanıcı başına 1 TB depolama sınırı</span><span class="sxs-lookup"><span data-stu-id="7ad23-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="7ad23-126">Sınırsız</span><span class="sxs-lookup"><span data-stu-id="7ad23-126">Unlimited</span></span> | 
| <span data-ttu-id="7ad23-127">Yammer, SharePoint Online, Planlayıcı, Akış</span><span class="sxs-lookup"><span data-stu-id="7ad23-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="7ad23-130">PersonelHub</span><span class="sxs-lookup"><span data-stu-id="7ad23-130">StaffHub</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="7ad23-133">Outlook Müşteri Yöneticisi, MileIQ</span><span class="sxs-lookup"><span data-stu-id="7ad23-133">Outlook Customer Manager, MileIQ</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | | 
| <span data-ttu-id="7ad23-135">**Tehdit Koruması**</span><span class="sxs-lookup"><span data-stu-id="7ad23-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="7ad23-136">Office 365 Gelişmiş Tehdit Koruması (ATP) Planı 1</span><span class="sxs-lookup"><span data-stu-id="7ad23-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | <span data-ttu-id="7ad23-138">Dahil değil, ancak eklenebilir</span><span class="sxs-lookup"><span data-stu-id="7ad23-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="7ad23-139">**Kimlik yönetimi**</span><span class="sxs-lookup"><span data-stu-id="7ad23-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="7ad23-140">Karma Azure Etkin Dizin (Azure AD) hesapları, Azure çok faktörlü kimlik doğrulama (MFA), Koşullu Erişim, şirket içi kimlikler için parola yazma için self servis parola sıfırlama</span><span class="sxs-lookup"><span data-stu-id="7ad23-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    |  | 
| <span data-ttu-id="7ad23-142">**Cihaz ve uygulama yönetimi**</span><span class="sxs-lookup"><span data-stu-id="7ad23-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="7ad23-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="7ad23-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    |  |
| <span data-ttu-id="7ad23-145">Paylaşılan bilgisayar etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="7ad23-145">Shared computer activation</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Office 365 E3 ile birlikte](../media/check-mark.png)| 
| <span data-ttu-id="7ad23-148">Win 7/8.1 Pro lisanslarından Windows 10 Pro'nun yükseltme hakları</span><span class="sxs-lookup"><span data-stu-id="7ad23-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    || 
| <span data-ttu-id="7ad23-150">**Bilgi koruması**</span><span class="sxs-lookup"><span data-stu-id="7ad23-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="7ad23-151">Office 365 Veri Kaybı Önleme</span><span class="sxs-lookup"><span data-stu-id="7ad23-151">Office 365 Data Loss Prevention</span></span>|    ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)|![Office 365 E3 ile birlikte](../media/check-mark.png)|
|<span data-ttu-id="7ad23-154">Azure Bilgi Koruma Planı 1, Bitlocker uygulaması</span><span class="sxs-lookup"><span data-stu-id="7ad23-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)||
|<span data-ttu-id="7ad23-156">Azure Bilgi Koruma Planı 1, Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="7ad23-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)||
|<span data-ttu-id="7ad23-158">**İstemci Erişim Lisansı (CAL hakları)**</span><span class="sxs-lookup"><span data-stu-id="7ad23-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="7ad23-159">Kurumsal CAL Paketi (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="7ad23-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Office 365 E3 ile birlikte](../media/check-mark.png)|

<span data-ttu-id="7ad23-161"><sup>1</sup> Office uygulamalarının Microsoft 365 Business Premium sürümü, Grup İlkesi, uygulama telemetrisi, denetimleri güncelleştirme, elektronik tablo karşılaştırma ve sorgulama veya iş Zekası yoluyla toplu etkinleştirme içermez.</span><span class="sxs-lookup"><span data-stu-id="7ad23-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="7ad23-162">Geçiş</span><span class="sxs-lookup"><span data-stu-id="7ad23-162">Migration</span></span>

<span data-ttu-id="7ad23-163">Aboneliğinizi geçirmek için, birkaç kişiyi Microsoft 365 Business Premium'a taşımak istiyorsanız, talimatları [el ile değiştir planlarına](../commerce/subscriptions/change-plans-manually.md) bakın.</span><span class="sxs-lookup"><span data-stu-id="7ad23-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="7ad23-164">E3 aboneliğinizi ve lisanslarınızı Microsoft 365 Business Premium aboneliğine taşımak için [herkesi otomatik olarak yükseltebilir](../commerce/subscriptions/upgrade-to-different-plan.md)veya bir iş ortağıyla birlikte çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7ad23-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="7ad23-165">Aşağıdaki bölümlerde, varsa yapmanız gereken değişiklikleri ve geçişten sonra neler yapabileceğiniz açıklanabilir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="7ad23-166">Office 365 E3 abonelik yapılandırması ve verileri</span><span class="sxs-lookup"><span data-stu-id="7ad23-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="7ad23-167">Geçiş yapmadan önce geçerli aboneliğinizde veya verilerinizde herhangi bir değişiklik yapmanız gerekmez:</span><span class="sxs-lookup"><span data-stu-id="7ad23-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="7ad23-168">DNS kayıtları ve etki alanı adları gibi abonelik yapılandırması.</span><span class="sxs-lookup"><span data-stu-id="7ad23-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="7ad23-169">Çok faktörlü kimlik doğrulama veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ve kimlik doğrulama ayarları.</span><span class="sxs-lookup"><span data-stu-id="7ad23-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="7ad23-170">Ekipler, Exchange Online posta kutuları, SharePoint Online siteleri, İş için OneDrive klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve verileri.</span><span class="sxs-lookup"><span data-stu-id="7ad23-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="7ad23-171">Office uygulamaları otomatik olarak ölçeklendirilir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-171">Office applications will scale automatically.</span></span> <span data-ttu-id="7ad23-172">Office 365 modern lisanslama, kullanıcının lisans atamasını her 72 saatte bir denetler ve Office uygulamalarını kullanıcı aboneliğiyle eşleşen sürüme dönüştürür.</span><span class="sxs-lookup"><span data-stu-id="7ad23-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="7ad23-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="7ad23-173">Windows 10</span></span>

<span data-ttu-id="7ad23-174">Windows'unuz Windows Pro Creator güncelleştirmesi kullanmıyorsa, [bunları Windows Pro Creators Update'e yükseltin.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="7ad23-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="7ad23-175">Kullanıcı aygıtlarını ve dosyalarını korumak için ilkeler ayarlama</span><span class="sxs-lookup"><span data-stu-id="7ad23-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="7ad23-176">Office 365 MDM ilkeleri ve aygıtları ayarlarsanız, bu aygıtlar Microsoft 365 yönetici merkezindeki **Cihazlar** sayfasında listelenir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="7ad23-177">Ayarladığınız tüm [ilkeler, Intune portalındaki](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasik ilkeler listesinde gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="7ad23-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="7ad23-178">Microsoft 365 Business Premium'a lisans lar atadıktan sonra, kullanıcıların aygıtlarını ve dosyalarını korumaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7ad23-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="7ad23-179">Kuruluşunuzdaki herkesi Microsoft 365 Business Premium'a yükselttiyseniz, Ana Sayfada kurulum sihirbazını görürsünüz ve dosyaları ve mobil aygıtları korumak için [kurulum sihirbazı adımlarında Microsoft 365 Business Premium'u](set-up.md) ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7ad23-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="7ad23-180">Ayrıca Cihazlar sayfasında aşağıdaki adımları tamamlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7ad23-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="7ad23-181">Yönetici merkezinde, sol navigasyonda Aygıt **Devices** \> **İlkeleri'ne**gidin.</span><span class="sxs-lookup"><span data-stu-id="7ad23-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="7ad23-182">Aygıt **ilkeleri** sayfasında **Ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="7ad23-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="7ad23-183">**İlke Ekle** bölmesinde ilke bir ad verin ve ardından açılan dan bir **İlke türü** seçin.</span><span class="sxs-lookup"><span data-stu-id="7ad23-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="7ad23-184">Android ve iPhone aygıtlarının yanı sıra Windows 10'daki dosyaları korumak için uygulama ilkeleri ayarlayabilir ve şirkete ait Windows 10 aygıtları için aygıt yapılandırma ilkeleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7ad23-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="7ad23-185">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="7ad23-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="7ad23-186">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="7ad23-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="7ad23-187">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="7ad23-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="7ad23-188">Windows 10 bilgisayarların aygıt koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="7ad23-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="7ad23-189">İlkeleri ayarladıktan sonra, siz ve çalışanlarınız aygıtlar ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7ad23-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="7ad23-190">Bkz. Windows aygıtları için adımlar [için Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlayın.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7ad23-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="7ad23-191">Bkz. Android telefonlar ve iPhone'lar için adımlar için [Microsoft 365 Business Premium kullanıcıları için mobil cihazlar ayarlama.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7ad23-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="7ad23-192">Tehdit koruması</span><span class="sxs-lookup"><span data-stu-id="7ad23-192">Threat protection</span></span>

<span data-ttu-id="7ad23-193">Microsoft 365 Business Premium'a geçtikten sonra Office 365 ATP'niz var.</span><span class="sxs-lookup"><span data-stu-id="7ad23-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="7ad23-194">Genel bakış için [Office 365 ATP'ye](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) bakın.</span><span class="sxs-lookup"><span data-stu-id="7ad23-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="7ad23-195">Kurmak için, [ATP güvenli bağlantılar kurmak,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa) [ATP güvenli ekleri kurmak](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)ve [ATP anti-phishing kurmak](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)bakın.</span><span class="sxs-lookup"><span data-stu-id="7ad23-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="7ad23-196">Duyarlılık etiketleri</span><span class="sxs-lookup"><span data-stu-id="7ad23-196">Sensitivity labels</span></span>

<span data-ttu-id="7ad23-197">Duyarlılık etiketleri kullanmaya başlamak için duyarlılık [etiketlerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) bölümüne bakın ve duyarlılık etiketleri videosu [oluşturun ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="7ad23-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
