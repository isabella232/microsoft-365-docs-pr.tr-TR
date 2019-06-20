---
title: Microsoft 365 iş için tehdit koruma artırın
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
search.appverid:
- BCS160
- MET150
description: Office 365 Gelişmiş tehdit koruma sisteminizi kurma ve hassas verilerinizi korumak.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086412"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="6cd92-103">Uyumluluk Özellikleri Kurma</span><span class="sxs-lookup"><span data-stu-id="6cd92-103">Set up compliance features</span></span>

<span data-ttu-id="6cd92-104">Microsoft 365 iş verilerinizi ve aygıtları korumak ve sizin ve müşterilerinizin önemli bilgilerin güvenliğini sağlamanıza yardımcı olmak için özellikler bulunur.</span><span class="sxs-lookup"><span data-stu-id="6cd92-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="6cd92-105">DLP özellikleri kurma</span><span class="sxs-lookup"><span data-stu-id="6cd92-105">Set up DLP features</span></span>

<span data-ttu-id="6cd92-106">[Bir şablondan bir DLP ilkesi oluşturma](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) kişisel olarak tanımlanabilen bilgiler (PII) karşı korumak için bir ilke ayarlama konusunda bir örnek için bkz.</span><span class="sxs-lookup"><span data-stu-id="6cd92-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="6cd92-107">DLP birçok farklı yerel ayarlar için birçok hazır kullanım ilkesi şablonuyla birlikte gelir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="6cd92-108">Örneğin, Avustralya mali verileri, kişisel bilgi Act Kanada, ABD finansal veriler, vb.. [Ne DLP ilke şablonları dahil](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) tam bir listesi için bkz.</span><span class="sxs-lookup"><span data-stu-id="6cd92-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="6cd92-109">Tüm bu şablonları PII şablon örneğe benzer şekilde etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="6cd92-110">E-posta bekletme çevrimiçi Exchange arşivleme ile ayarlama</span><span class="sxs-lookup"><span data-stu-id="6cd92-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="6cd92-111">**Exchange Online arşivleme** lisans özellikleri, uyumluluk ve yasal standartlar tarafından e-posta koruma eBulma için içerik sağlamak yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6cd92-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="6cd92-112">Ayrıca, bir açtığı dava sonucunda durumunda riskini azaltmaya yardımcı olur ve sonra bir güvenlik ihlali veya silinmiş öğeleri kurtarmak gereksinim duyduğunuzda verileri kurtarmak için bir yol sağlar.</span><span class="sxs-lookup"><span data-stu-id="6cd92-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="6cd92-113">Tüm kullanıcı içeriğini korumak için dava tutma kullanın veya korumak istediğiniz özelleştirmek için bekletme ilkeleri kullanın.</span><span class="sxs-lookup"><span data-stu-id="6cd92-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="6cd92-114">**Dava tutun:** Dava üzerinde bir kullanıcının tüm posta koyarak dahil silinmiş öğeleri tutma tüm posta kutusu içeriğini koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6cd92-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="6cd92-115">Dava Tutuluyor, Yönetim Merkezi bir posta kutusu yerleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="6cd92-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="6cd92-116">Sol nav uygulamasında, **Kullanıcılar** için giderek \> **Etkin kullanıcılar**.</span><span class="sxs-lookup"><span data-stu-id="6cd92-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="6cd92-117">Dava üzerinde yerleştirmek istediğiniz alıcının posta kutusu tutun bir kullanıcı seçin ve kullanıcı Bölmesi'nde **posta ayarları** ' nı genişletin ve **Exchange düzenleme özellikleri**yanında **daha fazla ayar** seçin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="6cd92-118">Kullanıcının posta kutusu sayfasında seçin \*\* posta kutusu özellikleri \*\* üzerinde sol nav ve **dava tutun**altında **Etkinleştir** bağlantısını seçin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="6cd92-119">**Dava tutun** dava belirtebileceğiniz iletişim kutusunu **dava tutma süresi** alanında süre basılı tutun, alan sonsuz bir ayrı tutma yerleştirmek isterseniz boş bırakın.</span><span class="sxs-lookup"><span data-stu-id="6cd92-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="6cd92-120">Ayrıca notlar ekleyin ve posta kutusu sahibi dava hakkında daha fazla tutun açıklamak için sahip olabileceği bir Web sitesine doğrudan \> **kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="6cd92-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="6cd92-121">**Tutma:** Belirli bir süre korumak veya içeriği saklama dönemi sonunda kalıcı olarak silmek için özelleştirilmiş bekletme ilkelerini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6cd92-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="6cd92-122">Daha fazla bilgi için [Bekletme İlkeleri'ne genel bakış](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="6cd92-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="6cd92-123">Azure bilgi koruma özellikleri kurma</span><span class="sxs-lookup"><span data-stu-id="6cd92-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="6cd92-124">Azure bilgi koruma (AIP) sınıflandırmak ve etiketleri uygulayarak belgeler ve e-postalar, isteğe bağlı olarak, korunmasına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="6cd92-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="6cd92-125">Kural ve koşulları tanımlamak yöneticileri tarafından el ile kullanıcılar tarafından veya kullanıcılara öneriler burada verilmiştir bir birleşimini kullanarak etiketleri otomatik olarak uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="6cd92-126">Outlook Web, e-postalar için aşağıdaki yerleşik etiketlerini ve kısıtlamaları uygulayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="6cd92-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="6cd92-127">**İletme**: alıcılar bu iletiyi okuyabilir, ancak bunlar iletemez, yazdıramaz, veya içerik kopyalama</span><span class="sxs-lookup"><span data-stu-id="6cd92-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="6cd92-128">**Şifreleme**: iletinin tamamını şifrelenir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="6cd92-129">Alıcılar şifrelenmiş içeriği erişmeden önce kimliklerini onaylamak gerekir ve şifrelemeyi kaldıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="6cd92-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="6cd92-130">**Gizli**: e-posta içeriğini ve eklerini, ancak kuruluşunuzun dışındaki kişilere, kuruluşunuzdaki çalışanların tam izinleri verir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="6cd92-131">Veri sahipleri izleyebilir ve içerik herhangi bir noktada iptal edin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="6cd92-132">**Oldukça gizli**: oldukça gizli verileri görüntülemek, düzenlemek ve Yanıtla, ancak değil iletmek, yazdırmak veya verileri kopyalamak çalışanların izin vererek, bu kısıtlamayı uygulanabilir.</span><span class="sxs-lookup"><span data-stu-id="6cd92-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="6cd92-133">Veri sahipleri izleyebilir ve içerik herhangi bir noktada iptal edin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="6cd92-134">Azure bilgi koruma etkinleştirilmiş olduğundan emin olun</span><span class="sxs-lookup"><span data-stu-id="6cd92-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="6cd92-135">AIP etkinleştirilmiş olduğunu doğrulamak için:</span><span class="sxs-lookup"><span data-stu-id="6cd92-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="6cd92-136">[Azure portal](https://portal.azure.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="6cd92-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="6cd92-137">**Arama kutusu** *Azure bilgi koruma* **tüm hizmetleri** ve türünü seçin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="6cd92-138">Sonuçları görüntüledikten sonra sık yapmak için **Azure bilginin korunması** için İleri ve kolayca bulabilmek için Başlat'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6cd92-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="6cd92-139">**Azure bilgi koruma** seçin \> **korumasını etkinleştirme** ve marka emin durumu ayarlanır için etkinleştirilmiş.</span><span class="sxs-lookup"><span data-stu-id="6cd92-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="6cd92-140">Azure bilgi koruma İlkesi ve varsayılan etiketleri görüntüleme</span><span class="sxs-lookup"><span data-stu-id="6cd92-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="6cd92-141">Görüntülemek ve değiştirmek için varolan etiketleri:</span><span class="sxs-lookup"><span data-stu-id="6cd92-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="6cd92-142">Azure bilgi koruma Panosu üzerinde **sınıflandırmaları** seçin \> **etiketleri**.</span><span class="sxs-lookup"><span data-stu-id="6cd92-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="6cd92-143">![Azure bilginin korunması için standart etiketler.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="6cd92-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="6cd92-144">Tüm etiket seçeneklerini görüntülemek için seçebilirsiniz, ancak değiştirebilirsiniz görünen ad, renkler vb..</span><span class="sxs-lookup"><span data-stu-id="6cd92-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="6cd92-145">Bkz: [Değiştir ve yeni etiketler oluşturmak](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) kendi oluşturmak istiyorsanız.</span><span class="sxs-lookup"><span data-stu-id="6cd92-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="6cd92-146">Azure bilgi koruma İstemcisi'ni el ile yükleme</span><span class="sxs-lookup"><span data-stu-id="6cd92-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="6cd92-147">AIP istemciyi el ile yüklemek için:</span><span class="sxs-lookup"><span data-stu-id="6cd92-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="6cd92-148">**AzInfoProtection.exe** , [Microsoft Yükleme Merkezi'ndeki](https://www.microsoft.com/download/details.aspx?id=53018)karşıdan yükleyin.</span><span class="sxs-lookup"><span data-stu-id="6cd92-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="6cd92-149">Yükleme Word belgesi görüntüleme ve **Koru** seçeneği **Giriş** sekmesinde kullanılabilir durumda olmasını sağlayarak çalışılan doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6cd92-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="6cd92-150">![Koruma sekmesini aşağı açılan bir Word belgesinde.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="6cd92-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="6cd92-151">Daha fazla bilgi için bkz: [İstemci Yükleme](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="6cd92-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
