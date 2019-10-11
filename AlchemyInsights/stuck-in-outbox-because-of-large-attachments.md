---
title: Terjebak dalam outbox karena lampiran besar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441309"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Memperbaiki pesan yang terjebak di kotak keluar

Kami sarankan Anda memulai dengan menjalankan skenario ["saya mengalami masalah mengirim, menerima, atau menemukan pesan email"](https://aka.ms/SaRA-OutlookSendReceive) dari [Microsoft dukungan dan pemulihan asisten](https://diagnostics.office.com/#/) alat.

Saat pesan macet di kotak keluar, kemungkinan penyebabnya adalah:
- Lampiran besar.
- **Kirim segera ketika opsi tersambung** tidak diaktifkan.

Untuk menghapus lampiran berukuran besar: 

1. Di Outlook, pilih **kirim/terima** > **bekerja secara offline**. 
2. Di panel navigasi, pilih **kotak keluar**. Dari sini, Anda dapat: 
    - Hapus pesan (pilih dan pilih **Hapus**).
    - Seret pesan ke folder draf, klik dua kali untuk membukanya, dan Hapus lampiran memilihnya lalu pilih **Hapus**).
3. Jika Anda menerima galat yang mengatakan Outlook mencoba untuk mengirimkan pesan, tutup Outlook. Mungkin perlu beberapa saat untuk keluar. Jika Outlook tidak menutup, tekan CTRL + ALT + delete dan pilih **mulai pengelola tugas**. Di Manajer tugas, pilih tab **proses** , gulir ke bawah ke Outlook. exe, dan pilih **Akhiri proses**.
4. Setelah menutup Outlook, mulai ulang dan ulangi langkah 2 dan 3. 
5. Setelah Anda menghapus lampiran, klik **kirim/terima** > **bekerja secara offline** untuk melanjutkan kerja online. 

Pesan juga macet di kotak keluar bila Anda mengklik **kirim**, namun Anda tidak tersambung. Klik **kirim/terima** dan lihat tombol **bekerja offline** . Jika berwarna biru, Anda akan terputus. Pilih untuk menghubungkan (tombol berubah putih) dan klik **kirim semua**.
 
Untuk mengaktifkan **kirim segera ketika terhubung**:
 
- Pilih **file** > **Options** >  **Advanced**.
Di bagian **mengirim dan menerima** , pilih **kirim segera ketika tersambung**, dan kemudian pilih **OK**.
 
Untuk detail selengkapnya, lihat:
- [Video: mengirim atau menghapus email yang macet](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Email tetap berada di folder kotak keluar sampai Anda secara manual memulai operasi kirim/terima di Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
