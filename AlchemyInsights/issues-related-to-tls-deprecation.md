---
title: Tidak dapat mengirim/menerima email ke/dari Office 365 karena Disablement TLS 1,0 dan TLS 1,1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745015"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Tidak dapat mengirim/menerima email ke/dari Office 365 karena Disablement TLS 1,0 dan TLS 1,1

Seperti yang dikonfirmasi oleh penghentian postingan pusat pesan MC229914, TLS 1,0 dan TLS 1,1 penghentian mulai memberlakukan untuk titik akhir aliran email Exchange Online. Segera Office 365 tidak akan lagi menerima TLS 1,0 dan TLS 1,1 koneksi email dari sumber eksternal. Selain itu, Exchange Online tidak akan pernah menggunakan TLS 1,0 atau 1,1 untuk mengirim email keluar. Jika Anda menghadapi masalah karena perbaikan TLS 1,0 atau 1,1, Anda mungkin mengalami salah satu kesalahan berikut ini-

- Pengirim mendapatkan NDR Bounce Back-' 421 4.4.2 koneksi menurun karena SocketError '
- Kesalahan dalam antrian penampil server lokal yang mengirim email ke petugas 365-' 421 4.4.2 koneksi turun karena SocketError '
- Kesalahan dalam [log protokol](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) Konektor Kirim di server yang mengirim email ke negosiasi Office 365-TLS gagal dengan kesalahan SocketError
- Kesalahan dalam Kirim atau terima protokol konektor log-' 451 5.7.3 harus mengeluarkan perintah STARTTLS terlebih dahulu '

Jika Anda mengalami kesalahan di atas, pastikan server yang mengirim atau menerima email memiliki TLS 1,2 diaktifkan dengan memeriksa kunci registri berikut-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klien] **"Disabledbydefault" = DWORD: 00000000 "diaktifkan" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"disabledbydefault" = DWORD: 00000000 "diaktifkan" = DWORD: 00000001**

Jika Anda membuat perubahan dalam kunci registri di atas untuk mengaktifkan TLS 1,2, mulai ulang server agar perubahan tersebut diterapkan. Pastikan juga Anda memiliki pembaruan Windows dan Exchange terbaru yang terinstal.

Untuk informasi selengkapnya, lihat:

- [Panduan TLS Exchange Server, Bagian 1: bersiap untuk TLS 1,2-komunitas teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Panduan TLS Exchange Server Bagian 2: mengaktifkan TLS 1,2 dan mengidentifikasi klien yang tidak menggunakannya-komunitas teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Memahami skenario email jika versi TLS tidak dapat disepakati dengan Exchange Online-komunitas teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
