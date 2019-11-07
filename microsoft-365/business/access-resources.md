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
description: Windows 10 aygıtına katılan bir Azure Active Directory'den Line Of Business uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara nasıl erişebilirsiniz öğrenin.
ms.openlocfilehash: 2af5d4b4f84f39f5b157313e5b38ef030da7263d
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030544"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="8c729-103">Microsoft 365 Business'ta Azure AD ile birleştirilmiş bir cihazdan şirket içi kaynaklara erişin</span><span class="sxs-lookup"><span data-stu-id="8c729-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="8c729-104">Azure Active Directory'nin birleştiği tüm Windows 10 aygıtları Office 365 uygulamalarınız gibi bulut tabanlı tüm kaynaklara erişebilir ve Microsoft 365 Business tarafından korunabilir.</span><span class="sxs-lookup"><span data-stu-id="8c729-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="8c729-105">Ayrıca, Business Line (LOB) uygulamaları, dosya paylaşımları ve yazıcılar gibi şirket içi kaynaklara erişim eizin vermek için, [Azure AD Connect'i](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)kullanarak şirket içi Active Directory'nizi Azure Etkin Dizini ile eşitlemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="8c729-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="8c729-106">Daha fazla bilgi edinmek [için Azure Active Directory'de aygıt yönetimine giriş](https://docs.microsoft.com/azure/active-directory/device-management-introduction) e-giriş e bakın.</span><span class="sxs-lookup"><span data-stu-id="8c729-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="8c729-107">Adımlar da aşağıdaki bölümlerde özetlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="8c729-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="8c729-108">Azure AD Connect çalıştırın</span><span class="sxs-lookup"><span data-stu-id="8c729-108">Run Azure AD Connect</span></span>

<span data-ttu-id="8c729-109">Kuruluşunuzun Azure AD'sinin birleştirilmiş aygıtlarının şirket içi kaynaklara erişmesini sağlamak için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="8c729-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="8c729-110">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure AD Connect'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="8c729-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="8c729-111">Dizin eşitlemesi tamamlandıktan sonra, kuruluşunuzun Windows 10 aygıtlarının Azure AD'ye katıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="8c729-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="8c729-112">Bu adım her Windows 10 aygıtında ayrı ayrı yapılır.</span><span class="sxs-lookup"><span data-stu-id="8c729-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="8c729-113">Ayrıntılar [için Microsoft 365 Business kullanıcıları için Windows aygıtları ayarlama'ya](set-up-windows-devices.md) bakın.</span><span class="sxs-lookup"><span data-stu-id="8c729-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="8c729-114">Windows 10 aygıtları Azure AD'ye katıldıktan sonra, her kullanıcı cihazlarını yeniden başlatmalı ve Microsoft 365 Business kimlik bilgileriyle oturum açmalıdır.</span><span class="sxs-lookup"><span data-stu-id="8c729-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="8c729-115">Artık tüm aygıtlar şirket içi kaynaklara da erişeceksiniz.</span><span class="sxs-lookup"><span data-stu-id="8c729-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="8c729-116">Azure AD'ye katılan aygıtlar için şirket içi kaynaklara erişmek için ek adım gerekmez.</span><span class="sxs-lookup"><span data-stu-id="8c729-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="8c729-117">Bu, Windows 10'da bulunan yerleşik işlevselliktir.</span><span class="sxs-lookup"><span data-stu-id="8c729-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="8c729-118">Kuruluşunuz yukarıda açıklanan Azure AD Joined Aygıt Yapılandırmasında kullanıma hazır değilse, [Karma Azure AD Joined aygıt yapılandırmasını](manage-windows-devices.md)ayarlamayı düşünün.</span><span class="sxs-lookup"><span data-stu-id="8c729-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="8c729-119">Windows aygıtlarınızı Azure AD'ye katılırken dikkat edilmesi gerekenler</span><span class="sxs-lookup"><span data-stu-id="8c729-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="8c729-120">Azure AD'nin daha önce etki alanına veya bir çalışma grubunda bir araya getirilmiş bir Windows aygıtına katılması durumunda, aşağıdaki sınırlamaları göz önünde bulundurmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="8c729-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="8c729-121">Bir aygıt Azure AD katıldığında, varolan bir profile başvurmadan yeni bir kullanıcı oluşturur.</span><span class="sxs-lookup"><span data-stu-id="8c729-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="8c729-122">Bunu düzeltmek için profillerin el ile geçirilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="8c729-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="8c729-123">Kullanıcı profili sık kullanılanlar, yerel dosyalar, tarayıcı ayarları, Başlat menüsü ayarları gibi bilgiler içerir. En iyi yaklaşım, varolan dosyaları ve ayarları yeni profille eşlemek için bir üçüncü taraf aracı bulmaktır</span><span class="sxs-lookup"><span data-stu-id="8c729-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="8c729-124">Aygıt Grup İlkesi Nesneleri (GPO) kullanıyorsa, bazı GPO'larda Intune'da karşılaştırılabilir bir [Yapılandırma Hizmet Sağlayıcısı](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="8c729-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="8c729-125">Mevcut GPO'lar için karşılaştırılabilir CSP'ler bulmak için [MMAT aracını](https://www.microsoft.com/download/details.aspx?id=45520) çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="8c729-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="8c729-126">Kullanıcılar Active Directory kimlik doğrulamasına bağlı olan uygulamaların kimliğini doğrulayamayacaktır.</span><span class="sxs-lookup"><span data-stu-id="8c729-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="8c729-127">Bu işlemle başa çıkmak için eski bir uygulamayı kullanarak değerlendirin ve mümkünse modern Auth kullanan bir uygulamaya güncellemeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="8c729-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="8c729-128">Etkin Dizin yazıcı sı yatsı bulma çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="8c729-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="8c729-129">Bunu düzeltmek için, tüm kullanıcılar için doğrudan yazıcı yolları sağlayın veya [Karma Bulut Baskısından](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)yararlanın.</span><span class="sxs-lookup"><span data-stu-id="8c729-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
