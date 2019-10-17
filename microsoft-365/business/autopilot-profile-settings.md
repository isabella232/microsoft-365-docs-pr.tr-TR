---
title: AutoPilot Profili ayarları hakkında
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
ms.openlocfilehash: eb0d9a95c796909d024db1d061aaeace7d07ed1b
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574588"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="5caa2-104">AutoPilot Profili ayarları hakkında</span><span class="sxs-lookup"><span data-stu-id="5caa2-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="5caa2-105">Otomatik Pilot profil ayarları</span><span class="sxs-lookup"><span data-stu-id="5caa2-105">AutoPilot profile settings</span></span>

<span data-ttu-id="5caa2-106">Otomatik Pilot profillerini kullanarak Windows'un kullanıcı aygıtlarına nasıl yüklenebileceğini denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5caa2-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="5caa2-107">Profiller aşağıdaki ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="5caa2-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="5caa2-108">**Otomatik Olarak ayarlanan Otomatik Pilot varsayılan özellikleri (gereklidir) :**</span><span class="sxs-lookup"><span data-stu-id="5caa2-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="5caa2-109">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="5caa2-109">**Setting**</span></span>|<span data-ttu-id="5caa2-110">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="5caa2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5caa2-111">Cortana, OneDrive ve OEM kaydını atla</span><span class="sxs-lookup"><span data-stu-id="5caa2-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="5caa2-112">Cortana ve kişisel OneDrive gibi tüketici uygulamalarının yüklenmesini atlar.</span><span class="sxs-lookup"><span data-stu-id="5caa2-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="5caa2-113">Aygıt kullanıcısı, aygıtta yerel bir yönetici olduğu sürece bunları daha sonra yükleyebilir.</span><span class="sxs-lookup"><span data-stu-id="5caa2-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="5caa2-114">Aygıt Microsoft 365 Business tarafından yönetilecektir, çünkü orijinal üretici kaydı atlanır.</span><span class="sxs-lookup"><span data-stu-id="5caa2-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="5caa2-115">Şirket markanızla deneyim de oturum açın</span><span class="sxs-lookup"><span data-stu-id="5caa2-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="5caa2-116">Şirketinizin Office [365 Oturum Aç sayfasına şirket markanızı ekle'ye](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)sahipse, cihaz kullanıcısı oturum açken bu deneyimi yaşar.</span><span class="sxs-lookup"><span data-stu-id="5caa2-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="5caa2-117">Yapılandırılmış AAD hesapları ile MDM otomatik kayıt.</span><span class="sxs-lookup"><span data-stu-id="5caa2-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="5caa2-118">Kullanıcı kimliği Azure Active dizini tarafından yönetilecek ve kullanıcılar Microsoft 365 Business kimlik bilgileriyle Windows ve Office 365'te oturum açacaktır.</span><span class="sxs-lookup"><span data-stu-id="5caa2-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="5caa2-119">**İsteğe bağlı ayarlar:**</span><span class="sxs-lookup"><span data-stu-id="5caa2-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="5caa2-120">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="5caa2-120">**Setting**</span></span>|<span data-ttu-id="5caa2-121">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="5caa2-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5caa2-122">Gizlilik ayarlarını atla (Varsayılan olarak kapalı)</span><span class="sxs-lookup"><span data-stu-id="5caa2-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="5caa2-123">Bu seçenek **Açık**olarak ayarlanmışsa, aygıt kullanıcısı ilk giriş yaptığında aygıt ve Windows için lisans sözleşmesini görmez.</span><span class="sxs-lookup"><span data-stu-id="5caa2-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="5caa2-124">Kullanıcının yerel yönetici olmasına izin verme</span><span class="sxs-lookup"><span data-stu-id="5caa2-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="5caa2-125">Bu seçenek A.B.D. olarak ayarlanmışsa, aygıt kullanıcısı Cortana gibi herhangi bir kişisel uygulama yükleyemez. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="5caa2-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
