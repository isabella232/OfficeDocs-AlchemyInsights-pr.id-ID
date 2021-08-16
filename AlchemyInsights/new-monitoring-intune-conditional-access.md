---
title: Memantau Akses Kondisional Intune
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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025505"
---
# <a name="monitor-intune-conditional-access"></a>Memantau Akses Kondisional Intune

Pengguna yang mendapatkan akses kondisional akan menerima email pemberitahuan jika mereka tidak memenuhi persyaratan akses organisasi Anda. Untuk mengatasinya, kami menyarankan satu atau beberapa solusi berikut:

1. Jika perangkat terdaftar, sarankan pengguna untuk masuk ke aplikasi Company Portal dan pastikan bahwa perangkat muncul di Company Portal. Jika tidak ada, pengguna harus mendaftarkan perangkat tersebut.
1. Di portal Azure, masuk ke **Intune**  >  **Device compliance**. 
1. Untuk menampilkan laporan kepatuhan perangkat untuk memastikan bahwa perangkat pengguna telah ditandai sebagai memenuhi syarat, di **bawah Monitor,** klik **Kepatuhan perangkat.**
1. Di portal Azure, masuk ke **Intune**  >  **Device compliance**. Di **bawah Kelola,** klik **Kebijakan.** Dalam daftar kebijakan kepatuhan, verifikasi bahwa profil telah ditetapkan ke perangkat pengguna Anda. Jika belum ditetapkan, Intune tidak akan dapat mengonfirmasi status kepatuhan perangkat.
1. Edit penetapan akses kondisional pengguna.
1. Di portal Azure, navigasikan ke **Kebijakan akses kondisional Intune**  >    >  , pilih kebijakan dari daftar, lalu klik **Pengguna dan grup.**
1. Untuk menargetkan kebijakan tertentu kepada seseorang, tambahkan orang tersebut ke **dalam daftar Sertakan.** Untuk memastikan bahwa seseorang tidak termasuk dalam kebijakan, tambahkan orang tersebut ke **dalam daftar Pengecualian.**

**Tautan yang berguna:**

- [Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Memecahkan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Kebijakan pemecahan masalah](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Memantau kepatuhan perangkat Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Langkah-langkah ini hanya berguna dalam memecahkan Azure Active Directory Akses Bersyarat. Juga dimungkinkan untuk melakukan karantina perangkat yang memblokir akses email dengan Exchange email. Informasi selengkapnya tentang Exchange manajemen perangkat Anda bisa ditemukan di [**sini**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
