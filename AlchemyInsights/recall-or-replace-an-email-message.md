---
title: Ingat atau ganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509459"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Ingat atau ganti pesan email di Microsoft 365

- Anda **hanya dapat mengingat pesan yang dikirim ke orang di organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak dapat mengingatnya.
- Anda **hanya dapat mengingat pesan yang dikirim dari Outlook 2016 untuk PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak dapat mengingatnya.
- Jika Anda adalah admin, Anda dapat **mengingat pesan atas nama pengguna menggunakan PowerShell**. Anda tidak dapat mengingat pesan dari Pusat admin. Scroll ke bawah ke "Cari dan Hapus pesan email di organisasi" untuk informasi selengkapnya.

**Ingat atau ganti pesan email yang Anda kirim**

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
2. Buka pesan yang ingin Anda ingat. Anda harus mengklik dua kali untuk membuka pesan. Memilih pesan sehingga muncul di panel baca tidak akan memungkinkan Anda untuk mengingat pesan.
3. Dari tab Pesan, pilih **tindakan**yang  >  **mengingat pesan ini**.
4. Pilih **Hapus salinan pesan ini yang belum dibaca** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.
5. Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.
6. Keberhasilan atau kegagalan pesan ingat tergantung pada pengaturan penerima di Outlook.

Untuk informasi lebih lanjut, termasuk cara memeriksa Recall, lihat [ingat atau ganti pesan email yang Anda kirim](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Mencari ***dan menghapus pesan email di organisasi Anda*** Untuk mencari dan menghapus pesan email di organisasi Anda, sangat mudah jika Anda adalah admin global. Jika Anda bukan admin global, akun Anda harus ditambahkan ke grup peran pengelola eDiscovery, atau ke peran manajemen penelusuran kepatuhan. Untuk menghapus pesan, Anda harus bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan. Izin untuk peran ini ditetapkan di [pusat kepatuhan & keamanan](https://protection.office.com/).

1. [Membuat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.
2. [Menyambung ke keamanan & kepatuhan pusat PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Jika Anda menggunakan MFA, lihat [tersambung ke Microsoft 365 keamanan & pusat kepatuhan PowerShell menggunakan otentikasi multi faktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
