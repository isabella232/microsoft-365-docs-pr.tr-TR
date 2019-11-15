---
title: Office 365 Business Premium'dan Microsoft 365 Business'a yükseltme
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
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: İşletmenizi Office 365 Business Premium'dan Microsoft 365 Business'a yükselten adımlar.
ms.openlocfilehash: 95c4504d7e6e33bdededee0cfca7add0cb5f7204
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640571"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="fc1cf-103">Office 365 Business Premium'dan Microsoft 365 Business'a yükseltme</span><span class="sxs-lookup"><span data-stu-id="fc1cf-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="fc1cf-104">İş aboneliği için bir [Office 365'iniz](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)varsa (örneğin, Office 365 Business Premium), Microsoft 365 Business'a kolayca yükseltebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="fc1cf-105">Eklemek isterseniz Microsoft 365 Business'a yükseltin:</span><span class="sxs-lookup"><span data-stu-id="fc1cf-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="fc1cf-106">Windows 10 Pro (Windows 8 veya sonraki çalıştıran bilgisayarlarına)</span><span class="sxs-lookup"><span data-stu-id="fc1cf-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="fc1cf-107">Aygıtlarda iş verilerini yöneten basit denetimler</span><span class="sxs-lookup"><span data-stu-id="fc1cf-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="fc1cf-108">Gelişmiş güvenlik yetenekleri.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-108">Advanced security capabilities.</span></span>
<span data-ttu-id="fc1cf-109">[Microsoft.com'da](https://www.microsoft.com/microsoft-365/business) Microsoft 365 Business hakkında daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="fc1cf-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="fc1cf-110">Office 365 Business Premium ile Microsoft 365 Business arasındaki fark nedir?</span><span class="sxs-lookup"><span data-stu-id="fc1cf-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="fc1cf-111">Bu iki planın yan yana karşılaştırmasını [Microsoft 365 İş Hizmeti Açıklaması'na](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description)ekledik.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="fc1cf-112">Başlamadan önce</span><span class="sxs-lookup"><span data-stu-id="fc1cf-112">Before you get started</span></span>

- <span data-ttu-id="fc1cf-113">**Yükseltmeyi ne zaman seçmeliyim?**</span><span class="sxs-lookup"><span data-stu-id="fc1cf-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="fc1cf-114">Yükseltme, tek bir plana atanan **tüm kullanıcıları** yükseltmek istediğinizde doğru seçimdir.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="fc1cf-115">Yükseltmeyi seçtiğinizde, tüm plan kullanıcıları aynı anda başka bir plana geçer.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="fc1cf-116">Tek bir plana atanan herkesi yükseltmek istemiyorsanız, yeni plan için lisans satın alın (bu durumda Microsoft 365 Business) ve bu lisansları yükseltmek istediğiniz her kullanıcıya [ayrı ayrı atayın.](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="fc1cf-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="fc1cf-117">**Bazı eklentiler yükseltmeyi engelleyebilir** Bir yükseltme başlatmaya çalışırsanız ve devam etmenizi engelleyen bir eklentiniz varsa, önce eklentiyi kaldırabilir ve daha sonra gerekirse yeniden ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span> 
- <span data-ttu-id="fc1cf-118">**Planınızı ön ödemeniz varsa** Ön ödemeli planlar için basit bir yükseltme yolu yoktur.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="fc1cf-119">Planınızı bir mağazadan satın almış olabileceğiniz bir ürün kimliği kullanarak ayarladığınızdan ön ödemeli bir planınız olup olmadığını anlarsınız.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="fc1cf-120">Bir iş ortağına başvurun, Microsoft Mağazası'na gidin veya yeni bir plana geçmek için ön ödemeli planınızın süresinin dolmasını bekleyin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="fc1cf-121">Microsoft 365 Business'a yükseltme</span><span class="sxs-lookup"><span data-stu-id="fc1cf-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="fc1cf-122">[Yeni yönetici merkezinde](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)aşağıdaki adımları izleyerek lisanslarınızı satın alın:</span><span class="sxs-lookup"><span data-stu-id="fc1cf-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="fc1cf-123">'de <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>yönetici merkezine giriş</span><span class="sxs-lookup"><span data-stu-id="fc1cf-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="fc1cf-124">Gezinti bölmesine gidin ve **Faturalama** \> Ürünleri **& Hizmetleri'ni**seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="fc1cf-125">Office 365 aboneliğinizi bulun ve ayrıntıları görüntülemek için bu aboneliği seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Ekran görüntüsü, yönetici merkezinde aboneliğinizi nasıl bulabileceğinizi ve seçileceksiniz.](media/FindYourSubscription.png)

3. <span data-ttu-id="fc1cf-127">Sonraki sayfada **Yükseltme'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-127">On the next page, select **Upgrade**.</span></span> 

      ![Ekran görüntüsü, yönetici merkezinde Yükseltme'nin nerede seçilen olduğunu gösterir.](media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="fc1cf-129">**Aboneliğinizi Yükseltmenin Azure Active Directory'de grup tabanlı lisanslamayla desteklenmediğini**belirten bir ileti görürseniz, çok büyük bir kuruluşunuz yoksa bunu güvenle göz ardı edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-129">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="fc1cf-130">Bu seçeneği seçen kuruluşlar, grup tabanlı lisanslama kullandıklarının farkında olurlar.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="fc1cf-131">Ardından, yükseltebileceğiniz Office planlarının listesini görüntüleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="fc1cf-132">Bu durumda, Microsoft 365 İş planını bulun.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="fc1cf-133">Bu plana dahil olan tüm Office uygulamalarını ve hizmetlerini görmek istiyorsanız aşağı kaydırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="fc1cf-134">**Microsoft 365 Business**altında, microsoft 365 Business'ı sepetinize eklemek için **Yükseltme'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="fc1cf-135">Arabada:</span><span class="sxs-lookup"><span data-stu-id="fc1cf-135">In the cart:</span></span>
    1. <span data-ttu-id="fc1cf-136">Tüm mevcut kullanıcılarınız için otomatik olarak lisansları dahil edeceğiz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-136">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="fc1cf-137">Daha fazla veya daha az lisansa ihtiyacınız varsa, [bu lisansları tek tek satın almanız ve atamalısınız.](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="fc1cf-137">If you need more or fewer licenses, you need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="fc1cf-138">Aylık veya yıllık ödeme yapmak istediğiniz ibareleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-138">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="fc1cf-139">Seçiminizi yapmak için açılır menüyü seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="fc1cf-140">Bu hesabın ödeme yöntemi de dahil olmak üzere satın alma işleminizin özetini göreceğiniz **Kullanıma Git'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="fc1cf-141">Ayrıca varsa buraya bir promosyon kodu ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="fc1cf-142">Satın alma işlemini tamamlamak için **Sipariş'i Yerleştir'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="fc1cf-143">Microsoft'un yeni hizmet planlarınızı ayarlaması birkaç dakika sürer.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="fc1cf-144">İlerlemeyi denetlemek için **yükseltme durumunu denetle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="fc1cf-145">Planınız hazır olduğunda, yönetici merkezinde bazı ek kurulum adımlarını tamamlamanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="fc1cf-146">Gezinti bölmesinde, ek kurulum adımlarını tamamlamak için **Ana Sayfa'yı** seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="fc1cf-147">Artık ihtiyacınız olmayan Ofifce 365 lisansları için eşit olarak geri ödeme alırsınız.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-147">You'll receive a prorated refund for the Ofifce 365 licenses that you no longer need.</span></span> <span data-ttu-id="fc1cf-148">Yeni planı ayarladıktan yaklaşık iki gün sonra banka hesabınız veya kredi kartınızdan ücret tahsil edilecektir.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="fc1cf-149">Kullanıcı cihazlarını ve dosyalarını koruma</span><span class="sxs-lookup"><span data-stu-id="fc1cf-149">Protect user devices and files</span></span>

<span data-ttu-id="fc1cf-150">Microsoft 365 İşletme lisansları atandığı için, aygıtları ve dosyaları korumaya başlamak için tüm adımları niçin tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="fc1cf-151">Yönetici merkezi gezinti bölmesinde yer alan bazı yeni seçenekleri kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-151">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="fc1cf-152">Yönetici merkezinde, gezinti bölmesinde AygıtLar \*\*\*\* \> **İlkeleri'ne**gidin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="fc1cf-153">Aygıt **ilkeleri** sayfasında **Ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="fc1cf-154">**İlke Ekle** bölmesinde ilke ye bir ad verin (örneğin, çalışma dosyalarını koruyun) ve ardından açılan listeden bir **İlke türü** seçin.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span> 
    
    <span data-ttu-id="fc1cf-155">Android ve iPhone aygıtlarının yanı sıra Windows 10'daki dosyaları korumak için uygulama ilkeleri ayarlayabilir ve şirkete ait Windows 10 aygıtları için aygıt yapılandırma ilkeleri ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="fc1cf-156">Ayrıntılar için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="fc1cf-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="fc1cf-157">Android veya iOS cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="fc1cf-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="fc1cf-158">Windows 10 cihazlarına yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="fc1cf-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="fc1cf-159">Windows 10 bilgisayarların aygıt koruma ayarlarını ayarlama</span><span class="sxs-lookup"><span data-stu-id="fc1cf-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="fc1cf-160">İlkeleri ayarladıktan sonra, siz ve çalışanlarınız aygıtlar ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="fc1cf-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="fc1cf-161">Windows aygıtlarınız Windows Pro Creator güncelleştirmesini zaten kullanmıyorsa, [bunları Windows Pro Creators Update'e yükseltmeniz](upgrade-to-windows-pro-creators-update.md)gerekir.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="fc1cf-162">Bkz. Windows aygıtları için adımlar [için Microsoft 365 İş kullanıcıları için Windows aygıtları ayarlama.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="fc1cf-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="fc1cf-163">Bkz. Android telefonlar ve iPhone'lar için adımlar için [Microsoft 365 Business kullanıcıları](set-up-mobile-devices.md) için mobil cihazlar ayarlama.</span><span class="sxs-lookup"><span data-stu-id="fc1cf-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
