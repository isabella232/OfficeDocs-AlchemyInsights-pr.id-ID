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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024389"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Memanggil kembali atau mengganti pesan email di Microsoft 365

- Anda hanya **bisa memanggil kembali pesan yang dikirim ke orang di organisasi Anda**. Misalnya, jika pesan dikirimkan ke alamat Gmail, Anda tidak dapat memanggil kembali alamat tersebut.
- Anda hanya **dapat memanggil kembali pesan yang dikirim Outlook untuk PC.** Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa memanggil kembali pesan itu.
- Sebagai administrator penyewa, Anda dapat memanggil kembali pesan atas nama pengguna menggunakan **PowerShell** (Untuk informasi selengkapnya, lihat: [Mencari dan menghapus pesan email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Anda tidak dapat memanggil kembali pesan dari pusat admin. Gulir ke bawah ke "Cari dan hapus pesan email di organisasi Anda" untuk informasi selengkapnya.

**Memanggil kembali atau mengganti pesan email yang telah Anda kirimkan**

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
2. Buka pesan yang ingin Anda panggil kembali. Klik dua kali untuk membuka pesan. Memilih pesan hingga muncul di panel baca tidak memungkinkan Anda untuk menarik pesan kembali.
3. Dari tab Pesan, pilih Tindakan **Panggil Kembali**  >  **Pesan Ini**.
4. Pilih **Hapus salinan yang belum dibaca untuk pesan ini** atau Hapus salinan yang belum dibaca dan ganti dengan pesan **baru**, lalu pilih **OK.**
5. Jika ingin mengirimkan pesan pengganti, tulis pesan, lalu pilih **Kirim**.
6. Keberhasilan atau kegagalan penarikan pesan bergantung pada pengaturan penerima di Outlook.

Untuk informasi selengkapnya, termasuk cara memeriksa penarikan kembali, lihat Memanggil [kembali atau mengganti pesan email yang dikirimkan.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Untuk mencari dan menghapus pesan email di organisasi Anda,*** akan lebih mudah jika Anda adalah admin global. Jika Anda bukan admin global, akun Anda harus ditambahkan ke grup peran Manajer eDiscovery, atau ke peran manajemen Pencarian Kepatuhan. Untuk menghapus pesan, Anda harus bergabung dalam grup peran Manajemen Organisasi atau peran manajemen Pencarian dan Pembersihan. Izin untuk peran ini ditetapkan di pusat keamanan [& kepatuhan .](https://protection.office.com/)

1. [Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.
2. [Koneksi ke PowerShell Pusat & Security .](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Jika Anda menggunakan MFA (multi-factor authentication), lihat Koneksi Microsoft 365 Security & Compliance Center PowerShell menggunakan [multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
