---
title: Microsoft 365 Business 'da Azure AD ile birleştirilmiş cihazından şirket içi kaynaklara erişme
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Bir Azure Active Directory 'de Windows 10 aygıtından iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim almayı öğrenin.
ms.openlocfilehash: 9b83781afee746b06bbdf90962de0f55ffbcb118
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47307503"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="586de-103">Microsoft 365 Business Premium 'da Azure AD ile birleştirilmiş cihazından şirket içi kaynaklara erişme</span><span class="sxs-lookup"><span data-stu-id="586de-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="586de-104">Bu makale Microsoft 365 Business Premium için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="586de-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="586de-105">Azure Active Directory 'deki herhangi bir Windows 10 aygıtının, Microsoft 365 uygulamalarınız gibi tüm bulut tabanlı kaynaklara erişimi vardır ve Microsoft 365 Business Premium tarafından korunabilir.</span><span class="sxs-lookup"><span data-stu-id="586de-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="586de-106">Ayrıca, iş kolu (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim izni verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="586de-107">Erişime izin vermek için, şirket içi Active Directory 'yi Azure Active Directory ile eşitlemek üzere [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) 'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="586de-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="586de-108">Daha fazla bilgi edinmek için [Azure Active Directory 'de cihaz yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="586de-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="586de-109">Adımlar aşağıdaki bölümlerde de özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="586de-109">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="586de-110">Bu yordam yalnızca OAuth ve NTLM için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="586de-110">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="586de-111">Kerberos desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="586de-111">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="586de-112">Azure AD Connect 'i çalıştırır</span><span class="sxs-lookup"><span data-stu-id="586de-112">Run Azure AD Connect</span></span>

<span data-ttu-id="586de-113">Kuruluşunuzun Azure AD birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="586de-113">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="586de-114">Kullanıcıları, grupları ve kişilerinizi yerel Active Directory 'den Azure Active Directory 'ye eşitlemek için, [Office 365 için dizin eşitlemeyi ayarlama](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)başlığı altında açıklandığı gibi dizin eşitleme Sihirbazı 'Nı ve Azure AD Connect 'i çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-114">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="586de-115">Dizin eşitleme işlemi tamamlandıktan sonra, kuruluşunuzun Windows 10 cihazlarının Azure AD 'de bulunduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="586de-115">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="586de-116">Bu adım her Windows 10 cihazında tek tek yapılır.</span><span class="sxs-lookup"><span data-stu-id="586de-116">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="586de-117">Ayrıntılar için [Microsoft 365 Business Premium kullanıcıları Için Windows cihazlarını ayarlama](set-up-windows-devices.md) bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="586de-117">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="586de-118">Windows 10 cihazları Azure AD 'e eklendiğinde, her kullanıcının cihazlarını yeniden başlatması ve Microsoft 365 Iş ekstra kimlik bilgileriyle oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="586de-118">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="586de-119">Tüm aygıtların artık şirket içi kaynaklara erişimi vardır.</span><span class="sxs-lookup"><span data-stu-id="586de-119">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="586de-120">Azure AD birleştirilmiş cihazları için şirket içi kaynaklara erişim için ek adım gerekmez.</span><span class="sxs-lookup"><span data-stu-id="586de-120">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="586de-121">Bu işlev Windows 10 ' da yerleşiktir.</span><span class="sxs-lookup"><span data-stu-id="586de-121">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="586de-122">WHFB kimlik bilgisi oturumu aracılığıyla PIN/Bio-metrik gibi parola yöntemi dışında, AYARLANABILIR bir cihazda oturum açma planınız varsa ve şirket içi kaynaklara (paylaşımlar, yazıcılar... vb), lütfen takip edin https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="586de-122">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="586de-123">Kuruluşunuz, yukarıda açıklanan Azure AD birleştirilmiş cihaz yapılandırmasında dağıtmaya hazır değilse, [karma Azure AD birleştirilmiş cihaz yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-123">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="586de-124">Windows cihazları Azure AD 'ye katıldığınızda dikkat edilecek noktalar</span><span class="sxs-lookup"><span data-stu-id="586de-124">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="586de-125">Azure-AD 'a katıldığınız Windows cihazı daha önce etki alanına veya bir çalışma grubunda yer alıyorsa aşağıdaki sınırlamaları dikkate alın:</span><span class="sxs-lookup"><span data-stu-id="586de-125">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="586de-126">Bir cihaz Azure AD birleştirdiğinde, var olan bir profile başvurulmadan yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="586de-126">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="586de-127">Profiller el ile geçirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="586de-127">Profiles must be manually migrated.</span></span> <span data-ttu-id="586de-128">Kullanıcı profili, sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="586de-128">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="586de-129">En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için üçüncü taraf bir aracı bulmalıdır.</span><span class="sxs-lookup"><span data-stu-id="586de-129">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="586de-130">Cihaz grup Ilkesi nesnelerini (GPO) kullanıyorsa, bazı GPO 'Larda karşılaştırılabilir bir [yapılandırma hizmeti sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="586de-130">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="586de-131">Var olan GPO 'Lara benzer CSP 'Leri bulmak için [Mvade aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-131">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="586de-132">Kullanıcılar, Active Directory kimlik doğrulamasına bağlı uygulamalarda kimlik doğrulaması yapamaz.</span><span class="sxs-lookup"><span data-stu-id="586de-132">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="586de-133">Eski uygulamayı değerlendirin ve mümkünse modern kimlik doğrulama kullanan bir uygulamaya güncelleştirmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-133">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="586de-134">Active Directory yazıcı keşfi çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="586de-134">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="586de-135">Tüm kullanıcılar için doğrudan yazıcı yolları sağlayabilir veya [karma bulut yazdırma](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="586de-135">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
