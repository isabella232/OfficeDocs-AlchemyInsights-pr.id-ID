---
title: 1490-pemecahan masalah-eDiscovery-kegagalan
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277829"
---
# <a name="troubleshoot-content-search-errors"></a>Memecahkan masalah kesalahan pencarian konten

Apakah Anda mengalami masalah dengan pencarian konten atau mendapatkan kegagalan ketika mengekspor hasil pencarian?

Misalnya, Apakah Anda menerima hal berikut ini saat menjalankan pencarian?

- Kesalahan CS008 atau CS012

- Kesalahan sibuk/waktu habis server

- Terjadi galat aplikasi

Atau saat mencari atau mengekspor hasil dari sejumlah besar kotak surat (lebih dari 100.000 kotak surat), Apakah Anda mendapatkan kesalahan ekspor?

Untuk tipe kesalahan ini, coba Cari lokasi konten yang gagal. Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.

Jika Anda mengekspor lebih dari 100K kotak surat, Anda perlu menggunakan PowerShell berikut untuk mengunduh hasil ekspor:  [mengekspor hasil dari kotak surat lebih dari 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
