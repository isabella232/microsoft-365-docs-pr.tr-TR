---
title: Kullanıcılarının Windows 10 cihazlarına Office yüklemesini yardımcı olun
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: Kullanıcılarının Windows 10 cihazlarına Office uygulamalarını yüklemelerini ve Office'i Microsoft 365 yönetim merkezinden Windows 10 pc'lere kolayca yüklemelerini sağlar.
ms.openlocfilehash: 5337c8ef008c1af79490eb6b6705d450055d24fb
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913356"
---
# <a name="help-your-users-install-office-on-windows-10-devices"></a><span data-ttu-id="f7104-103">Kullanıcılarının Windows 10 cihazlarına Office yüklemesini yardımcı olun</span><span class="sxs-lookup"><span data-stu-id="f7104-103">Help your users install Office on Windows 10 devices</span></span>

<span data-ttu-id="f7104-104">[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="f7104-104">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="f7104-105">Microsoft 365 yönetim merkezinden Windows 10 bilgisayarlara Office'i hızla ve kolayca yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7104-105">You can quickly and easily install Office on Windows 10 PCs from the Microsoft 365 admin center.</span></span>
  
<span data-ttu-id="f7104-106">Daha önce yüklenmiş Office uygulamaları olduğunda bu işlemin nasıl çalıştığını anlamak için, başlamadan önce [Office istemci yüklemesi hazırlığı](prepare-for-office-client-deployment.md) konusunu okuyun.</span><span class="sxs-lookup"><span data-stu-id="f7104-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span>

<span data-ttu-id="f7104-107">Office uygulamalarını yükleme hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="f7104-107">Watch a short video about installing Office apps.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/acce002c-0756-4b64-ac5d-2198ee96a9b1] 

<span data-ttu-id="f7104-108">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="f7104-108">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="manage-office-deployments"></a><span data-ttu-id="f7104-109">Office dağıtımlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="f7104-109">Manage Office deployments</span></span>

1. <span data-ttu-id="f7104-110">Yönetim merkezine gidin ve <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> genel yönetici kimlik bilgileriyle oturum açma.</span><span class="sxs-lookup"><span data-stu-id="f7104-110">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>, and sign in with global admin credentials.</span></span> 

2. <span data-ttu-id="f7104-111">Sol gezinti **bölmesinde** Kurulum'a gidin ve Kurulum sayfasında Uygulamalar **ve** güncelleştirmeler'e **ilerleyin.**</span><span class="sxs-lookup"><span data-stu-id="f7104-111">Go to **Setup** in the left navigation pane, and on the **Setup** page, scroll to **Apps and updates**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f7104-112">Tüm kullanıcılarınız Office uygulamalarını yüklemişse bu kartı görmeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f7104-112">You might not see this card if all of your  users have installed Office apps.</span></span>
  
3. <span data-ttu-id="f7104-113">Yardım **kullanıcılarının Office uygulamaları kartını yüklemelerine yardımcı** olun, Görünüm'e **ve** sonra da **Başla'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="f7104-113">On the **Help users install their Office apps** card, choose **View**, and then **Get started**.</span></span>
    
4. <span data-ttu-id="f7104-114">**E-posta kullanıcılarına Office panelini indirme** bağlantısında, e-postayla göndermek istediğiniz kullanıcıları seçin ve ardından E-postayla **seçilen kullanıcılara e-posta gönderin.**</span><span class="sxs-lookup"><span data-stu-id="f7104-114">On the **Email users a link to download Office** panel, select the users you want to email, and then **Email selected users**.</span></span>

   ![Office indirme bağlantısıyla e-posta göndermek için kullanıcıları seçin.](../media/sendemailtousers.png)

## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="f7104-116">Microsoft 365 İş Ekstra'ı ayarlama ve kullanma hakkında daha fazla bilgi için</span><span class="sxs-lookup"><span data-stu-id="f7104-116">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="f7104-117">İş için Microsoft 365 eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="f7104-117">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)