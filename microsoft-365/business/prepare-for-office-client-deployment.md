---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: 32 bit Office uygulamalarını Windows 10 bilgisayarlara otomatik olarak nasıl yükleyip güncel tutacağınızı öğrenin.
ms.openlocfilehash: fe1f946e4a216050e533604afa7c6e74e7b5980f
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288405"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı

Microsoft 365 İş kullanarak Windows 10 bilgisayarlarına 32 bit Office uygulamalarını otomatik olarak yükleyebilir ve güncelleştirmelerle bunların güncelliğini koruyabilirsiniz.
  
Bundan en iyi sonucu elde etmek için kullanıcının bilgisayarı Windows 10 Business çalıştırılıyor olmalı ve şu koşulları sağlamalıdır:
  
- Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.
    
    veya
    
- Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.
    
Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin. Aşağıdaki şekilde gösterildiği gibi Office Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılmıştır. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Bu özelliğe sahip olmak kimlerin işine yarar**
  
Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:
  
- Windows 10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update **bulunur** ve Azure Active Directory'ye katılmıştır. 
    
- 64 bit Office paketi **yoktur** (örneğin: Word, Excel, Powerpoint). 64 bit Office uygulamaları gerekiyorsa, bu özellik uygun değildir. Microsoft 365 İş yönetim konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği sağlanmaz. 
    
- Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**. Microsoft 365 İş, Office'i Office 2016 Tıkla-Çalıştır sürümüne yükseltir ve bu da Office 2016 MSI tek başına uygulamalarıyla çalışmaz. 
    
Aşağıdaki tabloda, son kullanıcıların/yöneticilerin, işleme başladıkları noktaya bağlı olarak Microsoft 365 İş yönetim merkezinden Office'in 32 bit Tıkla-Çalıştır sürümünün dağıtımını başarıyla tamamlaması için gerçekleştirmesi gereken işlemlerin ayrıntılarını bulabilirsiniz.
  
|**Başlangıçtaki Office yükleme durumu**|**Microsoft 365 İş Office yüklemesinden önce yapılması gereken işlem**|**Son durum**|
|:-----|:-----|:-----|
|Hiçbir Office paketi yüklü değil  <br/> |Yok  <br/> |Tıkla-çalıştır kullanılarak Office 2016 32 bit yüklenir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok  <br/> |Yok  <br/> |Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\*** <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 veya 64 bit tek başına Office uygulamaları (örneğin, Visio ve Project) var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> ||||
|Office'in Tıkla-Çalıştır 64 bit sürümü var  <br/> |64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmek sorun yaratmayacaksa, 64 bit uygulamalarını kaldırın  <br/> |Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir  <br/> |
|Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var  <br/> |MSI Office 2016'yı kaldırın.  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz  <br/> |
|Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var  <br/> |Yok  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır  <br/> |
||||
   
 **(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez. Düzeltme için çalışmalar devam etmektedir. 
  


