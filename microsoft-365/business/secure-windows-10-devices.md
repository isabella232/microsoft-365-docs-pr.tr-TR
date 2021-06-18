---
title: Windows 10 cihazlarının güvenliğini sağlama
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: İş veya okul hesaplarında oturum Windows 10 ilgili cihaza varsayılan cihaz ilkesi ayarlarını yapılandırma hakkında bilgi edinebilirsiniz.
ms.openlocfilehash: 3f85549e722c9aa4196cf50fc02bee2e89506017
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925249"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="4e16d-103">Windows 10 cihazlarının güvenliğini sağlama</span><span class="sxs-lookup"><span data-stu-id="4e16d-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="4e16d-104">Bu makale diğer Microsoft 365 İş Ekstra.</span><span class="sxs-lookup"><span data-stu-id="4e16d-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="4e16d-105">Burada yapılandırdığınız ayarlar, Windows 10 için varsayılan cihaz ilkesinin bir parçasıdır.</span><span class="sxs-lookup"><span data-stu-id="4e16d-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="4e16d-106">Mobil cihazlar ve bilgisayarlar da Windows 10 bir cihaza bağlı olarak iş hesaplarıyla oturum alan tüm kullanıcılar bu ayarları otomatik olarak alır.</span><span class="sxs-lookup"><span data-stu-id="4e16d-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="4e16d-107">Kurulum sırasında varsayılan ilkeyi kabul etmenizi ve daha sonra belirli kullanıcı gruplarını hedef alan ilkeler eklemenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="4e16d-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="4e16d-108">Windows 10 cihazlarının güvenliğini sağlayan ayarlar</span><span class="sxs-lookup"><span data-stu-id="4e16d-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="4e16d-p102">Varsayılan olarak tüm ayarlar **Açık** durumdadır. Aşağıdaki ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="4e16d-p102">By default all settings are **On**. The following settings are available:</span></span>
  


|<span data-ttu-id="4e16d-111">Ayar</span><span class="sxs-lookup"><span data-stu-id="4e16d-111">Setting</span></span>  <br/> |<span data-ttu-id="4e16d-112">Açıklama</span><span class="sxs-lookup"><span data-stu-id="4e16d-112">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="4e16d-113">Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="4e16d-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="4e16d-114">Bilgisayarları internete bağlı olmanın getirdiği tehlikelerden korumak için Windows Defender Virüsten Koruma programının açık olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4e16d-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="4e16d-115">Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="4e16d-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="4e16d-116">Edge'de, kullanıcıları kötü amaçlı sitelerden ve indirmelerden korumaya yardımcı olan ayarları açar.</span><span class="sxs-lookup"><span data-stu-id="4e16d-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="4e16d-117">BitLocker ile PC'lerdeki dosyaların ve klasörlerin yetkisiz erişime karşı korunmasına yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="4e16d-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="4e16d-118">BitLocker bilgisayar sabit sürücülerini şifreleyerek verileri korur ve bilgisayar kaybolduğunda veya çalındığında verilerin açığa çıkma durumuna karşı koruma sağlar.</span><span class="sxs-lookup"><span data-stu-id="4e16d-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="4e16d-119">Daha fazla bilgi için [bitlocker SSS bölümüne bakın.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)</span><span class="sxs-lookup"><span data-stu-id="4e16d-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="4e16d-120">Cihaz şu kadar süre boşta kaldığında ekranı kapat</span><span class="sxs-lookup"><span data-stu-id="4e16d-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="4e16d-p104">Kullanıcı cihaz başında olmadığında şirket verilerinin korunmasını sağlar. Kullanıcı bir kafe gibi herkese açık bir konumda çalışıyorken kısa süreliğine uzaklaşabilir veya başka bir şeyle ilgilenebilir ve bu sırada diğer kişiler cihazdaki bilgilere bakabilir. Bu ayar sayesinde, ekran kapanmadan önce kullanıcının ne kadar süre boşta olabileceğini denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4e16d-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|