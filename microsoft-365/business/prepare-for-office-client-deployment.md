---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak nasıl yükleyip güncel tutacağınızı öğrenin.
ms.openlocfilehash: 0f8cd7df49ad627b190fad6737ec95a6d64d99d0
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065126"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı

Microsoft 365 Business'ı kullanarak Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yükleyebilir ve güncelleştirmelerle güncel tutabilirsiniz.
  
Son kullanıcının bilgisayarı Windows 10 Business'taysa otomatik yükleme en iyi şekilde çalışır ve:
  
- Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.
    
    veya
    
- Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.
    
Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin. **Office Güncelleştirmeleri'ni** aşağıdaki şekilde gösterildiği gibi görürseniz, yükleme Tıkla-Çalıştır kullanılarak yapılmıştır. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Bu özelliğe sahip olmaktan kimler yararlanır?**
  
Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:
  
- Windows 10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update **bulunur** ve Azure Active Directory'ye katılmıştır. 
    
- 64 bit Office uygulamaları **yok** (örnek: Word, Excel, PowerPoint). 64 bit Office uygulamaları gerekiyorsa, Microsoft 365 Business yönetici konsolundan Office'in 64 bit 2016 Tıkla çalıştır sürümünü tetiklemek için destek olmadığından bu özellik uygun değildir. 
    
- Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**. Microsoft 365 Business, Office 2016'nın Tıkla Çalıştır sürümüne Office'i yükseltir ve bu office 2016 MSI bağımsız uygulamalarıyla çalışmaz. 
    
Aşağıdaki tablo, Microsoft 365 Business yönetici konsolundan Office dağıtımının 32 bit'lik başarılı bir Tıklamayla Çalıştır sürümüne sahip olmak için, başlangıç durumlarına bağlı olarak son kullanıcıların/yöneticilerin hangi eylemi üstlenmeleri gerekebileceğini gösterir.
  
|**Başlangıçtaki Office yükleme durumu**|**Microsoft 365 İş Office yüklemesinden önce yapılması gereken işlem**|**Son durum**|
|:-----|:-----|:-----|
|Hiçbir Office paketi yüklü değil  <br/> |Yok  <br/> |Office 2016 32 bit Tıkla çalıştır kullanılarak yüklenir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok  <br/> |Yok  <br/> |Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\*** <br/> |
|Office'in 32 bit'lik mevcut Click-to-Run sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit bağımsız Office uygulamaları (örneğin, Visio, Project)  <br/> |Yok  <br/> |Bağımsız uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var  <br/> |Yok  <br/> |Bağımsız uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> ||||
|Office'in Tıkla-Çalıştır 64 bit sürümü var  <br/> |64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmenin sakıncası yoksa, kaldırın  <br/> |Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir  <br/> |
|Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var  <br/> |MSI Office 2016'yı kaldırın.  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz  <br/> |
|Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var  <br/> |Yok  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır  <br/> |
||||
   
 **(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez. Bir düzeltme devam ediyor. 
  
