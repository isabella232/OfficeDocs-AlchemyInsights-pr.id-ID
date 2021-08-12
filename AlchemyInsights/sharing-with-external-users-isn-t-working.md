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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910369"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah berbagi SharePoint konten dengan pengguna eksternal

Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:
  
1. Masuk ke [halaman &amp; add-in Layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **Situs.**
    
2. Pastikan pengaturan diaktifkan ke "On." Jika "Hanya pengguna eksternal yang sudah ada" yang dipilih, pastikan pengguna eksternal tersebut tercantum di pusat admin Microsoft 365.
    
Pastikan berbagi eksternal telah diaktifkan untuk situs tersebut. Untuk kumpulan situs klasik:
  
1. Di pusat SharePoint admin baru, di panel kiri, klik **situs.**
    
2. Pilih situs atau situs, dan pada pita, klik **Berbagi.**
    
Untuk situs tim milik grup Microsoft 365, atau situs komunikasi:
  
- Tipe situs baru ini memiliki pengaturan berbagi yang sama seperti pengaturan seluruh organisasi Anda, kecuali pengaturan untuk seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk. Dalam kasus ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang sudah ada yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan pusat admin SharePoint atau PowerShell baru. [Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Pengaturan berbagi eksternal untuk situs apa pun dapat menjadi lebih terbatas daripada pengaturan untuk seluruh organisasi Anda, tetapi tidak lebih bebas dari pengaturan untuk seluruh organisasi. 
  

