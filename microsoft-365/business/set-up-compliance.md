---
title: Microsoft 365 Business Premium için tehdit korumasını arttırın
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Veri kaybını önlemek ve müşterilerinizin hassas bilgilerinin güvenliğini sağlamak için uyumluluk özelliklerini ayarlayın.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841183"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="63dfc-103">Uyumluluk özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="63dfc-103">Set up compliance features</span></span>

<span data-ttu-id="63dfc-104">Microsoft 365 Iş ekstra, verilerinizi ve aygıtlarınızı korumaya yönelik özelliklerle birlikte gelir ve müşterilerinizin hassas bilgilerini güvende tutmanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="63dfc-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="63dfc-105">DLP özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="63dfc-105">Set up DLP features</span></span>

<span data-ttu-id="63dfc-106">Kişisel verilerin kaybolmasını önlemek amacıyla ilke ayarlama hakkında örnek için bir [ŞABLONDAN DLP Ilkesi oluşturma](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="63dfc-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="63dfc-107">DLP, birçok farklı yerel ayar için kullanıma hazır birçok ilke şablonlarıyla gelir.</span><span class="sxs-lookup"><span data-stu-id="63dfc-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="63dfc-108">Örneğin, Avustralya finansal verileri, Kanada kişisel bilgileri, ABD finansal verileri vb.</span><span class="sxs-lookup"><span data-stu-id="63dfc-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="63dfc-109">Tam liste için [DLP ilkesi şablonlarının neler olduğunu](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) görün.</span><span class="sxs-lookup"><span data-stu-id="63dfc-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="63dfc-110">Bu şablonların tümü, PII şablon örneğine benzer şekilde etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="63dfc-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="63dfc-111">Exchange Online Arşivleme ile e-posta bekletmesini ayarlama</span><span class="sxs-lookup"><span data-stu-id="63dfc-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="63dfc-112">**Exchange Online arşivleme** lisansı özellikleri, eBulma için e-posta içeriğini koruyarak uyumluluk ve mevzuat standartlarını korumanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="63dfc-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="63dfc-113">Ayrıca, bir avda olması durumunda riskin azaltılmasına yardımcı olur ve bir güvenlik ihlalinin ardından silinmiş öğeleri kurtarmanız gerektiğinde verilerin kurtarılması için bir yol sağlar.</span><span class="sxs-lookup"><span data-stu-id="63dfc-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="63dfc-114">Bir kullanıcının içeriğinin tümünü korumak veya korumak istediğiniz öğeyi özelleştirmek için bekletme ilkeleri 'ni kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="63dfc-115">Dava **tutma:** Bir kullanıcının tüm posta kutusunu dava tutma ile birlikte bırakarak silinmiş öğeler dahil tüm posta kutusu içeriğini koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="63dfc-116">Posta kutusunu, bir posta kutusu</span><span class="sxs-lookup"><span data-stu-id="63dfc-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="63dfc-117">Sol gezintide, **Kullanıcılar** \> **etkin kullanıcılarına** gidin.</span><span class="sxs-lookup"><span data-stu-id="63dfc-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="63dfc-118">Posta kutusunu basılı tutma için yerleştirmek istediğiniz kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="63dfc-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="63dfc-119">Kullanıcı bölmesinde **posta ayarlarını** genişletin ve **daha fazla ayar** 'Nın yanında **Exchange özelliklerini Düzenle** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="63dfc-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="63dfc-120">Kullanıcının posta kutusu sayfasında, sol gezinti bölmesinde \* \* posta kutusu özellikleri \* \* seçeneğini belirleyin ve sonra da bir bağlantı altında **saklama** bağlantısını **Etkinleştir** 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="63dfc-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="63dfc-121">**Katmanlama bekletme** iletişim kutusunda, dava tutma **süresi** alanında dava tutma süresini belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="63dfc-122">Sonsuz bir bekletme yerleştirmek istiyorsanız alanı boş bırakın.</span><span class="sxs-lookup"><span data-stu-id="63dfc-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="63dfc-123">Ayrıca not ekleyebilir ve posta kutusu sahibini bir Web sitesine yönlendirebilirsiniz, bir dava alma hakkında daha fazla bilgi edinebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="63dfc-124">\>**Kaydetme**.</span><span class="sxs-lookup"><span data-stu-id="63dfc-124">\> **Save**.</span></span>
    
<span data-ttu-id="63dfc-125">**Bekletme:** Özel bekletme ilkelerini, örneğin belirli bir süre boyunca korumak veya saklama döneminin sonunda içeriği kalıcı olarak silmek için etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="63dfc-126">Daha fazla bilgi edinmek için [bekletme Ilkelerine genel bakış](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="63dfc-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="63dfc-127">Duyarlılık etiketlerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="63dfc-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="63dfc-128">Duyarlılık etiketleri Azure bilgi koruması (AıP) plan 1 ile gelir ve etiket uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="63dfc-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="63dfc-129">Etiketler, kuralları ve koşulları tanımlayan ve kullanıcılar tarafından el ile veya kullanıcıların öneri verdiği bileşimi kullanarak otomatik olarak uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="63dfc-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="63dfc-130">Duyarlılık etiketlerini ayarlamak için, [duyarlılık etiketleri oluşturma ve yönetme](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videosu.</span><span class="sxs-lookup"><span data-stu-id="63dfc-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="63dfc-131">Azure bilgi Koruması istemcisini el ile yükleme</span><span class="sxs-lookup"><span data-stu-id="63dfc-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="63dfc-132">AıP istemcisini el ile yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="63dfc-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="63dfc-133">[Microsoft İndirme merkezinden](https://www.microsoft.com/download/details.aspx?id=53018) **AzinfoProtection_UL.exe** indirin.</span><span class="sxs-lookup"><span data-stu-id="63dfc-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="63dfc-134">Bir Word belgesini görüntüleyerek ve **giriş** sekmesinde **duyarlılık** seçeneğinin kullanılabilir olduğundan emin olmak için yüklemenin çalıştığını doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63dfc-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="63dfc-135">![Word belgesinde koruma sekmesi açılır.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="63dfc-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="63dfc-136">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="63dfc-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
