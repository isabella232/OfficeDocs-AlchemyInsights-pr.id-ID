---
title: 1490-troubleshooting-eDiscovery-failures
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
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105571"
---
# <a name="troubleshoot-content-search-errors"></a>Memecahkan masalah kesalahan Pencarian Konten

Apakah Anda mengalami masalah dengan Pencarian Konten atau mengalami kegagalan saat mengekspor hasil pencarian?

Misalnya, apakah Anda menerima hal berikut saat menjalankan pencarian?

- Kesalahan CS008 atau CS012

- Kesalahan sibuk/waktu habis server

- Terjadi kesalahan aplikasi

Atau, saat mencari atau mengekspor hasil dari sejumlah besar kotak surat (lebih dari 100.000 kotak surat), apakah Anda mendapatkan kesalahan ekspor?

Untuk jenis kesalahan ini, coba lagi pencarian untuk lokasi konten yang telah gagal. Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.

Jika mengekspor lebih dari 100 kotak surat, Anda perlu menggunakan Powershell berikut untuk mengunduh hasil Ekspor: Mengekspor hasil dari lebih dari  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)kotak surat .
