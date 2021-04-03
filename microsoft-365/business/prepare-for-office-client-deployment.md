---
title: Microsoft 365 İş tarafından Office istemci dağıtımına hazırlanma
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
description: Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yükleme ve bunları güncelleştirme hakkında bilgi edinin.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580064"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Microsoft 365 İş tarafından Office istemci dağıtımına hazırlanma

Bu makale Microsoft 365 İş Ekstra için geçerlidir.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>İstemci bilgisayarlara Office uygulamalarını otomatik olarak yükleme hazırlığı

Windows 10 bilgisayarlara 32 bit Office uygulamalarını otomatik olarak yüklemek ve güncelleştirmelerle güncel tutmak için Microsoft 365 İş Ekstra'ya kullanabilirsiniz.
  
Otomatik yükleme en iyi şekilde çalışır; son kullanıcının bilgisayarı Windows 10 İş'tedir ve:
  
- Mevcut Office masaüstü uygulamaları (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access ve OneDrive) bulunmamalıdır.
    
    veya
    
- Office'in Tıkla-Çalıştır sürümü yüklü olmalıdır.
    
Office'in Tıkla-Çalıştır sürümüne sahip olup olmadığınızı belirlemek için, herhangi bir Office uygulamasında **Dosya** \> **Hesap**'a (Outlook'ta **Office Hesabı**) gidin. Aşağıdaki şekilde **gösterildiği gibi Office** Güncelleştirmeleri görüyorsanız, yükleme Tıkla-Çalıştır kullanılarak yapılır. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Bu özelliden yararlananlar**
  
Bilgisayarı aşağıdaki özelliklere sahip olan son kullanıcılar:
  
- **Windows**  10 Business kullanıcı lisansına, etkin bir iş için Microsoft 365 lisansına, Windows 10 Creators Update'e sahiptir ve Azure Active Directory'ye katılmış durumdadır. 
    
- **64** bit Office uygulamaları (örneğin: Word, Excel, PowerPoint) yok. 64 bit Office uygulamaları gerekli ise bu özellik uygun değildir, çünkü işletmeler için Microsoft 365 yönetici konsolundan Office'in 64 bit 2016 Tıkla-Çalıştır sürümünü tetikleme desteği yoktur. 
    
- Herhangi bir 2016 Windows Installer (MSI) tek başına uygulaması (örneğin, Visio veya Project) **yoktur**. Microsoft 365 İş, Office'i Office 2016'nın Tıkla-Çalıştır sürümüne yükselter ve bu da Office 2016 MSI tek başına uygulamalarıyla işe yaramadı. 
    
Aşağıdaki tablo, iş için Microsoft 365 yönetici konsolundan Office'in 32 bit Tıkla-Çalıştır sürümünün başarılı bir şekilde dağıtımını yapmak için, son kullanıcıların/yöneticilerin başlangıç durumlarına bağlı olarak hangi eylemi uygulaması gerekten olduğunu gösterir.
  
|**Başlangıçtaki Office yükleme durumu**|**Microsoft 365 İş Office yüklemesi öncesinde 2010'da 2010'da 2013'e kadar devam etmek için gereken işlem**|**Son durum**|
|:-----|:-----|:-----|
|Hiçbir Office paketi yüklü değil  <br/> |Yok  <br/> |Office 2016 32 bit, Tıkla-Çalıştır kullanılarak yüklenir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü (2016 veya önceki) var ve tek başına uygulama yok  <br/> |Yok  <br/> |Gerektiği gibi Office 2016'nın en son 32 bit Tıkla-Çalıştır sürümüne yükseltilir **\*** <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve Tıkla-Çalıştır 32 bit veya 64 bit tek başına Office uygulamaları (örneğin, Visio, Project) var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> |
|Office'in Tıkla-Çalıştır 32 bit sürümü ve 32 bit veya 64 bit (2016 dışında) MSI tek başına Office uygulamaları var  <br/> |Yok  <br/> |Tek başına uygulamalar etkilenmez. Paket, Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilir  <br/> ||||
|Office'in Tıkla-Çalıştır 64 bit sürümü var  <br/> |64 bit Office uygulamalarını 32 bit Office uygulamalarıyla değiştirmeniz sorun yoksa kaldırın  <br/> |Office 64 bit uygulamaları kaldırılmışsa, Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir  <br/> |
|Tek başına uygulamalarla veya bu uygulamalar olmadan Office 2016'nın MSI yüklemesi var  <br/> |MSI Office 2016'yı kaldırın.  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü yüklenir. Tek başına uygulamalarda hiçbir değişiklik olmaz  <br/> |
|Office 2013'ün (veya önceki sürümlerin) ve/veya tek başına Office uygulamalarının MSI yüklemesi var  <br/> |Yok  <br/> |Office 2016'nın Tıkla-Çalıştır 32 bit sürümü, önceden var olan MSI Office yüklemesiyle (ve tek başına uygulamalarla) birlikte kullanılır  <br/> |
||||
   
 **(\*) Not:** Bilinen bir hata nedeniyle Office 2016'nın Tıkla-Çalıştır 32 bit sürümüne yükseltilmez. Bir düzeltme devam ediyor. 
  
