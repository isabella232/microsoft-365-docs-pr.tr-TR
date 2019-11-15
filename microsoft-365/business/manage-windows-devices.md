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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Yerel Active Directory'yi korumak için Microsoft 365'i nasıl etkinleştirmek için Windows 10 aygıtlarına katıldığını öğrenin.
ms.openlocfilehash: 93e3364fc94f3878bec13d0a87b17a7d3678a4cc
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633279"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="f40c6-103">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="f40c6-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="f40c6-104">Kuruluşunuz Windows Server Active Directory'yi şirket içinde kullanıyorsa, Windows 10 aygıtlarınızı korumak için Microsoft 365 Business'ı ayarlayabilir ve yerel kimlik doğrulaması gerektiren şirket içi kaynaklara erişimi sürdürebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="f40c6-105">Bu korumayı ayarlamak için **Karma Azure AD birleştirilmiş aygıtları**uygulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="f40c6-106">Bu aygıtlar hem şirket içi Etkin Dizininizde hem de Azure Etkin Dizininizde birleştirilir.</span><span class="sxs-lookup"><span data-stu-id="f40c6-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="f40c6-107">Bu videoda, bunu en yaygın senaryo için nasıl ayarlayacaÄ ına yönelik adımlar açıklanmaktadır ve bu da izleyen adımlarda ayrıntılı olarak açıklanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="f40c6-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="f40c6-108">1. Dizin Senkronizasyonuna Hazırla</span><span class="sxs-lookup"><span data-stu-id="f40c6-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="f40c6-109">Kullanıcılarınızı ve bilgisayarlarınızı yerel Active Directory Etki Alanından eşitlemeden önce, [Office 365'e dizin eşitlemesi için hazırlayın'ı](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="f40c6-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="f40c6-110">Özellikle:</span><span class="sxs-lookup"><span data-stu-id="f40c6-110">In particular:</span></span>

   - <span data-ttu-id="f40c6-111">Aşağıdaki öznitelikler için dizininizde yineleme olmadığından emin olun: **posta,** **proxyAdresler**ve **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="f40c6-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="f40c6-112">Bu değerler benzersiz olmalı ve yinelenenler kaldırılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f40c6-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="f40c6-113">Her yerel kullanıcı hesabı için **userPrincipalName** (UPN) özniteliğini, lisanslı Microsoft 365 kullanıcısına karşılık gelen birincil e-posta adresiyle eşleşecek şekilde yapılandırmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="f40c6-114">Örneğin: *mary@contoso.yerel* yerine *mary.shelley@contoso.com*</span><span class="sxs-lookup"><span data-stu-id="f40c6-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="f40c6-115">Active Directory etki alanı *.com* veya *.org*gibi bir internet routable sonek yerine *.local* veya *.lan*gibi bir routable olmayan sonek biterse, önce yerel kullanıcı hesaplarının UPN sonekini [dizin eşitleme için routable olmayan bir etki alanı hazırlayın'da](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)açıklandığı gibi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="f40c6-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="f40c6-116">2. Azure AD Connect'i yükleme ve yapılandırma</span><span class="sxs-lookup"><span data-stu-id="f40c6-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="f40c6-117">Kullanıcılarınızı, gruplarınızı ve kişilerinizi yerel Active Directory'den Azure Etkin Dizini'ne senkronize etmek için Azure Active Directory Connect'i yükleyin ve dizin eşitlemesi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="f40c6-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="f40c6-118">Bkz. Daha fazla bilgi edinmek [için Office 365 için dizin eşitlemesi ayarla.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)</span><span class="sxs-lookup"><span data-stu-id="f40c6-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="f40c6-119">Adımlar Microsoft 365 Business için tam olarak aynıdır.</span><span class="sxs-lookup"><span data-stu-id="f40c6-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="f40c6-120">Azure AD Connect seçeneklerinizi yapılandırırken, Parola **Eşitleme**, **Sorunsuz Tek Oturum**Açma ve Microsoft 365 Business'ta da desteklenen **parola yazma** özelliğini etkinleştirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="f40c6-121">Azure AD Connect'teki onay kutusunun ötesinde parola yazma için bazı ek adımlar vardır.</span><span class="sxs-lookup"><span data-stu-id="f40c6-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="f40c6-122">Daha fazla bilgi için [bkz: Nasıl Yapılır: parola yazmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="f40c6-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="f40c6-123">3. Karma Azure REKLAM Birleştirme'yi Yapılandırma</span><span class="sxs-lookup"><span data-stu-id="f40c6-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="f40c6-124">Windows 10 aygıtların Karma Azure AD'ye katılmasını etkinleştirmeden önce aşağıdaki ön koşulları yerine getirebildiğinizden emin olun:</span><span class="sxs-lookup"><span data-stu-id="f40c6-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="f40c6-125">Azure AD Connect'in en son sürümünü çalıştırıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="f40c6-126">Azure AD bağlantısı, karma Azure AD olmak istediğiniz aygıtların tüm bilgisayar nesnelerini senkronize etti.</span><span class="sxs-lookup"><span data-stu-id="f40c6-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="f40c6-127">Bilgisayar nesneleri belirli kuruluş birimlerine (OU) aitse, bu OU'ların Azure AD bağlantısında eşitleme için ayarlandıklarından emin olun.</span><span class="sxs-lookup"><span data-stu-id="f40c6-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="f40c6-128">Karma Azure AD'nin katıldığı varolan etki alanı birleştirilmiş Windows 10 aygıtlarını kaydetmek [için, Öğreticideki adımları izleyin: Yönetilen etki alanları için karma Azure Active Directory join'i yapılandırın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="f40c6-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="f40c6-129">Bu karma, mevcut şirket içi Active Directory'nizin Windows 10 bilgisayarlarına katılmasını ve bulutu hazır hale getirmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="f40c6-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="f40c6-130">4. Windows 10 için otomatik kaydı etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="f40c6-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="f40c6-131">Mobil aygıt yönetimi için Windows 10 aygıtlarını Intune'a otomatik olarak kaydetmek için Grup [İlkesi'ni kullanarak bir Windows 10 aygıtını otomatik olarak kaydedin'e](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)bakın.</span><span class="sxs-lookup"><span data-stu-id="f40c6-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="f40c6-132">Grup İlkesi'ni yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için Etki Alanı Denetleyicinizde bu Grup İlkesi ayarını oluşturmak için Grup İlkesi Yönetim Konsolu ve ADMX şablonlarını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="f40c6-133">5. Yapılandırılan Sorunsuz Tek İşaret-On</span><span class="sxs-lookup"><span data-stu-id="f40c6-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="f40c6-134">Sorunsuz SSO, kullanıcıları kurumsal bilgisayarları kullanırken Microsoft 365 bulut kaynaklarına otomatik olarak imzalar.</span><span class="sxs-lookup"><span data-stu-id="f40c6-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="f40c6-135">[Azure Active Directory Seamless Tek Oturum Açma: Hızlı başlangıç'ta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)açıklanan iki Grup İlkesi seçeneğinden birini dağıtmanız yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="f40c6-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="f40c6-136">**Grup İlkesi** seçeneği kullanıcıların ayarlarını değiştirmesine izin vermezken, **Grup İlkesi Tercihi** seçeneği değerleri ayarlar, aynı zamanda kullanıcı tarafından yapılandırılabilir bırakır.</span><span class="sxs-lookup"><span data-stu-id="f40c6-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="f40c6-137">6. İşletmeler için Windows Hello'yu ayarlama</span><span class="sxs-lookup"><span data-stu-id="f40c6-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="f40c6-138">Windows Hello for Business, yerel bir bilgisayarda oturum açmak için parolaları güçlü iki faktörlü kimlik doğrulama (2FA) ile değiştirir.</span><span class="sxs-lookup"><span data-stu-id="f40c6-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="f40c6-139">Bir faktör asimetrik anahtar çifti, diğeri ise aygıtınız destekliyorsa parmak izi veya yüz tanıma gibi bir PIN veya diğer yerel harekettir.</span><span class="sxs-lookup"><span data-stu-id="f40c6-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="f40c6-140">Parolaları mümkün olduğunca 2FA ve Windows Hello for Business ile değiştirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="f40c6-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="f40c6-141">İşletmeler için Karma Windows Merhaba'yı yapılandırmak [için, İş Önkoşulları için Karma Anahtar güven Windows Hello'yu gözden geçirin.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs)</span><span class="sxs-lookup"><span data-stu-id="f40c6-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="f40c6-142">Ardından, İş [için Karma Windows Merhaba'yı Yapılandır'daki](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)yönergeleri izleyin anahtar güven ayarları.</span><span class="sxs-lookup"><span data-stu-id="f40c6-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
