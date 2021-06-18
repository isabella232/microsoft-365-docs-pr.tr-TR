---
title: Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Windows 10 bilgisayarlarına 32 bit Office uygulamalarını otomatik olarak yükleme ve bunları güncelleştirme hakkında bilgi edinin.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924237"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Microsoft 365 İş tarafından Office istemci dağıtımı hazırlığı

Bu makale Microsoft 365 İş Ekstra için geçerlidir.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı

32 bit Office uygulamalarını Windows 10 bilgisayarlara otomatik olarak yüklemek ve güncelleştirmelerle güncel tutmak için Microsoft 365 İş Ekstra'ya kullanabilirsiniz.
  
Otomatik yükleme en iyi şekilde, son kullanıcının bilgisayarı Windows 10 Business'da ise ve:
  
- Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.
    
    veya
    
- Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.
    
Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin. Aşağıdaki şekilde **gösterildiği gibi Office** Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılır. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Bu özele sahip olmak kimlerin avantajlarına sahip olacak?**
  
Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:
  
- **Windows**  10 Business kullanıcı lisansı, etkin bir Microsoft 365 İş lisansı, Windows 10 Creators Update vardır ve Azure Active Directory'ye katılmış durumdadır. 
    
- **64** bit Office uygulamaları (örneğin: Word, Excel, PowerPoint) yok. 64 bit Office uygulamaları gerekli ise, bu özellik uygun değildir çünkü microsoft 365 İş yönetici konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği yoktur. 
    
- Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**. Microsoft 365 İş, Office'i Office 2016'nın Tıkla-Çalıştır sürümüne yükselter ve bu da Office 2016 MSI tek başına uygulamalarıyla işe yaramadı. 
    
Aşağıdaki tabloda, son kullanıcıların/yöneticilerin, başlangıç durumlarına bağlı olarak, işletmeler için Microsoft 365 yönetici konsolundan Office'in 32 bit Tıkla-Çalıştır sürümünün dağıtımını başarılı bir şekilde yapmak için hangi eylemi uygulaması gerekten olduğu görüntülenir.<br/>


|Başlangıçtaki Office yükleme durumu|Microsoft 365 İş Office'i yüklemeden önce at gereken eylem|Son durum|
|:-----|:-----|:-----|
|Hiçbir Office paketi yüklü değil  <br/> |Yok  <br/> |Tıkla-Çalıştır kullanılarak Office 2016 32 bit yüklenir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok  <br/> |Yok  <br/> |Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\*** <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit tek başına Office uygulamaları (örneğin, Visio, Project) var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> |
|Office'in Tıkla-Çalıştır 64 bit sürümü var  <br/> |64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmek sorun yoksa bunları kaldırın  <br/> |Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir  <br/> |
|Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var  <br/> |MSI Office 2016'yı kaldırın.  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz  <br/> |
|Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var  <br/> |Yok  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır  <br/> |
||||
   
 **(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez. Düzeltme için çalışma devam etmektedir. 
  
