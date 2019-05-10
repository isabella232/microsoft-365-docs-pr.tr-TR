---
title: Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: İş kolu uygulamaları, dosya paylaşımları ve yazıcılar Azure Active Directory'den Windows 10 aygıt katıldı gibi yerinde kaynaklara erişmek nasıl öğrenin.
ms.openlocfilehash: 2be8eb16b9d17547d3bc4c3e4fe499b4c14117a4
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660279"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="7159d-103">Erişim yerinde Azure AD alanına aygıttan Microsoft 365 iş kaynakları</span><span class="sxs-lookup"><span data-stu-id="7159d-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="7159d-104">Azure Active Directory alanına dahil olan herhangi bir Windows 10 aygıt Office 365 uygulamalarınızı gibi tüm bulut tabanlı kaynaklara erişebilir ve Microsoft 365 işletme tarafından korunabilir.</span><span class="sxs-lookup"><span data-stu-id="7159d-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="7159d-105">Ayrıca şirket içi iş satır (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi kaynaklar için erişim sağlamak için [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)kullanarak, şirket içi Active Directory Azure Active Directory ile eşitlenmelidir.</span><span class="sxs-lookup"><span data-stu-id="7159d-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> <span data-ttu-id="7159d-106">Daha fazla bilgi için [Aygıt Yönetimi Azure Active Directory'de giriş](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="7159d-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="7159d-107">Bağlanma Azure AD Çalıştır</span><span class="sxs-lookup"><span data-stu-id="7159d-107">Run Azure AD Connect</span></span>

<span data-ttu-id="7159d-108">Şirket içi kaynaklara erişmek, kuruluşunuzun Azure AD alanına bağlı aygıtları etkinleştirmek için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="7159d-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="7159d-109">Azure Active Directory'ye, kullanıcıları, grupları ve yerel Active Directory'den kişileri eşitlemek için dizin eşitleme Sihirbazı'nı çalıştırın ve [Office 365 için'dizin eşitlemeyi ayarlamak](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)Azure AD Bağlan olarak açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="7159d-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="7159d-110">Dizin eşitleme tamamlandıktan sonra kuruluşunuzun Windows 10 aygıtları Azure AD alanına dahil olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7159d-110">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="7159d-111">Bu adım, tek tek her Windows 10 aygıtta yapılır.</span><span class="sxs-lookup"><span data-stu-id="7159d-111">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="7159d-112">[Microsoft 365 iş kullanıcıları için Windows aygıtları ayarlayın](set-up-windows-devices.md) ayrıntılı bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="7159d-112">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="7159d-113">Windows 10 aygıtları Azure AD alanına dahil olduğunda, her kullanıcının kendi aygıtları ve Microsoft 365 iş kimlik bilgileri ile oturum açma yeniden.</span><span class="sxs-lookup"><span data-stu-id="7159d-113">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="7159d-114">Tüm aygıtlar artık yerinde kaynaklara erişebilir.</span><span class="sxs-lookup"><span data-stu-id="7159d-114">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="7159d-115">Erişim aygıtları Azure Reklam kaynakları birleştirilmiş yerinde almak için hiçbir ek işlem gereklidir.</span><span class="sxs-lookup"><span data-stu-id="7159d-115">No additional steps are required to get access to on-premise resources for Azure AD joined devices.</span></span> <span data-ttu-id="7159d-116">Windows 10 kullanılabilir yerleşik işlevsellik budur.</span><span class="sxs-lookup"><span data-stu-id="7159d-116">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="7159d-117">Kuruluşunuzun Azure AD alanına bağlı aygıt yukarıda açıklanan yapılandırma dağıtmak hazır değilse, [karma Azure AD katılmış aygıt yapılandırması](manage-windows-devices.md)ayarlama göz önünde bulundurun.</span><span class="sxs-lookup"><span data-stu-id="7159d-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="7159d-118">Aygıtlarınızın Windows Azure AD katılırken dikkat edilmesi gereken noktalar</span><span class="sxs-lookup"><span data-stu-id="7159d-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="7159d-119">Azure AD katılmadan önce etki alanına katılmış Windows aygıtı varsa veya bir çalışma grubunda, aşağıdaki kısıtlamaları göz önüne almanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="7159d-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="7159d-120">Bir aygıtı Azure AD katıldığında, varolan bir profili başvurulmadan yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="7159d-120">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="7159d-121">Bu sorunu gidermek için profillerini el ile geçirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="7159d-121">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="7159d-122">Kullanıcı profili, Sık Kullanılanlar, yerel dosyalar, tarayıcı ayarlarını, Başlat menüsü ayarlarını, vb. gibi bilgileri içerir. Varolan dosyalarınızı ve ayarlarınızı yeni profile eşlemek için bir üçüncü taraf aracı bulmak için en iyi yaklaşım olduğunu</span><span class="sxs-lookup"><span data-stu-id="7159d-122">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="7159d-123">Grup İlkesi nesneleri (GPO) aygıtı kullanıyor olsa da, bazı GPO'ları bir karşılaştırılabilir [Yapılandırma hizmeti sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) içinde Intune olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="7159d-123">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="7159d-124">Varolan GPO'lar için karşılaştırılabilir CSP bulmak için [MMAT aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="7159d-124">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="7159d-125">Active Directory kimlik doğrulamasını kullanan uygulamalar için kimlik doğrulama olanağınız olur.</span><span class="sxs-lookup"><span data-stu-id="7159d-125">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="7159d-126">Çalışılabilecek bu eski bir uygulama kullanarak değerlendirmek ve mümkünse modern kimlik doğrulama kullanan bir uygulama için güncelleştirme göz önünde bulundurun.</span><span class="sxs-lookup"><span data-stu-id="7159d-126">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="7159d-127">Active Directory yazıcı bulma çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="7159d-127">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="7159d-128">Bu sorunu gidermek için tüm kullanıcılar için doğrudan yazıcı yolları sağlamak veya [Karma bulut baskı](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)yelpazesinin.</span><span class="sxs-lookup"><span data-stu-id="7159d-128">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
