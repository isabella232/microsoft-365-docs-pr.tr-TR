---
title: Microsoft 365 İş Standardı'ndan Microsoft 365 Business Premium'a yükseltme
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Microsoft 365 Business Standard ile Microsoft 365 Business Premium arasındaki farkı ve Microsoft 365 Business Premium'a nasıl yükseltebileceğinizi öğrenin.
ms.openlocfilehash: bdab8165623170926b17efa4cae9408b78a2f5f5
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401392"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a><span data-ttu-id="b05e7-103">Microsoft 365 İş Standardı'ndan Microsoft 365 Business Premium'a yükseltme</span><span class="sxs-lookup"><span data-stu-id="b05e7-103">Upgrade to Microsoft 365 Business Premium from Microsoft 365 Business Standard</span></span>

<span data-ttu-id="b05e7-104">İş aboneliği [için Microsoft 365'iniz](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)(örneğin, Microsoft 365 İş Standardı) varsa, Microsoft 365 Business Premium'a kolayca yükseltebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-104">If you have a [Microsoft 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Microsoft 365 Business Standard, you can easily upgrade to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="b05e7-105">Eklemek isterseniz Microsoft 365 Business Premium'a yükseltin:</span><span class="sxs-lookup"><span data-stu-id="b05e7-105">Upgrade to Microsoft 365 Business Premium if you want to add:</span></span>

- <span data-ttu-id="b05e7-106">Windows 10 Pro (Windows 8 veya sonraki çalıştıran bilgisayarlarına)</span><span class="sxs-lookup"><span data-stu-id="b05e7-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>

- <span data-ttu-id="b05e7-107">Aygıtlarda iş verilerini yöneten basit denetimler</span><span class="sxs-lookup"><span data-stu-id="b05e7-107">Simple controls that manage business data on devices</span></span>

- <span data-ttu-id="b05e7-108">Gelişmiş güvenlik yetenekleri.</span><span class="sxs-lookup"><span data-stu-id="b05e7-108">Advanced security capabilities.</span></span>
<span data-ttu-id="b05e7-109">[Microsoft.com'da](https://www.microsoft.com/microsoft-365/business) Microsoft 365 Business Premium hakkında daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="b05e7-109">Find out more about Microsoft 365 Business Premium at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a><span data-ttu-id="b05e7-110">Microsoft 365 İş Standardı ile Microsoft 365 Business Premium arasındaki fark nedir?</span><span class="sxs-lookup"><span data-stu-id="b05e7-110">What's the difference between Microsoft 365 Business Standard and Microsoft 365 Business Premium?</span></span>

<span data-ttu-id="b05e7-111">Bu iki planın yan yana karşılaştırmasını [Microsoft 365 Business Premium Service Description'a](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)ekledik.</span><span class="sxs-lookup"><span data-stu-id="b05e7-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Premium Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="b05e7-112">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="b05e7-112">Before you get started</span></span>

- <span data-ttu-id="b05e7-113">**Yükseltmeyi ne zaman seçmeliyim?**</span><span class="sxs-lookup"><span data-stu-id="b05e7-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="b05e7-114">Yükseltme, tek bir plana atanan **tüm kullanıcıları** yükseltmek istediğinizde doğru seçimdir.</span><span class="sxs-lookup"><span data-stu-id="b05e7-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="b05e7-115">Yükseltmeyi seçtiğinizde, tüm plan kullanıcıları aynı anda başka bir plana geçer.</span><span class="sxs-lookup"><span data-stu-id="b05e7-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="b05e7-116">Tek bir plana atanan herkesi yükseltmek istemiyorsanız, yeni plan için lisans satın alın (bu durumda Microsoft 365 Business Premium) ve bu lisansları yükseltmek istediğiniz her kullanıcıya [ayrı ayrı atayın.](../admin/manage/assign-licenses-to-users.md)</span><span class="sxs-lookup"><span data-stu-id="b05e7-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business Premium), and [assign those licenses individually](../admin/manage/assign-licenses-to-users.md) to each user that you want to upgrade.</span></span>

- <span data-ttu-id="b05e7-117">**Bazı eklentiler yükseltmeyi engelleyebilir** Bir yükseltme başlatmaya çalışırsanız ve devam etmenizi engelleyen bir eklentiniz varsa, önce eklentiyi kaldırabilir ve daha sonra gerekirse yeniden ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span>

- <span data-ttu-id="b05e7-118">**Planınızı ön ödemeniz varsa** Ön ödemeli planlar için basit bir yükseltme yolu yoktur.</span><span class="sxs-lookup"><span data-stu-id="b05e7-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="b05e7-119">Planınızı bir mağazadan satın almış olabileceğiniz bir ürün kimliği kullanarak ayarladığınızdan ön ödemeli bir planınız olup olmadığını anlarsınız.</span><span class="sxs-lookup"><span data-stu-id="b05e7-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="b05e7-120">Bir iş ortağına başvurun, Microsoft Mağazası'na gidin veya yeni bir plana geçmek için ön ödemeli planınızın süresinin dolmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business-premium"></a><span data-ttu-id="b05e7-121">Microsoft 365 Business Premium'a yükseltin</span><span class="sxs-lookup"><span data-stu-id="b05e7-121">Upgrade to Microsoft 365 Business Premium</span></span>

1. <span data-ttu-id="b05e7-122">'de yönetici merkezine giriş <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a></span><span class="sxs-lookup"><span data-stu-id="b05e7-122">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="b05e7-123">Navigasyon bölmesine gidin ve **Billing** \> **Ürünlerinizi Faturalandırma'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-123">Go to the navigation pane and select **Billing** \> **Your products**.</span></span> <span data-ttu-id="b05e7-124">Geçerli aboneliğinizi bulun ve ayrıntıları görüntülemek için aboneliğinizi seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-124">Find your current subscription and select it to view the details.</span></span>

3. <span data-ttu-id="b05e7-125">Sonraki sayfada **Yükseltme'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-125">On the next page, select **Upgrade**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="b05e7-126">**Aboneliğinizi Yükseltmenin Azure Active Directory'de grup tabanlı lisanslamayla desteklenmediğini**belirten bir ileti görürseniz, çok büyük bir kuruluşunuz yoksa bunu güvenle göz ardı edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-126">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="b05e7-127">Bu seçeneği seçen kuruluşlar, grup tabanlı lisanslama kullandıklarının farkında olurlar.</span><span class="sxs-lookup"><span data-stu-id="b05e7-127">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="b05e7-128">Ardından, yükseltebileceğiniz planların listesini görüntüleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-128">Next, you can view a list of plans that you can upgrade to.</span></span> <span data-ttu-id="b05e7-129">Bu durumda, Microsoft 365 Business Premium planını bulun.</span><span class="sxs-lookup"><span data-stu-id="b05e7-129">In this case, find the Microsoft 365 Business Premium plan.</span></span> <span data-ttu-id="b05e7-130">Bu plana dahil olan tüm uygulamaları ve hizmetleri görmek istiyorsanız aşağı kaydırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-130">You can scroll down if you want to see all the apps and services that are included with this plan.</span></span> <span data-ttu-id="b05e7-131">**Microsoft 365 Business Premium**altında, microsoft 365 Business Premium'u sepetinize eklemek için **Yükseltme'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-131">Under **Microsoft 365 Business Premium**, select **Upgrade** to add Microsoft 365 Business Premium to your cart.</span></span>

5. <span data-ttu-id="b05e7-132">Arabada:</span><span class="sxs-lookup"><span data-stu-id="b05e7-132">In the cart:</span></span>

    1. <span data-ttu-id="b05e7-133">Tüm mevcut kullanıcılarınız için otomatik olarak lisansları dahil edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-133">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="b05e7-134">Daha fazla veya daha az lisansa ihtiyacınız varsa, [bu lisansları tek tek satın almanız ve atamalısınız.](../admin/manage/assign-licenses-to-users.md)</span><span class="sxs-lookup"><span data-stu-id="b05e7-134">If you need more or fewer licenses, you need to [buy and assign those licenses individually](../admin/manage/assign-licenses-to-users.md).</span></span>  
    2. <span data-ttu-id="b05e7-135">Aylık veya yıllık ödeme yapmak istediğiniz ibareleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-135">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="b05e7-136">Seçiminizi yapmak için açılır menüyü seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-136">Select the drop-down menu to make your choice.</span></span>

6. <span data-ttu-id="b05e7-137">Bu hesabın ödeme yöntemi de dahil olmak üzere satın alma işleminizin özetini göreceğiniz **Kullanıma Git'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-137">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="b05e7-138">Ayrıca varsa buraya bir promosyon kodu ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-138">You can also add a promo code here if you have one.</span></span>

7. <span data-ttu-id="b05e7-139">Satın alma işlemini tamamlamak için **Sipariş'i** Seç'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-139">Select **Place order** to complete your purchase.</span></span>\
<span data-ttu-id="b05e7-140">Microsoft'un yeni hizmet planlarınızı ayarlaması birkaç dakika sürer.</span><span class="sxs-lookup"><span data-stu-id="b05e7-140">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="b05e7-141">İlerlemeyi denetlemek için **yükseltme durumunu denetle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-141">To check on progress, select **Check upgrade status**.</span></span>

8. <span data-ttu-id="b05e7-142">Planınız hazır olduğunda, yönetici merkezinde bazı ek kurulum adımlarını tamamlamanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="b05e7-142">When your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="b05e7-143">Gezinti bölmesinde, ek kurulum adımlarını tamamlamak için **Ana Sayfa'yı** seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-143">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="b05e7-144">Artık ihtiyacınız olmayan Microsoft 365 lisansları için eşit olarak geri ödeme alırsınız.</span><span class="sxs-lookup"><span data-stu-id="b05e7-144">You'll receive a prorated refund for the Microsoft 365 licenses that you no longer need.</span></span> <span data-ttu-id="b05e7-145">Yeni planı ayarladıktan yaklaşık iki gün sonra banka hesabınız veya kredi kartınızdan ücret tahsil edilecektir.</span><span class="sxs-lookup"><span data-stu-id="b05e7-145">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="b05e7-146">Kullanıcı cihazlarını ve dosyalarını koruma</span><span class="sxs-lookup"><span data-stu-id="b05e7-146">Protect user devices and files</span></span>

<span data-ttu-id="b05e7-147">Microsoft 365 Business Premium lisansları atandığı için, aygıtları ve dosyaları korumaya başlamak için tüm adımları niçin tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="b05e7-147">Now that Microsoft 365 Business Premium licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="b05e7-148">Yönetici merkezi gezinti bölmesinde yer alan bazı yeni seçenekleri kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="b05e7-148">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="b05e7-149">Yönetici merkezinde, gezinti bölmesinde **Devices** \> **AygıtLar İlkeleri'ne**gidin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-149">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="b05e7-150">Aygıt **ilkeleri** sayfasında **Ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-150">On the **Device policies** page, select **Add**.</span></span>

3. <span data-ttu-id="b05e7-151">**İlke Ekle** bölmesinde ilke ye bir ad verin (örneğin, çalışma dosyalarını koruyun) ve ardından açılan listeden bir **İlke türü** seçin.</span><span class="sxs-lookup"><span data-stu-id="b05e7-151">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span>

    <span data-ttu-id="b05e7-152">Android ve iPhone aygıtlarının yanı sıra Windows 10'daki dosyaları korumak için uygulama ilkeleri ayarlayabilir ve şirkete ait Windows 10 aygıtları için aygıt yapılandırma ilkeleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b05e7-152">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="b05e7-153">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="b05e7-153">See the following links for details:</span></span>

    - [<span data-ttu-id="b05e7-154">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="b05e7-154">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

    - [<span data-ttu-id="b05e7-155">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="b05e7-155">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

    - [<span data-ttu-id="b05e7-156">Windows 10 bilgisayarların aygıt koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="b05e7-156">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

4. <span data-ttu-id="b05e7-157">İlkeleri ayarladıktan sonra, siz ve çalışanlarınız aygıtlar ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b05e7-157">After you set up policies, you and your employees can set up devices:</span></span>

    - <span data-ttu-id="b05e7-158">Windows aygıtlarınız Windows Pro Creator güncelleştirmesini zaten kullanmıyorsa, [bunları Windows Pro Creators Update'e yükseltmeniz](upgrade-to-windows-pro-creators-update.md)gerekir.</span><span class="sxs-lookup"><span data-stu-id="b05e7-158">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

    - <span data-ttu-id="b05e7-159">Bkz. Windows aygıtları için adımlar [için Microsoft 365 Business Premium kullanıcıları için Windows aygıtları ayarlayın.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="b05e7-159">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span>

    - <span data-ttu-id="b05e7-160">Bkz. Android telefonlar ve iPhone'lar için adımlar için [Microsoft 365 Business Premium kullanıcıları için mobil cihazlar ayarlama.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="b05e7-160">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span>