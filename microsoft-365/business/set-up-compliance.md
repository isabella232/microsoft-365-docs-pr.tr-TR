---
title: Microsoft 365 Business için tehdit korumayı artırın
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
description: Veri kaybını önlemek ve sizin ve müşterilerinizin hassas bilgilerinin güvenliğini sağlamaya yardımcı olmak için uyumluluk özellikleri ayarlayın.
ms.openlocfilehash: 4c8efc4ca96f2db7bc4d1592ad3fdc85dfb6b3b5
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550067"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="1afec-103">Uyumluluk özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="1afec-103">Set up compliance features</span></span>

<span data-ttu-id="1afec-104">Microsoft 365 Business'ınız verilerinizi ve cihazlarınızı koruyan ve sizin ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olan özelliklerle birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="1afec-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="1afec-105">DLP özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="1afec-105">Set up DLP features</span></span>

<span data-ttu-id="1afec-106">Bkz. Kişisel olarak tanımlanabilir bilgilere (PII) karşı korumak için bir ilke oluşturma hakkında bir örnek için şablondan Bir [DLP ilkesi oluşturun.](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369)</span><span class="sxs-lookup"><span data-stu-id="1afec-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="1afec-107">DLP, birçok farklı yerel bölge için kullanıma hazır ilke şablonlarıyla birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="1afec-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="1afec-108">Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri ve benzeri.</span><span class="sxs-lookup"><span data-stu-id="1afec-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="1afec-109">Tam liste için [DLP ilkesi şablonlarının neler içerdiğini](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) görün.</span><span class="sxs-lookup"><span data-stu-id="1afec-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="1afec-110">Bu şablonların tümü, KIŞISEL bilgiler şablonu örneğine benzer şekilde etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="1afec-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="1afec-111">Exchange Online Arşivleme ile e-posta saklama yı ayarlama</span><span class="sxs-lookup"><span data-stu-id="1afec-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="1afec-112">**Exchange Online Arşivleme** lisansı özellikleri, e-posta içeriğini eDiscovery için koruyarak uyumluluk ve mevzuat standartlarını korumaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="1afec-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="1afec-113">Ayrıca, bir dava varsa riskinizi azaltmaya yardımcı olur ve bir güvenlik ihlalinden sonra veya silinen öğeleri kurtarmanız gerektiğinde verileri kurtarmanın bir yolunu sağlar.</span><span class="sxs-lookup"><span data-stu-id="1afec-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="1afec-114">Bir kullanıcının tüm içeriğini korumak için dava tutma yı kullanabilir veya korumak istediğiniz şeyi özelleştirmek için bekletme ilkelerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="1afec-115">**Dava tutma:** Bir kullanıcının tüm posta kutusunu dava beklemeye alarak silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="1afec-116">Yönetici merkezinde, dava beklemeye bir posta kutusu yerleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="1afec-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="1afec-117">Sol navigasyonda, **Users** \> **Active kullanıcılarına**gidin.</span><span class="sxs-lookup"><span data-stu-id="1afec-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="1afec-118">Dava beklemeye almak istediğiniz posta kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="1afec-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="1afec-119">Kullanıcı **bölmesinde, Posta ayarlarını**genişletin ve **Daha Fazla ayar'ın**yanında **Exchange özelliklerini edit'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="1afec-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="1afec-120">Kullanıcı için posta kutusu sayfasında, sol daki \*\* posta kutusu özelliklerini seçin ve ardından **Dava bekletme**altında **Etkinleştir** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="1afec-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="1afec-121">Dava **tutma** iletişim kutusunda, **Dava tutma süresi** alanında dava tutma süresini belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="1afec-122">Sonsuz bir tutma yerleştirmek istiyorsanız alanı boş bırakın.</span><span class="sxs-lookup"><span data-stu-id="1afec-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="1afec-123">Ayrıca notlar ekleyebilir ve posta kutusu sahibini dava tutma hakkında daha fazla açıklama nız gerekebilecek bir web sitesine yönlendirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="1afec-124">\>**Kaydet.**</span><span class="sxs-lookup"><span data-stu-id="1afec-124">\> **Save**.</span></span>
    
<span data-ttu-id="1afec-125">**Bekletme:** Örneğin, belirli bir süre için korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="1afec-126">Daha fazla bilgi için [bkz.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)</span><span class="sxs-lookup"><span data-stu-id="1afec-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="1afec-127">Duyarlılık etiketlerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="1afec-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="1afec-128">Duyarlılık etiketleri Azure Bilgi Koruması (AIP) Planı 1 ile birlikte gelir ve etiketler uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="1afec-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="1afec-129">Etiketler, kuralları ve koşulları tanımlayan yöneticiler tarafından, kullanıcılar tarafından el ile veya kullanıcılara önerilerin verildiği bir kombinasyon kullanılarak otomatik olarak uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="1afec-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="1afec-130">Duyarlılık etiketleri ayarlamak [için, duyarlılık etiketleri videosu oluşturma ve yönetme](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) yi görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="1afec-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="1afec-131">Azure Bilgi Koruması istemcisini el ile yükleme</span><span class="sxs-lookup"><span data-stu-id="1afec-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="1afec-132">AIP istemcisini el ile yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="1afec-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="1afec-133">[Microsoft indirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzinfoProtection_UL.exe** indirin.</span><span class="sxs-lookup"><span data-stu-id="1afec-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="1afec-134">Yüklemenin bir Word belgesini görüntüleyerek ve **Duyarlılık** seçeneğinin **Giriş** sekmesinde kullanılabilir olduğundan emin olarak çalıştığını doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1afec-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="1afec-135">![Word belgesinde koruma sekmesi açılır.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="1afec-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="1afec-136">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="1afec-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
