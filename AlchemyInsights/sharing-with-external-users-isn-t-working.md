---
title: Berbagi dengan pengguna eksternal tidak bekerja
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502234"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah yang berbagi konten SharePoint dengan pengguna eksternal

Pastikan eksternal berbagi dihidupkan untuk organisasi Anda:
  
1. Pergi ke [Layanan &amp; halaman add-in di Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.
    
2. Pastikan pengaturan diaktifkan "On." Jika "Hanya pengguna eksternal yang ada" dipilih, pastikan pengguna eksternal terdaftar di Microsoft 365 admin center.
    
Pastikan eksternal berbagi dihidupkan untuk situs. Untuk koleksi klasik situs:
  
1. Di SharePoint admin center baru, dalam pane kiri, klik **situs**.
    
2. Pilih situs atau situs, dan pada pita, klik **berbagi**.
    
Untuk situs tim milik Grup Office 365, atau situs komunikasi:
  
- Jenis situs ini baru memiliki pengaturan berbagi sama sebagai pengaturan seluruh organisasi Anda, kecuali jika pengaturan di seluruh organisasi yang memungkinkan berbagi file menggunakan link yang tidak memerlukan masuk. Dalam kasus ini, situs yang memungkinkan berbagi dengan baru dan yang ada pengguna eksternal yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan baru SharePoint admin center atau PowerShell. [Selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Pengaturan berbagi eksternal untuk setiap situs dapat lebih ketat daripada pengaturan seluruh organisasi Anda, tetapi tidak lebih permisif dari pengaturan di seluruh organisasi. 
  

