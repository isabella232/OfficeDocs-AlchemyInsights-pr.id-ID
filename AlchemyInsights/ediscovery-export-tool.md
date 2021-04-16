---
title: Alat ekspor eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814591"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery?

Jika tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery untuk mengunduh hasil pencarian, periksa hal-hal berikut:
  
- Komputer yang Anda gunakan memenuhi prasyarat berikut:

  - Windows 7 versi 32- atau 64-bit dan versi yang lebih baru

  - Microsoft .NET Framework 4.7

  - Browser yang didukung:

  - Microsoft Edge

    Atau

  - Internet Explorer 10 dan versi yang lebih baru

    Browser lain, seperti Google Chrome dan Mozilla Firefox tidak didukung.

- Organisasi Anda dapat tersambung ke titik akhir di Azure, yaitu **\* .blob.core.windows.net** (wildcard mewakili pengidentifikasi unik untuk pekerjaan ekspor Anda).

- Anda mendapatkan peran Ekspor di Pusat Kepatuhan Keamanan Microsoft 365. &amp; Secara default, peran ini hanya ditetapkan pada grup peran Manajer eDiscovery. Lihat [Menetapkan izin eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Untuk informasi selengkapnya, lihat [Mengekspor hasil Pencarian Konten.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Jika mengekspor lebih dari 100 kotak surat, Anda perlu menggunakan Powershell berikut untuk mengunduh hasil Ekspor: Mengekspor hasil dari lebih dari  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)kotak surat .