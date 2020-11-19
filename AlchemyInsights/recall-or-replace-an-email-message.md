---
title: Memanggil kembali atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353509"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Memanggil kembali atau mengganti pesan email di Microsoft 365

- Anda **hanya bisa mengingat pesan yang dikirim ke orang di dalam organisasi Anda**. Misalnya, jika pesan dikirim ke alamat Gmail, Anda tidak dapat mengingatnya.
- Anda **hanya dapat mengingat pesan yang dikirim dari Outlook untuk PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingatnya.
- Sebagai administrator penyewa, Anda bisa **mengingat pesan atas nama pengguna menggunakan PowerShell** (untuk informasi selengkapnya, lihat: [mencari dan menghapus pesan email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Anda tidak bisa mengingat pesan dari Pusat admin. Gulir ke bawah ke "Cari dan Hapus pesan email di organisasi Anda" untuk informasi selengkapnya.

**Memanggil kembali atau mengganti pesan email yang Anda kirim**

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
2. Buka pesan yang ingin Anda ingat. Anda harus mengklik ganda untuk membuka pesan. Memilih pesan sehingga muncul di panel baca tidak akan memperbolehkan Anda untuk mengingat pesan.
3. Dari tab Pesan, pilih **tindakan**  >  **ingat pesan ini**.
4. Pilih **Hapus salinan yang belum dibaca dari pesan ini** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.
5. Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.
6. Keberhasilan atau kegagalan penarikan kembali pesan bergantung pada pengaturan penerima di Outlook.

Untuk informasi selengkapnya, termasuk cara memeriksa penarikan kembali, lihat memanggil kembali [atau mengganti pesan email yang Anda kirim](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Untuk mencari dan menghapus pesan email di organisasi Anda_**, sangat mudah jika Anda adalah admin global. Jika Anda bukan admin global, akun Anda harus ditambahkan ke grup peran Manajer eDiscovery, atau ke peran manajemen pencarian kepatuhan. Untuk menghapus pesan, Anda harus bergabung dalam grup peran manajemen organisasi atau peran manajemen pencarian dan penghapusan. Izin untuk peran ini ditetapkan di [pusat kepatuhan & keamanan](https://protection.office.com/).

1. [Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.
2. [Sambungkan ke pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Jika Anda menggunakan MFA (multi-Factor Authentication), lihat [menyambungkan ke Microsoft 365 Security & pusat kepatuhan PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
