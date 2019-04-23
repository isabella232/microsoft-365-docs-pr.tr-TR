---
title: Windows 10 cihazlarında Office'i otomatik olarak yükleme veya kaldırma
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: "Yüklemek veya Windows 10 aygıtlarda Microsoft 365 iş Yönetim Merkezi'nden Office yüklemesini kaldırın. "
ms.openlocfilehash: fef4a543aed489202bf05dfb1e8cafbb784ca819
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277316"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="5c78e-103">Windows 10 cihazlarında Office'i otomatik olarak yükleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="5c78e-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="5c78e-104">Microsoft 365 İş yönetim merkezinden, Windows 10 bilgisayarlarına Office'i hızla ve kolayca yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5c78e-104">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="5c78e-105">Daha önce yüklenmiş Office uygulamaları olduğunda bu işlemin nasıl çalıştığını anlamak için, başlamadan önce [Office istemci yüklemesi hazırlığı](prepare-for-office-client-deployment.md) konusunu okuyun.</span><span class="sxs-lookup"><span data-stu-id="5c78e-105">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="5c78e-106">Office dağıtımlarını yönetme</span><span class="sxs-lookup"><span data-stu-id="5c78e-106">Manage Office deployments</span></span>

1. <span data-ttu-id="5c78e-107">Genel yönetici kimlik bilgileriyle [yönetim merkezinde](https://aka.ms/bcsportal) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="5c78e-107">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="5c78e-108">**Cihazlar** kartında **Office Dağıtımını Yönet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5c78e-108">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="5c78e-109">**Aygıt Eylemler** kartı görmüyorsanız Yönetim Merkezi **Giriş** sayfasında admin evinizin eklemek için **Ekle** (+) tıklatın.</span><span class="sxs-lookup"><span data-stu-id="5c78e-109">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="5c78e-111">Açılan **Office dağıtımını yönet** bölmesinde **Grup ekle**'yi ve sonra da kullanmak istediğiniz grupları seçin.</span><span class="sxs-lookup"><span data-stu-id="5c78e-111">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="5c78e-112">Kullanmak istediğiniz bir veya birden çok grubu ekledikten sonra, **Dağıtım Eylemi** açılan listesinden **En kısa zamanda Office'i yükle**'yi veya **Office'i kaldır**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="5c78e-112">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="5c78e-114">Choose **Next** \> review the settings and then choose **Confirm**.</span><span class="sxs-lookup"><span data-stu-id="5c78e-114">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="5c78e-115">Kullandığınız grup veya gruplarla belirtilen kullanıcıların sahip olduğu cihazlarda 32 bit bir Office otomatik olarak yüklenir veya kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="5c78e-115">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="5c78e-116">Office yüklemesi için seçilmiş olan bilgisayarda Görev Yöneticisi'ni açabildiğinizi doğrulayın ve Microsoft Office Tıkla-Çalıştır işlemini bulun.</span><span class="sxs-lookup"><span data-stu-id="5c78e-116">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


