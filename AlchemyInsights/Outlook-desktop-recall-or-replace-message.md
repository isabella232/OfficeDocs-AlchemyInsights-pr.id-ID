---
title: Outlook desktop memanggil kembali atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663993"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Memanggil kembali atau mengganti pesan email Outlook

- Sebagai admin, Anda dapat **memanggil kembali pesan atas nama pengguna menggunakan PowerShell**. Anda tidak bisa mengingat pesan dari Pusat admin.
- Anda **hanya bisa mengingat pesan yang dikirim ke orang di dalam organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa mengingatnya.
- Anda **hanya dapat mengingat pesan yang dikirim dari Outlook 2016 di PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingatnya.

Untuk memanggil kembali atau mengganti pesan email:

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
1. Klik ganda pesan yang ingin Anda ingat untuk membukanya.
1. Pilih tab **pesan** , lalu pilih **tindakan**  >  **ingat pesan ini**.
1. Pilih **Hapus salinan yang belum dibaca dari pesan ini** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.
1. Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.
1. Keberhasilan atau kegagalan penarikan kembali pesan bergantung pada pengaturan penerima di Outlook. Untuk langkah-langkah untuk memeriksa penarikan kembali, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Mencari dan menghapus pesan email di organisasi Anda

- Jika Anda bukan admin global, akun Anda harus ditambahkan ke peran Manajer eDiscovery atau peran manajemen pencarian kepatuhan untuk mencari pesan. Untuk menghapus pesan, Anda harus bergabung dalam grup peran manajemen organisasi atau peran manajemen pencarian dan penghapusan. Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.
- [Sambungkan ke pusat keamanan dan kepatuhan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jika Anda menggunakan autentikasi multifaktor, lihat [menyambungkan ke Microsoft 365 Security and Compliance Center PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).