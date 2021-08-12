---
title: Masalah kinerja yang SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911845"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna

SharePoint atau OneDrive mungkin lambat, tidak dapat diakses, atau tidak tersedia, atau mungkin menampilkan kesalahan layanan yang tidak tersedia atau 503, karena beberapa alasan:
  
- Jika proses SharePoint atau OneDrive Anda lambat atau tertunda untuk beberapa pengguna, mungkin terdapat masalah layanan sementara ketika pengguna mengalami penundaan yang sering terjadi atau kesalahan navigasi saat mengakses situs SharePoint atau OneDrive eksternal. Periksa dasbor [Kesehatan layanan untuk](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) melihat apakah organisasi Anda terkena dampak.
  
- Pengguna mungkin menerima kesalahan *server 503* sibuk ketika mencoba menavigasi ke situs SharePoint atau OneDrive lain. Kesalahan ini bisa disebabkan oleh pembatasan dalam layanan SharePoint ini. SharePoint Online menerapkan pembatasan untuk mempertahankan kinerja yang optimal dan keandalan layanan SharePoint Online. Pembatasan membatasi jumlah tindakan pengguna atau panggilan serentak (berdasarkan skrip atau kode) untuk mencegah penggunaan sumber daya secara berlebihan. Untuk informasi selengkapnya tentang pembatasan, lihat, Menghindari pembatasan atau [pemblokiran di](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)SharePoint Online.

- Jika anda mengalami kinerja yang lambat dengan **situs** **atau** halaman SharePoint modern atau klasik, manfaatkan alat Diagnostik [Halaman](https://aka.ms/perftool) untuk menganalisis halaman.
  
- Jika Anda masih mengalami kinerja lambat umum, silakan tinjau sumber daya di bagian bawah artikel ini: Pengenalan pada [penyetelan kinerja untuk SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  