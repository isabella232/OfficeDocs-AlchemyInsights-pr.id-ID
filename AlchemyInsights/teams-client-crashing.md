---
title: Klien Teams mengalami crash?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030684"
---
# <a name="teams-client-crashing"></a>Klien Teams mengalami crash?

Jika klien Teams Anda mengalami crash, cobalah langkah berikut:

- Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pastikan semua [URL dan rentang alamat Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dapat diakses.

- Masuklah dengan akun admin Anda, lalu periksa [Dasbor Kesehatan Layanan](https://docs.microsoft.com/office365/enterprise/view-service-health) untuk memverifikasi bahwa tidak ada gangguan atau penurunan layanan.

 - Sebagai langkah terakhir, Anda dapat mencoba membersihkan cache klien Teams Anda:

    1.  Keluarlah sepenuhnya dari klien desktop Microsoft Teams. Anda dapat mengklik kanan **Teams** dari Baki Ikon dan mengklik **Tutup**, atau menjalankan Manajer Tugas dan mengakhiri proses sepenuhnya.

    2.  Buka File Explorer, lalu ketik %appdata%\Microsoft\teams.

    3.  Setelah berada di direktori, Anda akan melihat beberapa folder berikut:

         - Dari dalam **Cache Aplikasi**, buka Cache dan hapus file apa pun di lokasi Cache: %appdata%\Microsoft\teams\application cache\cache.

        - Dari dalam **Penyimpanan_blob**, hapus semua file: %appdata%\Microsoft\teams\blob_storage.

        - Dari dalam **Cache**, hapus semua file: %appdata%\Microsoft\teams\Cache.

        - Dari dalam **database**, hapus semua file: %appdata%\Microsoft\teams\databases.

        - Dari dalam **GPUCache**, hapus semua file: %appdata%\Microsoft\teams\GPUcache.

        - Dari dalam **IndexedDB**, hapus file .db: %appdata%\Microsoft\teams\IndexedDB.

        - Dari dalam **Penyimpanan Lokal**, hapus semua file: %appdata%\Microsoft\teams\Local Storage.

        - Terakhir, dari dalam **tmp**, hapus semua file: %appdata%\Microsoft\teams\tmp.

    4. Mulai ulang klien Teams Anda.
