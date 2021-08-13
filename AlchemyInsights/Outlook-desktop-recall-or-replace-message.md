---
title: Outlook Memanggil kembali desktop atau mengganti pesan email
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918398"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Menarik kembali atau mengganti Outlook email

- Sebagai admin, Anda dapat **memanggil kembali pesan atas nama pengguna yang menggunakan PowerShell**. Anda tidak dapat memanggil kembali pesan dari pusat admin.
- Anda hanya **bisa memanggil kembali pesan yang dikirim ke orang di organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa memanggil kembali pesan itu.
- Anda hanya **bisa memanggil kembali pesan yang dikirim Outlook 2016 di PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa memanggil kembali pesan itu.

Untuk menarik kembali atau mengganti pesan email:

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
1. Klik ganda pesan yang ingin Anda panggil kembali untuk membukanya.
1. Pilih tab **Pesan,** lalu pilih Tindakan **Panggil**  >  **Kembali Pesan Ini**.
1. Pilih **Hapus salinan yang belum dibaca untuk pesan** ini atau Hapus salinan yang belum dibaca dan ganti dengan pesan **baru**, lalu pilih **OK.**
1. Jika ingin mengirimkan pesan pengganti, tulis pesan, lalu pilih **Kirim**.
1. Keberhasilan atau kegagalan penarikan pesan bergantung pada pengaturan penerima di Outlook. Untuk langkah-langkah memeriksa penarikan kembali, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Mencari dan menghapus pesan email di organisasi Anda

- Jika Anda bukan admin global, akun Anda harus ditambahkan ke peran Manajer eDiscovery atau peran manajemen Pencarian Kepatuhan untuk mencari pesan. Untuk menghapus pesan, Anda harus bergabung dalam grup peran Manajemen Organisasi atau peran manajemen Pencarian dan Pembersihan. Izin untuk peran ini ditetapkan di pusat [Keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Buat pencarian konten](https://docs.microsoft.com/microsoft-365/compliance/content-search) untuk menemukan pesan yang akan dihapus.
- [Koneksi ke PowerShell Pusat Keamanan dan Kepatuhan](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jika Anda menggunakan multi-factor authentication, lihat Koneksi to [Microsoft 365 Compliance Center PowerShell menggunakan multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).