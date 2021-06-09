---
title: Şirket içinde Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara Microsoft 365 İş
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
description: İş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara bir Azure Active Directory bir Windows 10 öğrenin.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843332"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="325bf-103">Şirket içinde Azure AD'ye katılmış bir cihazdan şirket içi kaynaklara Microsoft 365 İş Ekstra</span><span class="sxs-lookup"><span data-stu-id="325bf-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="325bf-104">Bu makale diğer Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="325bf-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="325bf-105">Bir Windows 10 bağlı Azure Active Directory cihaz, Microsoft 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişim iznine sahip olur ve Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="325bf-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="325bf-106">Ayrıca iş alanı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim izni de veebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="325bf-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="325bf-107">Erişime izin vermek [için, Azure AD Bağlan'i](/azure/active-directory/connect/active-directory-aadconnect) kullanarak şirket içi Active Directory'nizi diğer Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="325bf-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="325bf-108">Daha fazla bilgi edinmek için [bkz. Azure Active Directory'da cihaz yönetimine giriş.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="325bf-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="325bf-109">Adımlar aşağıdaki bölümlerde da özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="325bf-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="325bf-110">Azure AD Bağlan'i çalıştırma</span><span class="sxs-lookup"><span data-stu-id="325bf-110">Run Azure AD Connect</span></span>

<span data-ttu-id="325bf-111">Azure AD'ye katılmış cihazlarının şirket içi kaynaklara erişmesi için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="325bf-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="325bf-112">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Active Directory'e eşitlemek için, Office 365 için dizin eşitlemesini ayarlama konusunda açıklandığı gibi Dizin eşitleme sihirbazını Bağlan Azure AD [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="325bf-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="325bf-113">Dizin eşitlemesi tamamlandıktan sonra, tüm kuruluş cihazlarında Azure AD'Windows 10 bağlı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="325bf-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="325bf-114">Bu adım her cihazda ayrı Windows 10 yapılır.</span><span class="sxs-lookup"><span data-stu-id="325bf-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="325bf-115">Ayrıntılar [için Windows cihazları Microsoft 365 İş Ekstra'ya](set-up-windows-devices.md) bakın.</span><span class="sxs-lookup"><span data-stu-id="325bf-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="325bf-116">Cihaz Windows 10 Azure AD'ye katıldıktan sonra, her kullanıcının cihazlarını yeniden başlatması ve kendi kullanıcı kimlik bilgileriyle Microsoft 365 İş Ekstra gerekir.</span><span class="sxs-lookup"><span data-stu-id="325bf-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="325bf-117">Tüm cihazlar artık şirket içi kaynaklara da erişime sahip.</span><span class="sxs-lookup"><span data-stu-id="325bf-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="325bf-118">Azure AD'ye katılmış cihazlar için şirket içi kaynaklara erişmek için ek adımlar gerekmez.</span><span class="sxs-lookup"><span data-stu-id="325bf-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="325bf-119">Bu işlevsellik yeni bir Windows 10.</span><span class="sxs-lookup"><span data-stu-id="325bf-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="325bf-120">PIN/Biyometrik WHFB kimlik bilgileri aracılığıyla oturum açma gibi parola yöntemi dışında bir AADJ cihazında oturum açma ve ardından şirket içi kaynaklara (paylaşımlar, yazıcılar, vb.) erişme planlarınız varsa, lütfen bu [makaleyi izleyin.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="325bf-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="325bf-121">Organizasyon, yukarıda açıklanan Azure AD'ye katılmış cihaz yapılandırmasını dağıtmaya hazır değilse, Azure AD'ye Katılan Karma cihaz yapılandırmasını [ayarlamayı göz önünde bulundurabilirsiniz.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="325bf-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="325bf-122">Windows cihazları Azure AD'ye katılırken dikkate alınacak noktalar</span><span class="sxs-lookup"><span data-stu-id="325bf-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="325bf-123">Azure-AD Windows katıldığınız tüm cihaz daha önce etki alanına katılmış veya bir çalışma grubunda yer alan bir cihazsa, aşağıdaki sınırlamaları göz önünde önünde Windows:</span><span class="sxs-lookup"><span data-stu-id="325bf-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="325bf-124">Bir Azure AD birleştirme cihazı katsıyorsa, var olan profile başvurmak gerekmeden yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="325bf-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="325bf-125">Profillerin el ile geçişi gerekir.</span><span class="sxs-lookup"><span data-stu-id="325bf-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="325bf-126">Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="325bf-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="325bf-127">Mevcut dosyaları ve ayarları yeni profile eşlemek için bir üçüncü taraf aracı bulmak en iyi yaklaşımdır.</span><span class="sxs-lookup"><span data-stu-id="325bf-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="325bf-128">Cihaz Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPOS'ların Intune'da benzer bir Yapılandırma Hizmeti Sağlayıcısı [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) yok olabilir.</span><span class="sxs-lookup"><span data-stu-id="325bf-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="325bf-129">Var olan [GPOS'lar](https://www.microsoft.com/download/details.aspx?id=45520) için karşılaştırılabilir CSP'leri bulmak için MMAT aracını çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="325bf-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="325bf-130">Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulaması işlemi görenemmektedir.</span><span class="sxs-lookup"><span data-stu-id="325bf-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="325bf-131">Eski uygulamayı değerlendirin ve mümkünse modern Kimlik Doğrulaması kullanan bir uygulamaya güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="325bf-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="325bf-132">Active Directory yazıcı bulma işe yaramadı.</span><span class="sxs-lookup"><span data-stu-id="325bf-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="325bf-133">Tüm kullanıcılar için doğrudan yazıcı yolları s sağlamanın veya Evrensel [Yazdırma'nın kullanımını sebilirsiniz.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="325bf-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="325bf-134">İlgili Makaleler</span><span class="sxs-lookup"><span data-stu-id="325bf-134">Related Articles</span></span>

[<span data-ttu-id="325bf-135">Azure AD aboneliğinin önkoşulları Bağlan</span><span class="sxs-lookup"><span data-stu-id="325bf-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
