---
title: Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Windows 10 aygıtına katılan bir Azure Active Directory'den iş uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara nasıl erişebilirsiniz öğrenin.
ms.openlocfilehash: fdc1eca6913ba6af4f6b65691fdee2165e7c827e
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323405"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="6e064-103">Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin</span><span class="sxs-lookup"><span data-stu-id="6e064-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="6e064-104">Azure Active Directory'nin birleştiği tüm Windows 10 aygıtları, Office 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişebilir ve Microsoft 365 Business tarafından korunabilir.</span><span class="sxs-lookup"><span data-stu-id="6e064-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="6e064-105">Ayrıca, iş satırı (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişime de izin verebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e064-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="6e064-106">Erişime izin vermek için, şirket içi Active Directory'nizi Azure Etkin Dizini ile senkronize etmek için [Azure AD Connect'i](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) kullanın.</span><span class="sxs-lookup"><span data-stu-id="6e064-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="6e064-107">Daha fazla bilgi için Azure [Active Directory'de aygıt yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction)'e bakın.</span><span class="sxs-lookup"><span data-stu-id="6e064-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="6e064-108">Adımlar da aşağıdaki bölümlerde özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="6e064-108">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="6e064-109">Azure AD Connect çalıştırın</span><span class="sxs-lookup"><span data-stu-id="6e064-109">Run Azure AD Connect</span></span>

<span data-ttu-id="6e064-110">Kuruluşunuzun Azure AD'sinin birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="6e064-110">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="6e064-111">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="6e064-111">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="6e064-112">Dizin eşitlemesi tamamlandıktan sonra, kuruluşunuzun Windows 10 aygıtlarının Azure AD'ye katıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="6e064-112">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="6e064-113">Bu adım her Windows 10 aygıtında ayrı ayrı yapılır.</span><span class="sxs-lookup"><span data-stu-id="6e064-113">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="6e064-114">Ayrıntılar [için Microsoft 365 Business kullanıcıları için Windows aygıtları ayarlama'ya](set-up-windows-devices.md) bakın.</span><span class="sxs-lookup"><span data-stu-id="6e064-114">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="6e064-115">Windows 10 aygıtları Azure AD'ye katıldıktan sonra, her kullanıcının aygıtlarını yeniden başlatması ve Microsoft 365 İş kimlik bilgileriyle oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6e064-115">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="6e064-116">Artık tüm aygıtlar şirket içi kaynaklara da erişebilir.</span><span class="sxs-lookup"><span data-stu-id="6e064-116">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="6e064-117">Azure AD'ye katılan aygıtlar için şirket içi kaynaklara erişmek için ek adım gerekmez.</span><span class="sxs-lookup"><span data-stu-id="6e064-117">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="6e064-118">Bu işlev Windows 10'da yerleşiktir.</span><span class="sxs-lookup"><span data-stu-id="6e064-118">This functionality is built into Windows 10.</span></span> 
  
<span data-ttu-id="6e064-119">Kuruluşunuz yukarıda açıklanan Azure AD birleştirilmiş aygıt yapılandırmasında kullanıma hazır değilse, [Karma Azure AD Joined aygıt yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünün.</span><span class="sxs-lookup"><span data-stu-id="6e064-119">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="6e064-120">Windows aygıtlarını Azure AD'ye katılırken dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="6e064-120">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="6e064-121">Azure-AD'nizin katıldığı Windows aygıtı daha önce etki alanına veya bir çalışma grubunda ysa, aşağıdaki sınırlamaları göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="6e064-121">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="6e064-122">Bir aygıt Azure AD katıldığında, varolan bir profile başvurmadan yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="6e064-122">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="6e064-123">Profiller el ile geçirilmelidir.</span><span class="sxs-lookup"><span data-stu-id="6e064-123">Profiles must be manually migrated.</span></span> <span data-ttu-id="6e064-124">Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları ve Başlat menüsü ayarları gibi bilgiler içerir.</span><span class="sxs-lookup"><span data-stu-id="6e064-124">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="6e064-125">En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için bir üçüncü taraf aracı bulmaktır.</span><span class="sxs-lookup"><span data-stu-id="6e064-125">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="6e064-126">Aygıt Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPO'larda Intune'da karşılaştırılabilir bir [Yapılandırma Hizmet Sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="6e064-126">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="6e064-127">Mevcut GPO'lar için karşılaştırılabilir CSP'ler bulmak için [MMAT aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="6e064-127">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="6e064-128">Kullanıcılar Active Directory kimlik doğrulamasına bağlı olan uygulamaların kimliğini doğrulayamaz.</span><span class="sxs-lookup"><span data-stu-id="6e064-128">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="6e064-129">Eski uygulamayı değerlendirin ve mümkünse modern Auth kullanan bir uygulamaya güncelleştirmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="6e064-129">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="6e064-130">Etkin Dizin yazıcısı bulma çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="6e064-130">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="6e064-131">Tüm kullanıcılar için doğrudan yazıcı yolları sağlayabilir veya [Karma Bulut Yazdırma'yı](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e064-131">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
