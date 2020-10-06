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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366431"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Memantau akses bersyarat untuk Exchange

Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:

- Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
- Di portal Azure, masuk ke Intune > kepatuhan perangkat. Di bawah monitor klik kepatuhan perangkat. Tampilkan Laporan kepatuhan perangkat Anda untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai.
- Di portal Azure, masuk ke Intune > kepatuhan perangkat. Di bawah Kelola, klik kebijakan. Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda. Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.
- Mengedit penetapan akses bersyarat pengguna.

1. Di portal Azure, masuk ke **Intune**  >  **kebijakan akses bersyarat**Intune  >  **Policies**.
2. Pilih kebijakan dari daftar.
3. Klik pengguna dan grup.
4. Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke daftar sertakan. Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke daftar Kecualikan.

Link yang berguna:

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoring Intune Device Compliance](https://docs.microsoft.com/intune/compliance-policy-monitor)

Catatan: langkah-langkah ini hanya membantu dalam pemecahan masalah akses bersyarat fitur direktori aktif Azure. Memungkinkan untuk mengkarantina perangkat yang memblokir akses email itu dengan kebijakan Exchange. Informasi selengkapnya tentang manajemen perangkat Exchange bisa ditemukan [di sini](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
