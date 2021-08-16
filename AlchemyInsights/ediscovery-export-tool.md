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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101305"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery?

Jika tidak dapat menginstal atau menjalankan Alat Ekspor eDiscovery untuk mengunduh hasil pencarian, periksa hal-hal berikut:
  
- Komputer yang Anda gunakan memenuhi prasyarat berikut:

  - Versi 32 bit atau 64 bit Windows 7 dan yang lebih baru

  - Microsoft .NET Framework 4.7

  - Browser yang didukung:

  - Microsoft Edge

    Atau

  - Internet Explorer 10 dan versi yang lebih baru

    Browser lain, seperti Google Chrome dan Mozilla Firefox tidak didukung.

- Organisasi Anda dapat tersambung ke titik akhir di Azure, yaitu **\* .blob.core.windows.net** (wildcard mewakili pengidentifikasi unik untuk pekerjaan ekspor Anda).

- Anda mendapatkan peran Ekspor di Pusat Microsoft 365 &amp; Keamanan Keamanan. Secara default, peran ini hanya ditetapkan pada grup peran Manajer eDiscovery. Lihat [Menetapkan izin eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Untuk informasi selengkapnya, lihat [Mengekspor hasil Pencarian Konten.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Jika mengekspor lebih dari 100 kotak surat, Anda perlu menggunakan Powershell berikut untuk mengunduh hasil Ekspor: Mengekspor hasil dari lebih dari  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)kotak surat .