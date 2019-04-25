---
title: Ingat Desktop Outlook atau mengganti pesan email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389709"
---
# <a name="recall-or-replace-an-email-message"></a>Ingat atau mengganti pesan email

- Sebagai admin, Anda dapat **mengingat pesan atas nama pengguna menggunakan PowerShell**. Anda tidak bisa mengingat pesan dari di admin center.
- Anda dapat **hanya ingat pesan yang dikirim ke pengguna di organisasi Anda**. Jika pesan dikirim ke alamat Gmail, misalnya, Anda tidak bisa mengingat itu.
- Anda dapat **hanya ingat pesan yang dikirim dari Outlook 2016 pada PC**. Jika pengguna mengirim pesan menggunakan Outlook untuk Mac atau Outlook di web, Anda tidak bisa mengingat itu.

Untuk ingat atau mengganti pesan email:

1. Di panel map di sebelah kiri jendela Outlook, pilih folder Item Terkirim.
1. Klik dua kali pesan yang ingin Anda ingat untuk membukanya.
1. Pilih tab **pesan** , dan kemudian pilih **tindakan** > **Ingat pesan ini**.
1. Pilih **Hapus belum dibaca salinan pesan ini** atau **menghapus salinan yang belum dibaca dan menggantinya dengan pesan baru**, dan kemudian pilih **OK**.
1. Jika Anda mengirim pesan penggantian, menulis pesan, dan pilih **kirim**.
1. Keberhasilan atau kegagalan mengingat pesan tergantung pada pengaturan penerima di Outlook. Langkah-langkah untuk memeriksa ingat, lihat [artikel ini](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Mencari dan menghapus pesan email di organisasi Anda

- Jika Anda tidak global admin, akun Anda harus ditambahkan ke peran Manajer eDiscovery atau peran manajemen pencarian kepatuhan untuk mencari pesan. Untuk menghapus pesan, Anda akan perlu untuk bergabung dengan grup peran manajemen organisasi atau peran manajemen pencarian dan pembersihan. Izin untuk peran ini ditetapkan di [pusat keamanan dan kepatuhan](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Buat konten pencarian](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan untuk menghapus.
- [Terhubung ke keamanan dan kepatuhan pusat PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jika Anda menggunakan otentikasi faktor multi, lihat [tersambung ke kantor 365 keamanan dan kepatuhan pusat PowerShell menggunakan multi faktor otentikasi](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).