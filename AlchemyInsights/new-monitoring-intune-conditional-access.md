---
title: Memantau akses bersyarat Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427921"
---
# <a name="monitor-intune-conditional-access"></a>Memantau akses bersyarat Intune

Pengguna yang ditargetkan dengan akses bersyarat akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:

1. Jika perangkat dianggap terdaftar, Anjurkan pengguna untuk masuk ke aplikasi portal perusahaan dan memverifikasi bahwa perangkat tersebut muncul di portal perusahaan. Jika tidak, pengguna harus mendaftarkan perangkat.
1. Di portal Azure, masuk ke **Intune**  >  **Device Compliance**. 
1. Untuk menampilkan laporan kepatuhan perangkat untuk memverifikasi bahwa perangkat pengguna ditandai sebagai sesuai, di bawah **monitor**, klik **kepatuhan perangkat**.
1. Di portal Azure, masuk ke **Intune**  >  **Device Compliance**. Di bawah **Kelola,** klik **kebijakan**. Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil ditetapkan untuk perangkat pengguna Anda. Jika tidak ada profil yang ditetapkan, maka Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.
1. Mengedit penetapan akses bersyarat pengguna.
1. Di portal Azure, navigasikan ke   >  **kebijakan akses bersyarat** Intune  >  , pilih kebijakan dari daftar, dan klik **pengguna dan grup**.
1. Untuk menargetkan kebijakan tertentu pada seseorang, tambahkan ke **Daftar sertakan**. Untuk memastikan bahwa seseorang dihilangkan dari kebijakan, tambahkan ke **Daftar Kecualikan**.

**Link yang berguna:**

- [Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Kebijakan pemecahan masalah](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitoring Intune Device Compliance](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Langkah-langkah ini hanya membantu dalam pemecahan masalah akses bersyarat fitur direktori aktif Azure. Memungkinkan untuk mengkarantina perangkat yang memblokir akses email itu dengan kebijakan Exchange. Informasi selengkapnya tentang manajemen perangkat Exchange bisa ditemukan [**di sini**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
