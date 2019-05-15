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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profilleri Windows kullanıcı aygıtlarda ne yüklendiði denetlemenize yardımcı olur. Varsayılan profilleri içerir ve isteğe bağlı ayarlar Cortana yükleme atlamak istiyor.
ms.openlocfilehash: adc8112861b67fd96a91ff24dc155aeb0c394532
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071870"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="40ae5-104">AutoPilot Profili ayarları hakkında</span><span class="sxs-lookup"><span data-stu-id="40ae5-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="40ae5-105">AutoPilot profil ayarları</span><span class="sxs-lookup"><span data-stu-id="40ae5-105">AutoPilot profile settings</span></span>

<span data-ttu-id="40ae5-106">Windows kullanıcı aygıtlarda AutoPilot profilleri kullanarak nasıl yüklendiði kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="40ae5-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="40ae5-107">Profilleri aşağıdaki ayarları içerir.</span><span class="sxs-lookup"><span data-stu-id="40ae5-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="40ae5-108">**Otomatik olarak ayarlanır (gerekli) autoPilot varsayılan özellikleri:**</span><span class="sxs-lookup"><span data-stu-id="40ae5-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="40ae5-109">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="40ae5-109">**Setting**</span></span>|<span data-ttu-id="40ae5-110">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="40ae5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40ae5-111">Atla Cortana, OneDrive ve OEM kayıt</span><span class="sxs-lookup"><span data-stu-id="40ae5-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="40ae5-112">Tüketici uygulamaları Cortana ve kişisel OneDrive gibi yüklenmesi atlanıyor.</span><span class="sxs-lookup"><span data-stu-id="40ae5-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="40ae5-113">Aygıt üzerinde yerel bir yönetici izinli olduğu sürece aygıt kullanıcı bu daha sonra yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="40ae5-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="40ae5-114">Özgün üretici kayıt aygıtı Microsoft 365 işletme tarafından yönetilecek olduğundan atlandı.</span><span class="sxs-lookup"><span data-stu-id="40ae5-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="40ae5-115">Şirket markanızı deneyimiyle imi</span><span class="sxs-lookup"><span data-stu-id="40ae5-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="40ae5-116">Bir [Office 365 oturum sayfası için Ekle, şirketinizin markasını](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)şirketiniz varsa, aygıt kullanıcı oturumu açarken bu deneyimi elde edemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="40ae5-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="40ae5-117">MDM otomatik kayıt yapılandırılmış AAD hesapları ile.</span><span class="sxs-lookup"><span data-stu-id="40ae5-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="40ae5-118">Kullanıcı Kimliği Azure Active directory tarafından yönetilecek ve kullanıcıların Microsoft 365 iş kimlik bilgilerini Windows ve Office 365 imzalayacak.</span><span class="sxs-lookup"><span data-stu-id="40ae5-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="40ae5-119">**İsteğe bağlı ayarlar:**</span><span class="sxs-lookup"><span data-stu-id="40ae5-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="40ae5-120">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="40ae5-120">**Setting**</span></span>|<span data-ttu-id="40ae5-121">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="40ae5-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40ae5-122">Gizlilik ayarlarını Atla (varsayılan olarak kapalı)</span><span class="sxs-lookup"><span data-stu-id="40ae5-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="40ae5-123">**Üzerinde**bu seçeneği ayarlarsanız, isterse ilk açtığında aygıt kullanıcı aygıt ve Windows için Lisans Sözleşmesi'ni göremez.</span><span class="sxs-lookup"><span data-stu-id="40ae5-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="40ae5-124">Yerel yönetici olacak bir kullanıcı izin verme</span><span class="sxs-lookup"><span data-stu-id="40ae5-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="40ae5-125">**Üzerinde**bu seçeneği ayarlarsanız, aygıt kullanıcı Cortana gibi tüm kişisel uygulamalar yükleme olanağınız olur.</span><span class="sxs-lookup"><span data-stu-id="40ae5-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
