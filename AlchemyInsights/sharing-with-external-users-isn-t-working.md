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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900875"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Memperbaiki masalah yang berbagi konten SharePoint dengan pengguna eksternal

Pastikan eksternal berbagi dihidupkan untuk organisasi Anda:
  
1. Pergi ke [Layanan &amp; halaman add-in di Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), dan klik **situs**.
    
2. Pastikan pengaturan diaktifkan "On." Jika "Hanya pengguna eksternal yang ada" dipilih, pastikan pengguna eksternal terdaftar di Office 365 admin center.
    
Pastikan eksternal berbagi dihidupkan untuk situs. Untuk koleksi klasik situs:
  
1. Di klasik SharePoint admin center, dalam pane kiri, klik **situs koleksi**.
    
2. Pilih situs atau situs, dan pada pita, klik **berbagi**.
    
Untuk situs tim milik Grup Office 365, atau situs komunikasi:
  
- Jenis situs ini baru memiliki pengaturan berbagi sama sebagai pengaturan seluruh organisasi Anda, kecuali jika pengaturan di seluruh organisasi yang memungkinkan berbagi file menggunakan link yang tidak memerlukan masuk. Dalam kasus ini, situs yang memungkinkan berbagi dengan baru dan yang ada pengguna eksternal yang masuk. Untuk mengubah pengaturan untuk situs tertentu, gunakan baru SharePoint admin center (pratinjau) atau PowerShell. [Selengkapnya](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Pengaturan berbagi eksternal untuk setiap situs dapat lebih ketat daripada pengaturan seluruh organisasi Anda, tetapi tidak lebih permisif dari pengaturan di seluruh organisasi. 
  

