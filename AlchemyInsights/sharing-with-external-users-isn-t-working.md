---
title: Berbagi dengan pengguna eksternal tidak berfungsi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691578"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah berbagi konten SharePoint dengan pengguna eksternal

Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:
  
1. Masuk ke [ &amp; Halaman Add-in Services di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.
    
2. Pastikan pengaturan beralih ke "aktif." Jika "hanya pengguna eksternal yang sudah ada" yang dipilih, pastikan pengguna eksternal dicantumkan di pusat admin Microsoft 365.
    
Pastikan berbagi eksternal diaktifkan untuk situs tersebut. Untuk kumpulan situs klasik:
  
1. Di pusat admin SharePoint baru, di panel kiri, klik **situs**.
    
2. Pilih situs atau situs, dan pada pita, klik **berbagi**.
    
Untuk situs tim yang termasuk dalam grup Microsoft 365, atau situs komunikasi:
  
- Tipe situs baru ini memiliki pengaturan berbagi yang sama seperti pengaturan seluruh organisasi Anda, kecuali pengaturan di seluruh organisasi memungkinkan berbagi file menggunakan link yang tidak memerlukan masuk. Dalam kasus ini, situs memperbolehkan berbagi dengan pengguna eksternal baru dan yang sudah ada yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan Pusat admin SharePoint atau PowerShell yang baru. [Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Pengaturan berbagi eksternal untuk setiap situs dapat lebih ketat daripada pengaturan seluruh organisasi Anda, tetapi tidak lebih permisif dari pengaturan seluruh organisasi. 
  

