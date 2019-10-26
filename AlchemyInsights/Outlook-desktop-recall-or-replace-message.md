---
title: Outlook desktop ingat atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496114"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Ingat atau ganti pesan email Outlook

- Sebagai admin, Anda dapat **memanggil kembali pesan atas nama pengguna menggunakan PowerShell**. Anda tidak dapat mengingat pesan dari Pusat admin.
- Anda **hanya dapat mengingat pesan yang dikirim ke orang di organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak dapat mengingatnya.
- Anda **hanya dapat mengingat pesan yang dikirim dari Outlook 2016 pada PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak dapat mengingatnya.

Untuk mengingat atau mengganti pesan email:

1. Di panel folder di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
1. Klik pesan dua kali yang ingin Anda ingat untuk membukanya.
1. Pilih tab **pesan** , dan kemudian pilih **tindakan** > yang**ingat pesan ini**.
1. Pilih **Hapus salinan pesan yang belum dibaca** atau **Hapus salinan yang belum dibaca dan ganti dengan pesan baru**, lalu pilih **OK**.
1. Jika Anda mengirim pesan pengganti, tulis pesan, lalu pilih **kirim**.
1. Keberhasilan atau kegagalan pesan ingat tergantung pada pengaturan penerima di Outlook. Untuk langkah untuk memeriksa Recall, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Mencari dan menghapus pesan email di organisasi Anda

- Jika Anda bukan admin global, akun Anda harus ditambahkan ke peran pengelola eDiscovery atau peran manajemen penelusuran kepatuhan untuk mencari pesan. Untuk menghapus pesan, Anda harus bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan. Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Membuat pencarian konten](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan yang akan dihapus.
- [Sambungkan ke pusat keamanan dan kepatuhan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jika Anda menggunakan otentikasi multi faktor, lihat [tersambung ke Office 365 keamanan dan kepatuhan pusat PowerShell menggunakan otentikasi multi faktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).