---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068408"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna

SharePoint atau OneDrive mungkin lambat, tidak dapat diakses, atau tidak tersedia, atau mungkin menampilkan layanan tidak tersedia atau 503 kesalahan, karena beberapa alasan:
  
- Jika situs SharePoint atau OneDrive lambat atau tertunda untuk beberapa pengguna, mungkin ada masalah layanan sementara di mana pengguna mengalami penundaan terputus-putus atau galat navigasi ketika mengakses situs SharePoint atau konten OneDrive. Periksa [dasbor Kesehatan Layanan](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.
  
- Pengguna akan menerima *503 server sibuk* galat saat berusaha menavigasi ke situs SharePoint atau OneDrive. Galat ini dapat disebabkan oleh pelambatan dalam Layanan SharePoint. SharePoint Online menggunakan pelambatan untuk mempertahankan kinerja optimal dan keandalan Layanan SharePoint online. Pelambatan membatasi jumlah tindakan pengguna atau panggilan bersamaan (dengan skrip atau kode) untuk mencegah penggunaan sumber daya berlebihan. Untuk informasi lebih lanjut tentang pelambatan Lihat, [Hindari mendapatkan mengalami kelambatan atau diblokir di SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Jika Anda mengalami kinerja yang lambat dengan situs atau halaman SharePoint **klasik** atau **modern** , gunakan [alat diagnostik halaman](https://aka.ms/perftool) untuk menganalisis halaman.
  
- Jika Anda masih mengalami kinerja lambat umum, Tinjau sumber daya di bagian bawah artikel ini: [pengantar tuning kinerja untuk SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  