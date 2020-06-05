---
title: Berbagi dengan pengguna eksternal tidak berfungsi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582778"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah saat berbagi konten SharePoint dengan pengguna eksternal

Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:
  
1. Buka [ &amp; Halaman Add-in layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.
    
2. Pastikan setelan diubah menjadi "aktif". Jika "hanya ada pengguna eksternal" dipilih, pastikan pengguna eksternal tercantum di pusat admin Microsoft 365.
    
Pastikan berbagi eksternal diaktifkan untuk situs. Untuk koleksi situs klasik:
  
1. Di pusat admin SharePoint baru, di sebelah kiri, klik **situs**.
    
2. Pilih situs atau situs, dan pada pita, klik **berbagi**.
    
Untuk situs tim milik Grup 365 Microsoft, atau situs komunikasi:
  
- Jenis situs baru ini memiliki setelan berbagi yang sama dengan setelan di seluruh organisasi, kecuali jika setelan di seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk. Dalam hal ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang ada yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan Pusat admin SharePoint baru atau PowerShell. [Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Setelan berbagi eksternal untuk situs mana pun dapat lebih ketat daripada setelan di seluruh organisasi, tetapi tidak lebih permisif daripada setelan di seluruh organisasi. 
  

