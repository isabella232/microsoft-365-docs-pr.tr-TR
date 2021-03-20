---
title: Microsoft 365 İş Ekstra için tehdit korumasını artırma
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
description: Veri kaybını önlemek ve müşterilerimizin hassas bilgilerini güvende tutmaya yardımcı olmak için uyumluluk özelliklerini ayarlayın.
ms.openlocfilehash: e210787718025c5df29af8d4a2283291dcecc2a8
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912540"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="a0bd9-103">Uyumluluk özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="a0bd9-103">Set up compliance features</span></span>

<span data-ttu-id="a0bd9-104">Microsoft 365 İş Ekstra, verilerinizi ve cihazlarınızı korumaya ve müşterilerimizin hassas bilgilerini güvende tutmanıza yardımcı olacak özelliklerle birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="a0bd9-105">DLP özelliklerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="a0bd9-105">Set up DLP features</span></span>

<span data-ttu-id="a0bd9-106">Kişisel [verilerin kaybına karşı korunmak için](../compliance/create-a-dlp-policy-from-a-template.md) bir ilke ayarlama örneği için, şablondan DLP ilkesi oluşturma hakkında bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="a0bd9-107">DLP, birçok farklı yerel ayarın kullanımına hazır ilke şablonlarıyla birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="a0bd9-108">Örneğin, Avustralya Finansal Verileri, Kanada Kişisel Bilgiler Yasası, ABD Finansal Verileri, gibi.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="a0bd9-109">Tam [liste için DLP ilkesi şablonlarının](../compliance/what-the-dlp-policy-templates-include.md) neler içermesi hakkında bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="a0bd9-110">Bu şablonların hepsi, PII şablonu örneğine benzer şekilde etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="a0bd9-111">Exchange Online Arşivleme ile e-posta bekletmeyi ayarlama</span><span class="sxs-lookup"><span data-stu-id="a0bd9-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="a0bd9-112">**Exchange Online Arşivleme lisans** özellikleri, eBulma için e-posta içeriğini koruyarak uyumluluk ve mevzuat standartlarının korunmasına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="a0bd9-113">Ayrıca, bir sorun olduğu zaman risklerinizi azaltmaya yardımcı olur ve güvenlik ihlali sonrasında veya silinmiş öğeleri kurtarmanız gereken zaman verileri kurtarmak için bir yol sağlar.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="a0bd9-114">Bir kullanıcının içeriğinin hepsini korumak için mahkeme tutma veya korumak istediğiniz içeriği özelleştirmek için bekletme ilkelerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="a0bd9-115">**Mahkeme tutma:** Silinen öğeler de dahil olmak üzere tüm posta kutusu içeriğini, kullanıcının posta kutusunun tamamını mahkemelere koyarak koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="a0bd9-116">Posta kutusunu mahkeme tutmada tutmak için Yönetim merkezinde:</span><span class="sxs-lookup"><span data-stu-id="a0bd9-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="a0bd9-117">Sol gezintide, Kullanıcılar Etkin  \> **kullanıcılar'a gidin.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="a0bd9-118">Posta kutusunu mahkeme tutması için kullanmak istediğiniz bir kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="a0bd9-119">Kullanıcı bölmesinde Posta ayarlarını genişletin ve **Diğer ayarlar'ın** **yanında** Exchange özelliklerini **düzenle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="a0bd9-120">Kullanıcının posta kutusu sayfasında, sol gezintide \*\* posta kutusu özellikleri  \*\* seçin ve ardından Mahkeme tutma altındaki Etkinleştir **bağlantısını seçin.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="a0bd9-121">Mahkeme **tutma iletişim kutusunda,** Mahkeme tutma süresi alanında mahkeme tutma **süresini belirtebilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="a0bd9-122">Sonsuz bir tutunma yapmak için alanı boş bırakın.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="a0bd9-123">Ayrıca, not ekleyebilir ve posta kutusu sahibini mahkeme tutma hakkında daha fazla açıklamanız gerekten bir web sitesine yönlendirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="a0bd9-124">\>**Kaydet 'i tıklatın.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-124">\> **Save**.</span></span>
    
<span data-ttu-id="a0bd9-125">**Bekletme:** Örneğin, belirli bir süre boyunca korumak veya bekletme döneminin sonunda içeriği kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="a0bd9-126">Daha fazla bilgi edinmek için, bekletme [ilkelerine Genel Bakış'a bakın.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="a0bd9-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="a0bd9-127">Duyarlılık etiketlerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="a0bd9-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="a0bd9-128">Duyarlılık etiketleri Azure Information Protection (AIP) Plan 1 ile birlikte gelir ve etiketleri uygulayarak belgelerinizi ve e-postalarınızı sınıflandırmanıza ve isteğe bağlı olarak korumanıza yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="a0bd9-129">Etiketler, kurallar ve koşullar tanımlayan yöneticiler, kullanıcılar tarafından el ile veya kullanıcıların önerilerinin verildiği bir birleşim kullanılarak otomatik olarak uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="a0bd9-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="a0bd9-130">Duyarlılık etiketlerini ayarlamak için, duyarlılık [etiketleri videosunu oluşturun ve yönetin.](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="a0bd9-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="a0bd9-131">Azure Information Protection istemcisini el ile yükleme</span><span class="sxs-lookup"><span data-stu-id="a0bd9-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="a0bd9-132">AIP istemcisini el ile yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="a0bd9-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="a0bd9-133">Microsoft **AzinfoProtection_UL.exe** [merkezinden indirin.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="a0bd9-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="a0bd9-134">Bir Word belgesini görüntüerek ve Giriş sekmesinde Duyarlılık seçeneğinin kullanılabilir olduğundan emin **olarak** yüklemenin çalıştığını **doğruleyebilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="a0bd9-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="a0bd9-135">![Word belgesinde Koruma sekmesi açılan listesinde.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="a0bd9-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="a0bd9-136">Daha fazla bilgi için [bkz. İstemciyi yükleme.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="a0bd9-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>