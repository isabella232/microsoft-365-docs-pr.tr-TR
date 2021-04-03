---
title: Microsoft 365 İş'te Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara erişme
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Azure Active Directory'ye katılmış bir Windows 10 cihazından iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişmeyi öğrenin.
ms.openlocfilehash: 27549d6c3b03413f2f05c69845caad155333ca97
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580324"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="fac3e-103">Microsoft 365 İş Ekstra'da Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara erişme</span><span class="sxs-lookup"><span data-stu-id="fac3e-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="fac3e-104">Bu makale Microsoft 365 İş Ekstra için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fac3e-105">Azure Active Directory'ye katılmış tüm Windows 10 cihazlarında, Microsoft 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişimi vardır ve Microsoft 365 İş Ekstra tarafından korunabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fac3e-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="fac3e-106">Ayrıca iş hattı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişime izin veabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fac3e-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="fac3e-107">Erişime izin vermek [için, Şirket içi](/azure/active-directory/connect/active-directory-aadconnect) Active Directory'nizi Azure Active Directory ile eşitlemek için Azure AD Connect'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="fac3e-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="fac3e-108">Daha fazla bilgi edinmek için [Bkz. Azure Active Directory'de cihaz yönetimine giriş.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="fac3e-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="fac3e-109">Adımlar aşağıdaki bölümlerde de özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="fac3e-110">Azure AD Connect'i çalıştırma</span><span class="sxs-lookup"><span data-stu-id="fac3e-110">Run Azure AD Connect</span></span>

<span data-ttu-id="fac3e-111">Kuruma katılan Azure AD cihazlarının şirket içi kaynaklara erişmesi için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="fac3e-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="fac3e-112">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'ye eşitlemek için, [Office 365](../enterprise/set-up-directory-synchronization.md)için dizin eşitlemesini ayarlama konusunda açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="fac3e-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>
    
2. <span data-ttu-id="fac3e-113">Dizin eşitlemesi tamamlandıktan sonra, kuruluşun Windows 10 cihazlarının Azure AD'ye katıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="fac3e-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="fac3e-114">Bu adım, her Windows 10 cihazında ayrı ayrı yapılır.</span><span class="sxs-lookup"><span data-stu-id="fac3e-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="fac3e-115">Ayrıntılar [için Bkz. Microsoft 365 İş Ekstra kullanıcıları](set-up-windows-devices.md) için Windows cihazlarını ayarlama.</span><span class="sxs-lookup"><span data-stu-id="fac3e-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="fac3e-116">Windows 10 cihazları Azure AD'ye katıldıktan sonra, her kullanıcının cihazlarını yeniden başlatması ve Microsoft 365 İş Ekstra kimlik bilgileriyle oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="fac3e-117">Artık tüm cihazlara şirket içi kaynaklara da erişebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fac3e-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="fac3e-118">Azure AD'ye katılmış cihazlar için şirket içi kaynaklara erişmek için ek adım gerekmez.</span><span class="sxs-lookup"><span data-stu-id="fac3e-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="fac3e-119">Bu işlev Windows 10'da yerleşik olarak yer alan bir işlevdir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="fac3e-120">WHFB kimlik bilgileriyle oturum açma yoluyla PIN/Biyometrik gibi parola yöntemi dışında AADJ cihazında oturum açma ve ardından şirket içi kaynaklara (paylaşımlar,yazıcılar) erişme planlarınız varsa. vb. gibi) lütfen https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="fac3e-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="fac3e-121">Organizasyonunız yukarıda açıklanan Azure AD'ye katılmış cihaz yapılandırmasında dağıtmaya hazır değilse, Karma Azure AD Katıldı cihaz [yapılandırmasını ayarlamayı göz önünde bulundurabilirsiniz.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="fac3e-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="fac3e-122">Windows cihazlarıyla Azure AD'ye katılırken dikkat edilmesi gereken noktalar</span><span class="sxs-lookup"><span data-stu-id="fac3e-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="fac3e-123">Azure-AD'ye katıldığınız Windows cihazı daha önce etki alanına katılmış veya bir çalışma grubunda yer alan bir cihazsa, aşağıdaki sınırlamaları göz önünde önünde önünde düşünün:</span><span class="sxs-lookup"><span data-stu-id="fac3e-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="fac3e-124">Azure AD'nin bir cihaz birleştirmesi, var olan bir profile başvurmadan yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="fac3e-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="fac3e-125">Profillerin el ile geçirilir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="fac3e-126">Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlangıç menüsü ayarları gibi bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="fac3e-127">Mevcut dosyaları ve ayarları yeni profile eşlemek için üçüncü taraf bir araç bulmak en iyi yaklaşımdır.</span><span class="sxs-lookup"><span data-stu-id="fac3e-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="fac3e-128">Cihaz Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPOS'ların Intune'da karşılaştırılabilir bir Yapılandırma Hizmeti Sağlayıcısı [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olabilir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="fac3e-129">Mevcut [GPO'lar](https://www.microsoft.com/download/details.aspx?id=45520) için benzer CSP'leri bulmak için MMAT aracını çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="fac3e-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="fac3e-130">Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulamasına sahip olamayabilecektir.</span><span class="sxs-lookup"><span data-stu-id="fac3e-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="fac3e-131">Eski uygulamayı değerlendirin ve mümkünse modern Kimlik Doğrulaması kullanan bir uygulamaya güncelleştirmeyi göz önünde bulundurabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fac3e-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="fac3e-132">Active Directory yazıcı bulma çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="fac3e-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="fac3e-133">Tüm kullanıcılar için doğrudan yazıcı yolları s sağlama veya [Evrensel Yazdırma'ı kullanabilirsiniz.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="fac3e-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="fac3e-134">İlgili Makaleler</span><span class="sxs-lookup"><span data-stu-id="fac3e-134">Related Articles</span></span>

[<span data-ttu-id="fac3e-135">Azure AD Connect için önkoşullar</span><span class="sxs-lookup"><span data-stu-id="fac3e-135">Prerequisites for Azure AD Connect</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
