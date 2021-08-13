---
title: Memantau Akses Kondisional
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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975104"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Memantau Akses Kondisional untuk Exchange

Pengguna yang mendapatkan akses kondisional akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:

- Jika perangkat terdaftar, sarankan pengguna untuk masuk ke aplikasi Company Portal dan pastikan bahwa perangkat muncul di Company Portal. Jika tidak ada, pengguna harus mendaftarkan perangkat tersebut.
- Di portal Azure, masuk ke Intune > Kepatuhan perangkat. Di bawah Monitor, klik Kepatuhan perangkat. Lihat laporan kepatuhan perangkat untuk memastikan bahwa perangkat pengguna telah ditandai sebagai memenuhi syarat.
- Di portal Azure, masuk ke Intune > Kepatuhan perangkat. Di bawah Kelola, klik Kebijakan. Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil telah ditetapkan ke perangkat pengguna Anda. Jika belum ditetapkan, Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.
- Edit penetapan akses kondisional pengguna.

1. Di portal Azure, masuk ke **Kebijakan akses**  >  **kondisional** Intune  >  .
2. Pilih kebijakan dari daftar.
3. Klik Pengguna dan grup.
4. Untuk menargetkan kebijakan tertentu kepada seseorang, tambahkan orang tersebut ke dalam daftar Sertakan. Untuk memastikan bahwa seseorang tidak termasuk dalam kebijakan, tambahkan orang tersebut ke dalam daftar Pengecualian.

Tautan yang berguna:

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Memecahkan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Memantau kepatuhan perangkat Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Catatan: langkah-langkah ini hanya membantu dalam memecahkan Azure Active Directory Akses Bersyarat. Juga dimungkinkan untuk melakukan karantina perangkat yang memblokir akses email dengan Exchange email. Informasi selengkapnya tentang Exchange manajemen perangkat dapat ditemukan [di sini]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
