---
title: Cara menambahkan atau menghapus delegasi di Outlook untuk Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573579"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Cara menambahkan atau menghapus delegasi di Outlook untuk Windows

Untuk menambahkan delegasi di Outlook untuk Windows: 

1. Klik tab **file** yang diikuti dengan **pengaturan akun**, lalu pilih **akses delegasi**.
2. Klik **Tambahkan**. Jika **Add** tidak muncul, koneksi aktif mungkin tidak ada antara Outlook dan Exchange. Bilah status Outlook menampilkan status koneksi.
3. Ketikkan nama orang yang ingin Anda tetapkan sebagai delegasi Anda, atau Cari dan pilih nama dalam daftar hasil pencarian.

    > [!NOTE]
    > Delegasi harus merupakan orang di daftar alamat global (GAL) organisasi Anda.
4. Klik **Tambahkan** diikuti dengan **OK**.
5. Dalam kotak dialog **izin delegasi** , terima pengaturan izin default atau pilih tingkat akses kustom untuk folder Exchange.

    - Jika delegasi memerlukan izin untuk bekerja hanya dengan permintaan dan respons Rapat, pengaturan izin default seperti **delegasi menerima salinan pesan terkait Rapat yang dikirimkan kepada saya** sudah cukup. Anda dapat membiarkan pengaturan izin **kotak masuk** **tidak ada**. Permintaan dan respons Rapat akan langsung masuk ke kotak masuk delegasi.

    > [!NOTE]
    > Secara default, delegasi diberikan izin **editor (dapat membaca, membuat, dan mengubah item)** ke folder **kalender** Anda. Saat delegasi merespons ke Rapat atas nama Anda, delegasi tersebut secara otomatis ditambahkan ke folder **kalender** Anda.

5. Untuk mengirim pesan untuk memberi tahu delegasi izin yang diubah, pilih kotak centang **secara otomatis mengirim pesan untuk mendelegasikan ringkasan izin ini** .
6. Jika Anda ingin, pilih kotak centang **delegasi dapat melihat item pribadi saya** .

    > [!IMPORTANT]
    > Pengaturan ini mempengaruhi semua folder Exchange. Ini mencakup semua email, kontak, kalender, tugas, catatan, dan folder jurnal. Tidak ada cara untuk memberi akses ke item pribadi dalam folder tertentu saja.

7. Pilih **OK**.

    > [!NOTE]
    >
    > - Pesan yang dikirim dengan izin Kirim atas nama menyertakan delegasi dan nama Anda di samping **dari**. Saat pesan dikirim dengan izin Kirim sebagai, hanya nama Anda yang muncul.
    > - Setelah Anda menambahkan seseorang sebagai delegasi, mereka bisa menambahkan kotak surat Exchange Anda ke profil Outlook mereka. Untuk instruksi, lihat [mengelola email dan item kalender orang lain](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Untuk menghapus delegasi di Outlook untuk Windows:

1. Klik tab **file** .
2. Klik **pengaturan akun** yang diikuti oleh **akses delegasi**.
3. Pilih nama delegasi yang ingin Anda ubah izinnya, lalu klik **Hapus** diikuti dengan **OK**.
