---
title: Alat ekspor eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277930"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Tidak dapat menginstal atau menjalankan alat ekspor eDiscovery?

Jika Anda tidak dapat menginstal atau menjalankan alat ekspor eDiscovery untuk mengunduh hasil pencarian, periksa hal-hal berikut ini:
  
- Komputer yang Anda gunakan memenuhi prasyarat ini:

  - 32-atau 64-bit versi Windows 7 dan versi yang lebih baru

  - Microsoft .NET Framework 4.7

  - Browser yang didukung:

  - Microsoft Edge

    Atau

  - Internet Explorer 10 dan versi yang lebih baru

    Browser lain, seperti Google Chrome dan Mozilla Firefox tidak didukung.

- Organisasi Anda dapat menyambungkan ke titik akhir di Azure, yaitu ** \* . Blob.Core.Windows.net** (wildcard mewakili pengidentifikasi unik untuk pekerjaan ekspor Anda).

- Anda diberi peran ekspor di pusat kepatuhan keamanan Microsoft 365 &amp; . Secara default, peran ini hanya ditetapkan ke grup peran Manajer eDiscovery. Lihat [menetapkan izin eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Untuk informasi selengkapnya, lihat [mengekspor hasil pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Jika Anda mengekspor lebih dari 100K kotak surat, Anda perlu menggunakan PowerShell berikut untuk mengunduh hasil ekspor:  [mengekspor hasil dari kotak surat lebih dari 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).