---
title: Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Microsoft 365'in yerel AD'yi korumak için Windows 10 aygıtlarını nasıl koruyacağınızı öğrenin.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992239"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="4697a-103">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="4697a-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="4697a-104">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4697a-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="4697a-105">Bunu, önce Active Directory ile senkronize ederek, ardından Windows 10 aygıtlarını Azure AD'ye kaydederek ve Microsoft 365 Business tarafından mobil cihaz yönetimine kaydederek ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4697a-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="4697a-106">Aşağıdaki video, bunu en yaygın senaryo için nasıl ayarlayabilmek için gereken adımları ayrıntılarıyla açıklar.</span><span class="sxs-lookup"><span data-stu-id="4697a-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="4697a-107">Microsoft 365 Business tarafından yönetilecek etki alanı birleştirilmiş aygıtları ayarlama</span><span class="sxs-lookup"><span data-stu-id="4697a-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="4697a-108">Kurum içi Active Directory'ye ek olarak Azure Active Directory tarafından sağlanan özelliklerden yararlanacak şekilde kuruluşunuzun etki alanına katılan aygıtlarını ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4697a-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="4697a-109">Bunlar, hem şirket içi Active Dizininize hem de Azure Etkin Dizininize katılan aygıtlardır.</span><span class="sxs-lookup"><span data-stu-id="4697a-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="4697a-110">Karma Azure AD birleştirilmiş aygıtlar Microsoft 365 Business tarafından korunabilir ve yönetilebilir.</span><span class="sxs-lookup"><span data-stu-id="4697a-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="4697a-111">Windows 10 cihazlarınızı Karma Azure AD'nin Microsoft 365 Business tarafından birleştirilmiş ve yönetildiği yapmak için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="4697a-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="4697a-112">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek [için, Office 365 için dizin eşitlemesi ayarlayın'da](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi Dizin eşitleme sihirbazını ve Azure Etkin Dizin Bağlantısı'nı çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="4697a-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="4697a-113">Adımlar Microsoft 365 Business için tam olarak aynıdır.</span><span class="sxs-lookup"><span data-stu-id="4697a-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="4697a-114">Windows 10 aygıtların Karma Azure AD'ye katılmasını sağlamak için 3.</span><span class="sxs-lookup"><span data-stu-id="4697a-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="4697a-115">Azure AD bağlantısının en son sürümünü çalıştırıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="4697a-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="4697a-116">Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti.</span><span class="sxs-lookup"><span data-stu-id="4697a-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="4697a-117">Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.</span><span class="sxs-lookup"><span data-stu-id="4697a-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="4697a-118">Karma Azure AD Joined olmak üzere varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydedin ve Bunları Intune (Microsoft 365 Business) tarafından mobil cihaz yönetimine kaydedin:</span><span class="sxs-lookup"><span data-stu-id="4697a-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="4697a-119">[Karma Azure Active Directory'yi birleştirme aygıtlarını yapılandırma](https://go.microsoft.com/fwlink/p/?linkid=872870)konusunda adım adım yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="4697a-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="4697a-120">Bu, şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını sağlar ve bulutları hazır hale getirecektir.</span><span class="sxs-lookup"><span data-stu-id="4697a-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="4697a-121">Mobil aygıt yönetimi için bir Windows 10 aygıtı kaydetmek için, talimatlar için [Bir Grup İlkesi kullanarak Bir Windows 10 aygıtını Intune'a](https://go.microsoft.com/fwlink/p/?linkid=872871) kaydedin' e bakın.</span><span class="sxs-lookup"><span data-stu-id="4697a-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="4697a-122">Grup İlkesi'ni yerel bir bilgisayar düzeyinde veya toplu işlemler için ayarlayabilirsiniz, etki alanı denetleyici sunucunuzda bu grup ilkesi ayarını oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4697a-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>