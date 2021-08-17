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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304372"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah berbagi SharePoint dengan pengguna eksternal

Pastikan berbagi eksternal diaktifkan untuk organisasi Anda:
  
1. Masuk ke [halaman &amp; add-in Layanan di pusat admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **Situs.**
    
2. Pastikan pengaturan dinyalakan menjadi "On." Jika "Hanya pengguna eksternal yang sudah ada" yang dipilih, pastikan pengguna eksternal tersebut tercantum di pusat admin Microsoft 365.
    
Pastikan berbagi eksternal telah diaktifkan untuk situs tersebut. Untuk kumpulan situs klasik:
  
1. Di pusat SharePoint admin baru, di panel kiri, klik **situs.**
    
2. Pilih situs atau situs, dan pada pita, klik **Berbagi.**
    
Untuk situs tim yang dimiliki oleh Microsoft 365 tim, atau situs komunikasi:
  
- Tipe situs baru ini memiliki pengaturan berbagi yang sama seperti pengaturan seluruh organisasi Anda, kecuali pengaturan untuk seluruh organisasi memungkinkan berbagi file menggunakan tautan yang tidak memerlukan masuk. Dalam kasus ini, situs memungkinkan berbagi dengan pengguna eksternal baru dan yang sudah ada yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan pusat admin SharePoint atau PowerShell. [Pelajari selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Catatan:** Pengaturan berbagi eksternal untuk situs apa pun dapat menjadi lebih terbatas daripada pengaturan untuk seluruh organisasi Anda, tetapi tidak lebih sesuai dengan pengaturan untuk seluruh organisasi. 
  

