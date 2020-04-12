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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232633"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Memperbaiki pesan yang terjebak di kotak keluar

Kami sarankan Anda memulai dengan menjalankan skenario ["saya mengalami masalah mengirim, menerima, atau menemukan pesan email"](https://aka.ms/SaRA-OutlookSendReceive) dari [Microsoft Support dan pemulihan asisten](https://diagnostics.office.com/#/) alat pada mesin yang terpengaruh.

Saat pesan macet di kotak keluar, kemungkinan penyebabnya adalah lampiran besar atau opsi "Kirim segera saat tersambung" tidak diaktifkan.

**Menghapus lampiran besar**

1. Klik **kirim/terima** > **bekerja secara offline**. 
2. Di panel navigasi, klik **kotak keluar**. Dari sini, Anda dapat: 
    - Hapus pesan. Cukup pilih dan klik **Delete**.
    - Seret pesan ke **folder draf**, klik dua kali untuk membuka pesan, dan Hapus lampiran (klik dan klik **Hapus**).
3. Jika kesalahan memberitahu Anda Outlook mencoba untuk mengirimkan pesan, tutup Outlook. Mungkin perlu beberapa saat untuk keluar. Jika Outlook tidak menutup, tekan **CTRL + ALT + delete** dan klik **mulai manajer tugas**. Di Manajer tugas, pilih tab **proses** , gulir ke bawah ke Outlook. exe, dan klik **Akhiri proses**.
4. Setelah menutup Outlook, mulai ulang Outlook dan ulangi langkah 2-3. 
5. Setelah Anda menghapus lampiran, klik **kirim/terima** > **bekerja secara offline** untuk membatalkan pilihan tombol dan untuk melanjutkan kerja secara online. 

Pesan juga macet di kotak keluar bila Anda mengklik **kirim**, namun Anda tidak tersambung. Klik **kirim/terima** dan lihat tombol **bekerja offline** . Jika berwarna biru, Anda akan terputus. Klik untuk menghubungkan (tombol berubah putih) dan klik **kirim semua**.
 
**Aktifkan kirim segera ketika terhubung**
 
1. Pada file tab, klik **opsi**.

2. Di kotak dialog Opsi Outlook, klik **lanjut**.

3. Di bagian kirim dan terima, klik untuk mengaktifkan **kirim segera ketika tersambung**. Klik **OK**.
 
Untuk detail selengkapnya, lihat:
- [Video: mengirim atau menghapus email yang macet](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Email tetap berada di folder kotak keluar sampai Anda secara manual memulai operasi kirim/terima di Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
