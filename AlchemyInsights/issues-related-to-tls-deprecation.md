---
title: Tidak dapat mengirim/menerima email ke/dari Office 365 karena pennonaktifkan TLS 1.0 dan TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054909"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Tidak dapat mengirim/menerima email ke/dari Office 365 karena pennonaktifkan TLS 1.0 dan TLS 1.1

Saat dikonfirmasi oleh postingan pusat pesan MC229914, TLS 1.0 dan TLS 1.1 penghentian mulai memberlakukan Exchange Online titik akhir aliran email. Segera Office 365 menerima koneksi email TLS 1.0 dan TLS 1.1 dari sumber eksternal. Selain itu, Exchange Online tidak akan pernah menggunakan TLS 1.0 atau 1.1 untuk mengirim email keluar. Jika Anda mengalami masalah karena pennonaktifkan TLS 1.0 atau 1.1, Anda mungkin mengalami salah satu kesalahan berikut ini-

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Kesalahan dalam Penampil Antrean dari server Lokal yang mengirimkan email ke Officer 365- '421 4.4.2 Koneksi menurun karena SocketError'
- Kesalahan dalam Log [Protokol konektor Kirim](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) pada server saat mengirimkan email ke Office 365- Negosiasi TLS gagal dengan kesalahan SocketError
- Kesalahan dalam log protokol konektor Kirim atau terima - '451 5.7.3 Harus mengeluarkan perintah STARTTLS terlebih dahulu'

Jika mengalami salah satu kesalahan di atas, pastikan server yang mengirim atau menerima email memiliki TLS 1.2 diaktifkan dengan memeriksa kunci registri berikut-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Jika Anda membuat perubahan dalam kunci registri di atas untuk mengaktifkan TLS 1.2, mulai ulang server agar perubahan bisa diterapkan. Pastikan juga Anda telah menginstal pembaruan Windows Exchange terbaru.

Untuk informasi selengkapnya, lihat:

- [Server Exchange Panduan TLS, bagian 1: Bersiap untuk TLS 1.2 - Komunitas Teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Server Exchange Panduan TLS Bagian 2: Mengaktifkan TLS 1.2 dan Mengidentifikasi Klien yang Tidak Menggunakannya - Komunitas Teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Memahami skenario email jika versi TLS tidak dapat disetujui dengan Exchange Online - Komunitas Teknologi Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
