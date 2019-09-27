---
title: Microsoft 365 Business için tehdit korumayı artırın
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş Tehdit Koruması'nı ayarlayın ve hassas verileri koruyun.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288755"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="afc8f-103">Uyumluluk özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="afc8f-103">Set up compliance features</span></span>

<span data-ttu-id="afc8f-104">Microsoft 365 Business'ınız verilerinizi ve cihazlarınızı koruyan ve sizin ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olan özelliklerle birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="afc8f-105">DLP özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="afc8f-105">Set up DLP features</span></span>

<span data-ttu-id="afc8f-106">Bkz. Kişisel olarak tanımlanabilir bilgilere (PII) karşı korumak için bir ilke oluşturma hakkında bir örnek için şablondan Bir [DLP ilkesi oluşturun.](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369)</span><span class="sxs-lookup"><span data-stu-id="afc8f-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="afc8f-107">DLP, birçok farklı yerel bölge için kullanıma hazır ilke şablonlarıyla birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="afc8f-108">Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri, vb. Tam liste için [DLP ilkesi şablonlarının neler içerdiğini](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) görün.</span><span class="sxs-lookup"><span data-stu-id="afc8f-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="afc8f-109">Bu şablonların tümü, KIŞISEL bilgiler şablonu örneğine benzer şekilde etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="afc8f-110">Exchange Online Arşivleme ile e-posta saklama yı ayarlama</span><span class="sxs-lookup"><span data-stu-id="afc8f-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="afc8f-111">**Exchange Online Arşivleme** lisansı özellikleri, e-posta içeriğini eDiscovery için koruyarak uyumluluk ve mevzuat standartlarını korumaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="afc8f-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="afc8f-112">Ayrıca, bir dava durumunda riskinizi azaltmaya yardımcı olur ve bir güvenlik ihlalinden sonra veya silinen öğeleri kurtarmanız gerektiğinde verileri kurtarmanın bir yolunu sağlar.</span><span class="sxs-lookup"><span data-stu-id="afc8f-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="afc8f-113">Bir kullanıcının tüm içeriğini korumak için dava tutma yı kullanabilir veya korumak istediğiniz şeyi özelleştirmek için bekletme ilkelerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="afc8f-114">**Dava tutma:** Bir kullanıcının tüm posta kutusunu dava beklemeye alarak silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="afc8f-115">Yönetici merkezinde, dava beklemeye bir posta kutusu yerleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="afc8f-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="afc8f-116">Sol navigasyonda, **Users** \> **Active kullanıcılarına**gidin.</span><span class="sxs-lookup"><span data-stu-id="afc8f-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="afc8f-117">Dava beklemeye ve kullanıcı bölmesine yerleştirmek istediğiniz posta kutusunu seçin **Posta ayarlarını** genişletin ve **Daha Fazla ayar** yanında Exchange özelliklerini **düzenleyin'** i seçin.</span><span class="sxs-lookup"><span data-stu-id="afc8f-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="afc8f-118">Kullanıcı için posta kutusu sayfasında, sol daki \*\* posta kutusu özelliklerini seçin ve ardından **Dava bekletme**altında **Etkinleştir** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="afc8f-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="afc8f-119">Dava **tutma** iletişim kutusunda, **dava bekleme süresi** alanında dava tutma süresini belirtebilir, sonsuz bir bekleme yerleştirmek istiyorsanız alanı boş bırakabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="afc8f-120">Ayrıca notlar ekleyebilir ve posta kutusu sahibini \> **kaydet**davası hakkında daha fazla açıklama yapmak zorunda kabileceğiniz bir web sitesine yönlendirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="afc8f-121">**Bekletme:** Örneğin, belirli bir süre için korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="afc8f-122">Daha fazla bilgi için [bkz.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)</span><span class="sxs-lookup"><span data-stu-id="afc8f-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="afc8f-123">Azure Bilgi Koruması özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="afc8f-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="afc8f-124">Azure Bilgi Koruması (AIP), etiketler uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="afc8f-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="afc8f-125">Etiketler, kuralları ve koşulları tanımlayan yöneticiler tarafından, kullanıcılar tarafından el ile veya kullanıcılara önerilerin verildiği bir kombinasyon kullanılarak otomatik olarak uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="afc8f-126">Web'deki Outlook'ta e-postalarınıza aşağıdaki yerleşik etiketleri ve kısıtlamaları uygulayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="afc8f-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="afc8f-127">**İletme :** Alıcılar iletiyi okuyabilir, ancak içeriği iletemez, yazdıramaz veya kopyalayamaz</span><span class="sxs-lookup"><span data-stu-id="afc8f-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="afc8f-128">**Şifrele**: İletinin tamamı şifrelenir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="afc8f-129">Alıcıların şifreli içeriğe erişmeden önce kimliklerini doğrulamaları ve şifrelemeyi kaldıramamaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="afc8f-130">**Gizli**: Kuruluşunuzdaki çalışanlara e-posta içeriği ne kadar e-posta içeriğine ve ekleri için tam izin verir, ancak kuruluşunuz dışındaki kişilere tam izin verir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="afc8f-131">Veri sahipleri herhangi bir noktada içeriği izleyebilir ve iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="afc8f-132">**Son Derece Gizli**: Bu kısıtlama, çalışanların verileri görüntülemesine, görüntülemesine ve yanıtlamasına izin veren, ancak verileri iletmeme, yazdırmama veya kopyalamama olanağı tanıyan son derece gizli verilere uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="afc8f-133">Veri sahipleri herhangi bir noktada içeriği izleyebilir ve iptal edebilir.</span><span class="sxs-lookup"><span data-stu-id="afc8f-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="afc8f-134">Azure Bilgi Korumasının etkinleştirildiğinden emin olun</span><span class="sxs-lookup"><span data-stu-id="afc8f-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="afc8f-135">AIP'nin etkinleştirildiğini doğrulamak için:</span><span class="sxs-lookup"><span data-stu-id="afc8f-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="afc8f-136">Azure [portalında](https://portal.azure.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="afc8f-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="afc8f-137">**Tüm hizmetleri** seçin ve **Arama Kutusu'nda**Azure *Bilgi Koruması* yazın.</span><span class="sxs-lookup"><span data-stu-id="afc8f-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="afc8f-138">Sonuçlar görüntülendikten sonra, sık kullanılan ve daha sonra kolayca bulunmasını sağlamak için **Azure Bilgi Koruması'nın** yanındaki başlat'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="afc8f-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="afc8f-139">**Azure Bilgi Koruması** \> **Koruması etkinleştirmesini** seçin ve durumun etkinleştirilecek şekilde ayarlandıklarına emin olun.</span><span class="sxs-lookup"><span data-stu-id="afc8f-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="afc8f-140">Azure Bilgi Koruması ilkesini ve varsayılan etiketleri görüntüleyin</span><span class="sxs-lookup"><span data-stu-id="afc8f-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="afc8f-141">Varolan etiketleri görüntülemek ve değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="afc8f-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="afc8f-142">Azure Bilgi Koruması panosunda Sınıflandırma \> **Etiketleri'ni**seçin. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="afc8f-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="afc8f-143">![Azure Bilgi Koruması için standart etiketler.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="afc8f-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="afc8f-144">Seçenekleri görüntülemek için herhangi bir etiket seçebilirsiniz, ekran adını, renkleri, vb değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="afc8f-145">Bkz. Kendi etiketinizi oluşturmak istiyorsanız [Değiştir ve yeni etiketler oluşturun.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2)</span><span class="sxs-lookup"><span data-stu-id="afc8f-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="afc8f-146">Azure Bilgi Koruması istemcisini el ile yükleme</span><span class="sxs-lookup"><span data-stu-id="afc8f-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="afc8f-147">AIP istemcisini el ile yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="afc8f-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="afc8f-148">[Microsoft indirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzInfoProtection.exe** indirin.</span><span class="sxs-lookup"><span data-stu-id="afc8f-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="afc8f-149">Yüklemenin bir Word belgesini görüntüleyerek ve **Koruma** seçeneğinin **Ana sayfa** sekmesinde kullanılabilir olduğundan emin olarak çalıştığını doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="afc8f-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="afc8f-150">![Word belgesinde koruma sekmesi açılır.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="afc8f-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="afc8f-151">Daha fazla bilgi için bkz: [Istemciyi yükleyin.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="afc8f-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
