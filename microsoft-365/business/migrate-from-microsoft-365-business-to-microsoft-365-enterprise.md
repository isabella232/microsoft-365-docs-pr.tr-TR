---
title: Microsoft 365 Business'tan Microsoft 365 E3'e geçiş
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: İşletmenizi Microsoft 365 Business Premium'dan Microsoft 365 E3'e nasıl taşıyacın öğrenin.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081921"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="267be-103">Microsoft 365 Business Premium'dan Microsoft 365 E3'e geçiş</span><span class="sxs-lookup"><span data-stu-id="267be-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="267be-104">Microsoft 365 Business Premium, çalışanlarınızın en iyi işlerini yapmalarını sağlayan basit cihaz yönetimi ve güvenlikle sınıfının en iyisi bulut tabanlı üretkenlik uygulamalarını birleştirerek küçük işletmeniz için ihtiyacınız olan her şeye sahiptir.</span><span class="sxs-lookup"><span data-stu-id="267be-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="267be-105">Ancak bazı durumlarda, Microsoft 365 Business Premium aboneliğinizi Microsoft 365 E3'e geçirmeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="267be-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="267be-106">Örneğin, işletmeniz büyüdü ve 300'den fazla lisansa ihtiyacı var (tebrikler, bu arada).</span><span class="sxs-lookup"><span data-stu-id="267be-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="267be-107">Veya işletmenizin kurumsal için Microsoft 365 Uygulamaları, Windows 10 Kurumsal E3 veya Kurumsal İstemci Erişim Lisansları (CALs) gibi kurumsal özelliklere ihtiyacı vardır.</span><span class="sxs-lookup"><span data-stu-id="267be-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="267be-108">Yükseltme kolaydır: [Yükseltmeyi Yönetici merkezinden](../commerce/subscriptions/upgrade-to-different-plan.md)başlatabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="267be-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="267be-109">Geçerli aboneliğinizdeki tüm verileriniz ve yapılandırmanız korunur.</span><span class="sxs-lookup"><span data-stu-id="267be-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="267be-110">Geçişe hazırlanmak için yapacak bir şeyiniz yok ve yeni özelliklerden yararlanmak dışında daha sonra yapacak bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="267be-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="267be-111">Ayrıca 300'e kadar koltuk için Microsoft 365 Business Premium aboneliği kullanabilir ve 300'den fazla koltuk için Microsoft 365 E3 aboneliği alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="267be-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="267be-112">Ancak, Office 365 ATP Microsoft 365 E3 dahil değildir.</span><span class="sxs-lookup"><span data-stu-id="267be-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="267be-113">Sürekli tehdit koruması için, Office 365 ATP polisleriniz kapsamındaki tüm kullanıcıların lisanslı olması için ek Office 365 ATP lisansları eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="267be-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="267be-114">Microsoft 365 Business Premium ve Microsoft 365 Enterprise arasındaki farklar</span><span class="sxs-lookup"><span data-stu-id="267be-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="267be-115">Bu tablo, Microsoft 365 Business Premium ve Microsoft 365 E3 arasındaki farkları gösterir.</span><span class="sxs-lookup"><span data-stu-id="267be-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="267be-116">Özellik</span><span class="sxs-lookup"><span data-stu-id="267be-116">Feature</span></span>    | <span data-ttu-id="267be-117">Microsoft 365 Business Premium desteği</span><span class="sxs-lookup"><span data-stu-id="267be-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="267be-118">Microsoft 365 E3 desteği</span><span class="sxs-lookup"><span data-stu-id="267be-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="267be-119">**Şirket içi**</span><span class="sxs-lookup"><span data-stu-id="267be-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="267be-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="267be-120">Windows 10</span></span>    | <span data-ttu-id="267be-121">Windows 10 İş</span><span class="sxs-lookup"><span data-stu-id="267be-121">Windows 10 Business</span></span>  |     <span data-ttu-id="267be-122">Windows 10 Kurumsal E3</span><span class="sxs-lookup"><span data-stu-id="267be-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="267be-123">Ofis uygulamaları\*</span><span class="sxs-lookup"><span data-stu-id="267be-123">Office apps\*</span></span>    | [<span data-ttu-id="267be-124">Microsoft 365 İş uygulamaları</span><span class="sxs-lookup"><span data-stu-id="267be-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="267be-125">Kurumsal uygulamalar için Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="267be-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="267be-126">**Bulut üretkenliği uygulamaları**</span><span class="sxs-lookup"><span data-stu-id="267be-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="267be-127">Exchange Online ve Outlook</span><span class="sxs-lookup"><span data-stu-id="267be-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="267be-128">Posta kutusu başına 50 GB depolama sınırı ve sınırsız Exchange Online arşivleme</span><span class="sxs-lookup"><span data-stu-id="267be-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="267be-129">Posta kutusu başına 100 GB depolama sınırı ve sınırsız Exchange Online arşivleme</span><span class="sxs-lookup"><span data-stu-id="267be-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="267be-130">Takım</span><span class="sxs-lookup"><span data-stu-id="267be-130">Teams</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-133">OneDrive İş</span><span class="sxs-lookup"><span data-stu-id="267be-133">OneDrive for Business</span></span>    | <span data-ttu-id="267be-134">Kullanıcı başına 1 TB depolama sınırı</span><span class="sxs-lookup"><span data-stu-id="267be-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="267be-135">Sınırsız</span><span class="sxs-lookup"><span data-stu-id="267be-135">Unlimited</span></span> | 
| <span data-ttu-id="267be-136">Yammer, SharePoint Online, Planlayıcı, Akış</span><span class="sxs-lookup"><span data-stu-id="267be-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-139">Outlook Müşteri Yöneticisi, MileIQ</span><span class="sxs-lookup"><span data-stu-id="267be-139">Outlook Customer Manager, MileIQ</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | | 
| <span data-ttu-id="267be-141">**Tehdit Koruması**</span><span class="sxs-lookup"><span data-stu-id="267be-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="267be-142">Saldırı yüzey azaltma yetenekleri</span><span class="sxs-lookup"><span data-stu-id="267be-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="267be-143">Bu listeye bakın</span><span class="sxs-lookup"><span data-stu-id="267be-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="267be-144">Microsoft Edge için donanım tabanlı yalıtımın kurumsal yönetimi</span><span class="sxs-lookup"><span data-stu-id="267be-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="267be-145">Office 365 Gelişmiş Tehdit Koruması (ATP) Planı 1</span><span class="sxs-lookup"><span data-stu-id="267be-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | <span data-ttu-id="267be-147">Dahil değil, ancak eklenebilir</span><span class="sxs-lookup"><span data-stu-id="267be-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="267be-148">**Kimlik yönetimi**</span><span class="sxs-lookup"><span data-stu-id="267be-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="267be-149">Karma Azure Etkin Dizin (Azure AD) hesapları, Azure çok faktörlü kimlik doğrulama (MFA), Koşullu Erişim, şirket içi kimlikler için parola yazma için self servis parola sıfırlama</span><span class="sxs-lookup"><span data-stu-id="267be-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-152">Bulut Uygulaması Bulma, Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="267be-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-154">Azure AD Office 365 uygulamaları Tek Oturum Açma (SSO): Kullanıcı başına 10 uygulama (Salesforce gibi Galeri SaaS uygulamaları)\*</span><span class="sxs-lookup"><span data-stu-id="267be-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-157">Azure AD Premium 1 SSO: limitsiz (Azure AD Uygulama Proxy'si aracılığıyla şirket içi uygulamalar ve Self Servis Uygulama Tümleştirme şablonlarını kullanan galeri dışı uygulamalar)</span><span class="sxs-lookup"><span data-stu-id="267be-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-159">**Cihaz ve uygulama yönetimi**</span><span class="sxs-lookup"><span data-stu-id="267be-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="267be-160">Microsoft Intune, Windows Otomatik Pilot</span><span class="sxs-lookup"><span data-stu-id="267be-160">Microsoft Intune, Windows Autopilot</span></span>|     ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|<span data-ttu-id="267be-163">Sanal Masaüstü Erişimi (VDA)</span><span class="sxs-lookup"><span data-stu-id="267be-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|<span data-ttu-id="267be-165">Windows Sanal Masaüstü (WVD)</span><span class="sxs-lookup"><span data-stu-id="267be-165">Windows Virtual Desktop (WVD)</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
|<span data-ttu-id="267be-168">Paylaşılan Bilgisayar Etkinleştirme (SCA)</span><span class="sxs-lookup"><span data-stu-id="267be-168">Shared Computer Activation (SCA)</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png) |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-171">Microsoft Masaüstü Optimizasyon Paketi</span><span class="sxs-lookup"><span data-stu-id="267be-171">Microsoft Desktop Optimization Package</span></span>    | |     ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-173">**Bilgi koruması**</span><span class="sxs-lookup"><span data-stu-id="267be-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="267be-174">Office 365 Veri Kaybıönleme, Azure Bilgi Koruma Planı 1</span><span class="sxs-lookup"><span data-stu-id="267be-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-177">Uç nokta DLP için Pencere Bilgi Koruması</span><span class="sxs-lookup"><span data-stu-id="267be-177">Window Information Protection for endpoint DLP</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-180">**İstemci Erişim Lisansı (CAL hakları)**</span><span class="sxs-lookup"><span data-stu-id="267be-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="267be-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Hakları Yönetimi)</span><span class="sxs-lookup"><span data-stu-id="267be-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-183">**Uyumlu -luk**</span><span class="sxs-lookup"><span data-stu-id="267be-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="267be-184">Sınırsız e-posta arşivleme</span><span class="sxs-lookup"><span data-stu-id="267be-184">Unlimited email archiving</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-187">Uyumluluk Puanı/Uyumluluk Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="267be-187">Compliance Score/Compliance Manager</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-190">Ediscovery</span><span class="sxs-lookup"><span data-stu-id="267be-190">eDiscovery</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-193">Yerinde bekleme ve dava tutma</span><span class="sxs-lookup"><span data-stu-id="267be-193">In-place hold and litigation hold</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
| <span data-ttu-id="267be-196">Mesajlaşma Kayıtları Yönetimi (MRM) bekletme etiketleri ve bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="267be-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Microsoft 365 Business Premium'a dahildir](../media/check-mark.png)    | ![Microsoft 365 E3 ile birlikte](../media/check-mark.png) | 
||||

<span data-ttu-id="267be-199">\*SaaS uygulamalarına erişim izni alan kullanıcılar, SSO'nun en fazla 10 uygulamaya erişebiliyor.</span><span class="sxs-lookup"><span data-stu-id="267be-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="267be-200">Yöneticiler SSO'yı yapılandırabilir ve kullanıcı erişimini farklı SaaS uygulamalarına değiştirebilir, ancak SSO erişimine aynı anda kullanıcı başına yalnızca 10 uygulama için izin verilir.</span><span class="sxs-lookup"><span data-stu-id="267be-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="267be-201">Tüm Office 365 uygulamaları tek bir uygulama olarak sayılır.</span><span class="sxs-lookup"><span data-stu-id="267be-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="267be-202">Geçiş</span><span class="sxs-lookup"><span data-stu-id="267be-202">Migration</span></span>

<span data-ttu-id="267be-203">Geçiş yapmak için, Microsoft 365 Business Premium aboneliğinizi ve lisanslarınızı lisansları olan uygun bir Microsoft 365 E3 aboneliğine taşımak için iş ortağınızla birlikte çalışın.</span><span class="sxs-lookup"><span data-stu-id="267be-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="267be-204">Aşağıdaki bölümlerde, varsa hangi değişiklikleri yapmanız gerektiği ve geçişten sonra neler yapabileceğiniz açıklanabilir.</span><span class="sxs-lookup"><span data-stu-id="267be-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="267be-205">Microsoft 365 abonelik yapılandırması ve verileri</span><span class="sxs-lookup"><span data-stu-id="267be-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="267be-206">Geçiş yapmadan önce geçerli aboneliğinizde veya verilerinizde herhangi bir değişiklik yapmanız gerekmez:</span><span class="sxs-lookup"><span data-stu-id="267be-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="267be-207">DNS etki alanı adları gibi abonelik yapılandırması.</span><span class="sxs-lookup"><span data-stu-id="267be-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="267be-208">Çok faktörlü kimlik doğrulama veya koşullu erişim ilkeleri gibi kullanıcı ve grup hesapları ve kimlik doğrulama ayarları.</span><span class="sxs-lookup"><span data-stu-id="267be-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="267be-209">Ekipler, Exchange Online posta kutuları, SharePoint Online siteleri, İş için OneDrive klasörleri ve OneNote not defterleri gibi üretkenlik hizmeti yapılandırmaları ve verileri.</span><span class="sxs-lookup"><span data-stu-id="267be-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="267be-210">Kullanıcılarınız artık Exchange Online posta kutularında ve İş için OneDrive klasörlerinde sınırsız depolama alanının keyfini çıkarabilir.</span><span class="sxs-lookup"><span data-stu-id="267be-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="267be-211">10'dan fazla uygulama için Cloud App Discovery, Azure AD Connect Health ve SSO'yı kullanmaya başlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="267be-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="267be-212">Microsoft 365 E3'e geçirilen kullanıcılar artık Outlook Müşteri Yöneticisi ve MileIQ kullanamaz.</span><span class="sxs-lookup"><span data-stu-id="267be-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="267be-213">Tehdit koruması</span><span class="sxs-lookup"><span data-stu-id="267be-213">Threat protection</span></span>

<span data-ttu-id="267be-214">Windows 10 İş bu korumaları içerir:</span><span class="sxs-lookup"><span data-stu-id="267be-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="267be-215">İşletim sistemi önyükleme işleminin bütünlük uygulaması</span><span class="sxs-lookup"><span data-stu-id="267be-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="267be-216">Hassas işletim bileşenlerinin bütünlük zorlama</span><span class="sxs-lookup"><span data-stu-id="267be-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="267be-217">Gelişmiş güvenlik açığı ve sıfır gün istismarı azaltımları</span><span class="sxs-lookup"><span data-stu-id="267be-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="267be-218">Microsoft Edge, Internet Explorer ve Chrome için itibar tabanlı ağ koruması</span><span class="sxs-lookup"><span data-stu-id="267be-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="267be-219">Ana bilgisayar tabanlı güvenlik duvarı</span><span class="sxs-lookup"><span data-stu-id="267be-219">Host-based firewall</span></span>
- <span data-ttu-id="267be-220">Ransomware azaltma</span><span class="sxs-lookup"><span data-stu-id="267be-220">Ransomware mitigations</span></span>
- <span data-ttu-id="267be-221">Microsoft Edge için donanım tabanlı yalıtım</span><span class="sxs-lookup"><span data-stu-id="267be-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="267be-222">Akıllı Güvenlik Grafiği ile desteklenen uygulama denetimi</span><span class="sxs-lookup"><span data-stu-id="267be-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="267be-223">Cihaz kontrolü (USB)</span><span class="sxs-lookup"><span data-stu-id="267be-223">Device control (USB)</span></span>
- <span data-ttu-id="267be-224">Web tabanlı tehditler için ağ koruması</span><span class="sxs-lookup"><span data-stu-id="267be-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="267be-225">Ev sahibi izinsiz giriş önleme kuralları</span><span class="sxs-lookup"><span data-stu-id="267be-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="267be-226">Windows 10 Enterprise E3, Microsoft Edge için donanım tabanlı yalıtımın kurumsal yönetimini de içerir.</span><span class="sxs-lookup"><span data-stu-id="267be-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="267be-227">Microsoft 365 E3'e geçirilen kullanıcıların her biri sürekli tehdit koruması için bir Office 365 ATP lisansı gerektirir.</span><span class="sxs-lookup"><span data-stu-id="267be-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="267be-228">Office 365 ATP polisleriniz kapsamındaki tüm kullanıcıların lisanslı olması için ek Office 365 ATP lisansları satın aldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="267be-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="267be-229">Intune ile cihaz yönetimi</span><span class="sxs-lookup"><span data-stu-id="267be-229">Device management with Intune</span></span>

<span data-ttu-id="267be-230">Geçiş yapmadan önce kayıtlı aygıtlar, aygıtlar ve uygulama ayarlarını içeren geçerli Intune yapılandırmanızda herhangi bir değişiklik yapmanız gerekmez.</span><span class="sxs-lookup"><span data-stu-id="267be-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="267be-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="267be-231">Windows 10</span></span>

<span data-ttu-id="267be-232">Microsoft 365 Business Premium, Windows AutoPilot ile yükleyebileceğiniz Windows 10 Business'ı içerir.</span><span class="sxs-lookup"><span data-stu-id="267be-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="267be-233">Microsoft 365 E3'e geçiş yaptığınızda, her kullanıcı lisansı, Windows Autopilot ile de yükleyebileceğiniz Windows 10 Enterprise E3 içerir.</span><span class="sxs-lookup"><span data-stu-id="267be-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="267be-234">Microsoft 365 İş uygulamaları</span><span class="sxs-lookup"><span data-stu-id="267be-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="267be-235">Cihazlarınızda yüklü olan Microsoft 365 Apps iş istemcisi için Uygulamalarınız, kurumsal olarak Microsoft 365 Apps özelliklerini otomatik olarak kullanmaya başlar.</span><span class="sxs-lookup"><span data-stu-id="267be-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="267be-236">Geçişten sonra artık şunları kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="267be-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="267be-237">Grup İlkesi ile birim etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="267be-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="267be-238">Uygulama telemetrisi</span><span class="sxs-lookup"><span data-stu-id="267be-238">App telemetry</span></span>
 - <span data-ttu-id="267be-239">Denetimleri güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="267be-239">Update controls</span></span>
 - <span data-ttu-id="267be-240">Elektronik tablo karşılaştırın ve sorgulayın</span><span class="sxs-lookup"><span data-stu-id="267be-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="267be-241">İş zekası</span><span class="sxs-lookup"><span data-stu-id="267be-241">Business intelligence</span></span>

