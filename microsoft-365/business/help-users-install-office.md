---
title: Kullanıcılarınızın Windows 10 cihazlarında Office 'i yüklemesine yardımcı olma
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
description: Kullanıcılarınızın Windows 10 cihazlarında Office uygulamalarını yüklemesine ve Microsoft 365 Yönetim Merkezi 'nden Windows 10 PC 'Lere kolayca Office yüklemesine yardımcı olun.
ms.openlocfilehash: 680c1c4e43a037c6afd109220090f387b207f8b1
ms.sourcegitcommit: d39694d7b2c98350b0d568dfd03fa0ef44ed4c1d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/10/2020
ms.locfileid: "46601993"
---
# <a name="help-your-users-install-office-on-windows-10-devices"></a><span data-ttu-id="df66b-103">Kullanıcılarınızın Windows 10 cihazlarında Office 'i yüklemesine yardımcı olma</span><span class="sxs-lookup"><span data-stu-id="df66b-103">Help your users install Office on Windows 10 devices</span></span>

<span data-ttu-id="df66b-104">[![Yönetim merkezinin değiştiğini size bildirmeye yarayan etiket ve daha fazla ayrıntıyı aka.ms/aboutM365preview sayfasında bulabilirsiniz.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="df66b-104">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="df66b-105">Microsoft 365 Yönetim Merkezi 'nden Windows 10 PC 'ye hızla ve kolayca Office yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="df66b-105">You can quickly and easily install Office on Windows 10 PCs from the Microsoft 365 admin center.</span></span>
  
<span data-ttu-id="df66b-106">Daha önce yüklenmiş Office uygulamaları olduğunda bu işlemin nasıl çalıştığını anlamak için, başlamadan önce [Office istemci yüklemesi hazırlığı](prepare-for-office-client-deployment.md) konusunu okuyun.</span><span class="sxs-lookup"><span data-stu-id="df66b-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span>

<span data-ttu-id="df66b-107">Office uygulamalarını yükleme hakkında kısa bir video izleyin.</span><span class="sxs-lookup"><span data-stu-id="df66b-107">Watch a short video about installing Office apps.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/acce002c-0756-4b64-ac5d-2198ee96a9b1] 

<span data-ttu-id="df66b-108">Bu videoyu faydalı bulduysanız, [küçük işletmelere ve Microsoft 365’i ilk kez kullananlara yönelik eğitim serisinin tamamına göz atın](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="df66b-108">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="manage-office-deployments"></a><span data-ttu-id="df66b-109">Office dağıtımlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="df66b-109">Manage Office deployments</span></span>

1. <span data-ttu-id="df66b-110">Yönetim Merkezi 'ne gidin <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ve genel yönetici kimlik bilgileriyle oturum açın.</span><span class="sxs-lookup"><span data-stu-id="df66b-110">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>, and sign in with global admin credentials.</span></span> 

2. <span data-ttu-id="df66b-111">Sol gezinti bölmesinde **Kurulum** 'a gidin ve **Kurulum** sayfasında **uygulamalar ve güncelleştirmeler**'e gidin.</span><span class="sxs-lookup"><span data-stu-id="df66b-111">Go to **Setup** in the left navigation pane, and on the **Setup** page, scroll to **Apps and updates**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="df66b-112">Tüm kullanıcılarınızın Office uygulamalarını yüklediği bu kartı göremeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="df66b-112">You might not see this card if all of your  users have installed Office apps.</span></span>
  
3. <span data-ttu-id="df66b-113">**Kullanıcıların Office uygulamalarını yüklemelerinde** , **Görünüm**'ü ve sonra **Başlangıç**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="df66b-113">On the **Help users install their Office apps** card, choose **View**, and then **Get started**.</span></span>
    
4. <span data-ttu-id="df66b-114">**E-posta kullanıcıları Office 'i indirme bağlantısı** için, e-posta almak istediğiniz kullanıcıları seçin ve ardından **Seçili kullanıcılara e-posta gönderin**.</span><span class="sxs-lookup"><span data-stu-id="df66b-114">On the **Email users a link to download Office** panel, select the users you want to email, and then **Email selected users**.</span></span>

   ![Office indirme bağlantısı ile e-posta göndermek için kullanıcıları seçin.](../media/sendemailtousers.png)

## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="df66b-116">Microsoft 365 Business Premium 'u ayarlama ve kullanma konusunda daha fazla bilgi için</span><span class="sxs-lookup"><span data-stu-id="df66b-116">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="df66b-117">Microsoft 365 iş eğitim videoları</span><span class="sxs-lookup"><span data-stu-id="df66b-117">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
