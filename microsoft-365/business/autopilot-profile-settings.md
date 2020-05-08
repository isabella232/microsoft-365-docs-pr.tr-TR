---
title: AutoPilot Profili ayarları hakkında
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
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
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Otomatik Pilot profilleri, Windows'un kullanıcı aygıtlarına nasıl yükleniyi denetlemenize yardımcı olur. Profiller Cortana yüklemesini atla gibi varsayılan ve isteğe bağlı ayarlar içerir.
ms.openlocfilehash: 0c706d12ba262856ff40ea3bee57c64234fd77f7
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165851"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="ea2f8-104">AutoPilot Profili ayarları hakkında</span><span class="sxs-lookup"><span data-stu-id="ea2f8-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="ea2f8-105">Otomatik Pilot profil ayarları</span><span class="sxs-lookup"><span data-stu-id="ea2f8-105">AutoPilot profile settings</span></span>

<span data-ttu-id="ea2f8-106">Windows'un kullanıcı aygıtlarına nasıl yüklenirdenetlemek için Otomatik Pilot profillerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="ea2f8-107">Profiller aşağıdaki ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="ea2f8-108">**Otomatik Olarak ayarlanan Otomatik Pilot varsayılan özellikleri (gereklidir) :**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="ea2f8-109">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-109">**Setting**</span></span>|<span data-ttu-id="ea2f8-110">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea2f8-111">Cortana, OneDrive ve OEM kaydını atla</span><span class="sxs-lookup"><span data-stu-id="ea2f8-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="ea2f8-112">Cortana ve kişisel OneDrive gibi tüketici uygulamalarının yüklenmesini atlar.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="ea2f8-113">Aygıt kullanıcısı, aygıtta yerel bir yönetici olduğu sürece bunları daha sonra yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="ea2f8-114">Aygıt Microsoft 365 Business Premium tarafından yönetilecektir, çünkü orijinal üretici kaydı atlanır.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="ea2f8-115">Şirket markanızla deneyim de oturum açın</span><span class="sxs-lookup"><span data-stu-id="ea2f8-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="ea2f8-116">Şirketinizin Microsoft [365 Oturum Açma sayfasına şirket markanızı ekle'ye](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page)sahipse, aygıt kullanıcısı oturum açken bu deneyimi yaşar.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="ea2f8-117">Yapılandırılmış AAD hesapları ile MDM otomatik kayıt.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="ea2f8-118">Kullanıcı kimliği Azure Active Directory tarafından yönetilecek ve kullanıcılar Microsoft 365 Business Premium kimlik bilgileriyle Windows ve Microsoft 365'te oturum açacaktır.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="ea2f8-119">**İsteğe bağlı ayarlar:**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="ea2f8-120">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-120">**Setting**</span></span>|<span data-ttu-id="ea2f8-121">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea2f8-122">Gizlilik ayarlarını atla (Varsayılan olarak kapalı)</span><span class="sxs-lookup"><span data-stu-id="ea2f8-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="ea2f8-123">Bu seçenek **Açık**olarak ayarlanmışsa, aygıt kullanıcısı ilk giriş yaptığında aygıt ve Windows için lisans sözleşmesini görmez.</span><span class="sxs-lookup"><span data-stu-id="ea2f8-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="ea2f8-124">Kullanıcının yerel yönetici olmasına izin verme</span><span class="sxs-lookup"><span data-stu-id="ea2f8-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="ea2f8-125">Bu seçenek A.B.D. olarak ayarlanmışsa, aygıt kullanıcısı Cortana gibi herhangi bir kişisel uygulama yükleyemez. **On**</span><span class="sxs-lookup"><span data-stu-id="ea2f8-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
