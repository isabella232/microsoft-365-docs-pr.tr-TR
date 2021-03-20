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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profilleri, Windows'un kullanıcı cihazlarına nasıl yük olduğunu denetlemeye yardımcı olur. Profiller, Cortana yüklemesini atlama gibi varsayılan ve isteğe bağlı ayarlar içerir.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913388"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="a707d-104">AutoPilot Profili ayarları hakkında</span><span class="sxs-lookup"><span data-stu-id="a707d-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="a707d-105">AutoPilot profil ayarları</span><span class="sxs-lookup"><span data-stu-id="a707d-105">AutoPilot profile settings</span></span>

<span data-ttu-id="a707d-106">Kullanıcı cihazlarına Windows'un nasıl yük olduğunu kontrol etmek için AutoPilot profillerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a707d-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="a707d-107">Profiller aşağıdaki ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="a707d-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="a707d-108">**Otomatik olarak ayarlanmış AutoPilot varsayılan özellikleri (gerekli):**</span><span class="sxs-lookup"><span data-stu-id="a707d-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="a707d-109">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="a707d-109">**Setting**</span></span>|<span data-ttu-id="a707d-110">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="a707d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a707d-111">Cortana, OneDrive ve OEM kaydını atlama</span><span class="sxs-lookup"><span data-stu-id="a707d-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="a707d-112">Cortana ve kişisel OneDrive gibi tüketici uygulamalarının yüklemesini atlar.</span><span class="sxs-lookup"><span data-stu-id="a707d-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="a707d-113">Kullanıcı cihazda yerel yönetici olduğu sürece cihaz kullanıcısı bunları daha sonra yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="a707d-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="a707d-114">Cihaz Microsoft 365 İş Ekstra tarafından yönetilecek olduğundan orijinal üretici kaydı atlanır.</span><span class="sxs-lookup"><span data-stu-id="a707d-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="a707d-115">Şirket markanız ile oturum açma deneyimi</span><span class="sxs-lookup"><span data-stu-id="a707d-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="a707d-116">Şirketinizin Microsoft [365](../admin/setup/customize-sign-in-page.md)Oturum Açma sayfasına şirket markası eklemesi varsa, cihaz kullanıcısı oturum aken bu deneyimi edinecektir.</span><span class="sxs-lookup"><span data-stu-id="a707d-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="a707d-117">Yapılandırılmış AAD hesaplarıyla MDM otomatik kaydı.</span><span class="sxs-lookup"><span data-stu-id="a707d-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="a707d-118">Kullanıcı kimliği Azure Active Directory tarafından yönetiliyor ve kullanıcılar Windows ve Microsoft 365'te Microsoft 365 İş Ekstra kimlik bilgileriyle oturum aecek.</span><span class="sxs-lookup"><span data-stu-id="a707d-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="a707d-119">**İsteğe bağlı ayarlar:**</span><span class="sxs-lookup"><span data-stu-id="a707d-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="a707d-120">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="a707d-120">**Setting**</span></span>|<span data-ttu-id="a707d-121">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="a707d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a707d-122">Gizlilik ayarlarını atla (Varsayılan olarak kapalı)</span><span class="sxs-lookup"><span data-stu-id="a707d-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="a707d-123">Bu seçenek Açık olarak **ayarlanırsa,** cihaz kullanıcısı ilk kez oturum anlaşmayı kabul etmek için cihaz ve Windows lisans sözleşmesini görmez.</span><span class="sxs-lookup"><span data-stu-id="a707d-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="a707d-124">Kullanıcının yerel yönetici olmasına izin verme</span><span class="sxs-lookup"><span data-stu-id="a707d-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="a707d-125">Bu seçenek Açık olarak **ayarlanırsa,** cihaz kullanıcısı Cortana gibi hiçbir kişisel uygulama yükleyemz.</span><span class="sxs-lookup"><span data-stu-id="a707d-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
