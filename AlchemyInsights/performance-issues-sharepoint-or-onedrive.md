---
title: Masalah kinerja-SharePoint atau OneDrive
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771904"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna

SharePoint atau OneDrive mungkin lambat, tidak dapat diakses, atau tidak tersedia, atau mungkin menampilkan kesalahan layanan yang tidak tersedia atau 503, karena beberapa alasan:
  
- Jika situs SharePoint atau OneDrive Anda lambat atau tertunda untuk beberapa pengguna, mungkin ada masalah layanan sementara ketika pengguna mengalami keterlambatan atau kesalahan navigasi saat mengakses situs SharePoint atau konten OneDrive. Lihat [dasbor Kesehatan Layanan](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.
  
- Pengguna mungkin menerima *server 503 adalah kesalahan sibuk* ketika mencoba menavigasi ke situs SharePoint atau OneDrive. Kesalahan ini bisa disebabkan oleh pembatasan dalam Layanan SharePoint. SharePoint Online menerapkan pembatasan untuk mempertahankan kinerja yang optimal dan keandalan layanan SharePoint Online. Pembatasan membatasi jumlah tindakan pengguna atau panggilan serentak (berdasarkan skrip atau kode) untuk mencegah penggunaan sumber daya secara berlebihan. Untuk informasi selengkapnya tentang pembatasan, [Hindari mendapatkan pembatasan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Jika Anda mengalami kinerja yang lambat dengan situs atau halaman SharePoint **klasik** atau **modern** , gunakan [alat diagnostik halaman](https://aka.ms/perftool) untuk menganalisis halaman.
  
- Jika Anda masih mengalami kinerja yang lambat umum, silakan Tinjau sumber daya di bagian bawah artikel ini: [pengenalan ke tuning kinerja untuk SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  