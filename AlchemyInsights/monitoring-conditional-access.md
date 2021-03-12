---
title: Memantau akses bersyarat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708677"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Memantau akses bersyarat untuk Exchange

Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:

- Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
- Di portal Azure, masuk ke Intune > kepatuhan perangkat. Di bawah monitor klik kepatuhan perangkat. Tampilkan Laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai.
- Di portal Azure, masuk ke Intune > kepatuhan perangkat. Di bawah Kelola, klik kebijakan. Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda. Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.
- Mengedit penetapan akses bersyarat pengguna.

1. Di portal Azure, masuk ke   >  **kebijakan akses bersyarat** Intune  >  .
2. Pilih kebijakan dari daftar.
3. Klik pengguna dan grup.
4. Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke daftar sertakan. Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke daftar Kecualikan.

Link yang berguna:

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoring Intune Device Compliance](https://docs.microsoft.com/intune/compliance-policy-monitor)

Catatan: langkah-langkah ini hanya membantu dalam pemecahan masalah akses bersyarat fitur direktori aktif Azure. Memungkinkan untuk mengkarantina perangkat yang memblokir akses email itu dengan kebijakan Exchange. Informasi selengkapnya tentang manajemen perangkat Exchange bisa ditemukan [di sini] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
