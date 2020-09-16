---
title: Memecahkan masalah audio di Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750310"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Memecahkan masalah audio di Windows 10

**Menjalankan pemecah masalah audio**

1.  Buka [pengaturan pemecahan masalah](ms-settings:troubleshoot).

2.  Pilih **putar audio**  >  **Jalankan pemecah masalah**.

**Mengatur perangkat default**

Jika Anda menyambungkan ke perangkat audio menggunakan USB atau HDMI, Anda mungkin perlu mengatur perangkat tersebut sebagai default:

1. Buka **mulai**  >  **suara**, lalu pilih **suara** atau **Ubah suara sistem** dari daftar hasil.

2.  Pada tab **pemutaran** , pilih perangkat, pilih **setel default**, lalu pilih **OK**.

**Memeriksa kabel, volume, speaker, dan headphone**

1. Periksa koneksi speaker dan headphone Anda untuk kabel longgar, dan pastikan tersambung ke Jack yang tepat.

2. Periksa tingkat kekuatan dan volume Anda dan cobalah mengubah semua kontrol volume ke atas.

3. Beberapa speaker dan aplikasi memiliki kontrol volume sendiri; Anda mungkin harus memeriksa semuanya untuk memastikan mereka berada di tingkat yang tepat.

4. Cobalah menyambungkan menggunakan port USB yang berbeda.

**Catatan**: ingat bahwa speaker Anda mungkin tidak berfungsi ketika headphone dicolokkan.

**Periksa manajer perangkat**

Untuk memastikan bahwa driver telah diperbarui:

1. Pilih **mulai**, ketikkan **manajer perangkat**, lalu pilih **pengelola perangkat** dari daftar hasil.

2. Di bawah **suara, video, dan pengendali permainan**, pilih kartu suara Anda, buka, pilih tab **pengandar** , dan pilih **Perbarui pengandar**.

**Catatan**: jika Windows tidak menemukan driver baru, Cari salah satu di situs web pabrikan perangkat dan ikuti instruksinya.

**Menginstal ulang driver**

Jika Anda tidak dapat memperbarui melalui manajer perangkat atau menemukan driver baru di situs web produsen, cobalah langkah-langkah berikut:

1. Di manajer perangkat, klik kanan (atau tekan dan tahan) driver audio, lalu pilih **hapus instalan**. Mulai ulang perangkat Anda dan Windows akan mencoba menginstal ulang driver.

2. Jika menginstal ulang driver tidak berfungsi, coba gunakan driver audio generik yang disertakan dengan Windows. Di manajer perangkat, klik kanan (atau tekan dan tahan) driver audio Anda > **Perbarui perangkat lunak pengandar**  >  **Telusuri komputer saya untuk perangkat lunak pengandar**  >  **biarkan saya memilih dari daftar driver perangkat di komputer saya**, pilih **perangkat audio definisi tinggi**, pilih **berikutnya**, dan ikuti instruksi untuk menginstalnya.
