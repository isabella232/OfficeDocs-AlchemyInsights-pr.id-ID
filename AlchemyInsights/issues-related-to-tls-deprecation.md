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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="ecfbc-102">Tidak dapat mengirim/menerima email ke/dari Office 365 karena Disablement TLS 1,0 dan TLS 1,1</span><span class="sxs-lookup"><span data-stu-id="ecfbc-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="ecfbc-103">Seperti yang dikonfirmasi oleh penghentian postingan pusat pesan MC229914, TLS 1,0 dan TLS 1,1 penghentian mulai memberlakukan untuk titik akhir aliran email Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ecfbc-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="ecfbc-104">Segera Office 365 tidak akan lagi menerima TLS 1,0 dan TLS 1,1 koneksi email dari sumber eksternal.</span><span class="sxs-lookup"><span data-stu-id="ecfbc-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="ecfbc-105">Selain itu, Exchange Online tidak akan pernah menggunakan TLS 1,0 atau 1,1 untuk mengirim email keluar.</span><span class="sxs-lookup"><span data-stu-id="ecfbc-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="ecfbc-106">Jika Anda menghadapi masalah karena perbaikan TLS 1,0 atau 1,1, Anda mungkin mengalami salah satu kesalahan berikut ini-</span><span class="sxs-lookup"><span data-stu-id="ecfbc-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="ecfbc-107">Pengirim mendapatkan NDR Bounce Back-' 421 4.4.2 koneksi menurun karena SocketError '</span><span class="sxs-lookup"><span data-stu-id="ecfbc-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ecfbc-108">Kesalahan dalam antrian penampil server lokal yang mengirim email ke petugas 365-' 421 4.4.2 koneksi turun karena SocketError '</span><span class="sxs-lookup"><span data-stu-id="ecfbc-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ecfbc-109">Kesalahan dalam [log protokol](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) Konektor Kirim di server yang mengirim email ke negosiasi Office 365-TLS gagal dengan kesalahan SocketError</span><span class="sxs-lookup"><span data-stu-id="ecfbc-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="ecfbc-110">Kesalahan dalam Kirim atau terima protokol konektor log-' 451 5.7.3 harus mengeluarkan perintah STARTTLS terlebih dahulu '</span><span class="sxs-lookup"><span data-stu-id="ecfbc-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="ecfbc-111">Jika Anda mengalami kesalahan di atas, pastikan server yang mengirim atau menerima email memiliki TLS 1,2 diaktifkan dengan memeriksa kunci registri berikut-</span><span class="sxs-lookup"><span data-stu-id="ecfbc-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="ecfbc-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klien] **"Disabledbydefault" = DWORD: 00000000 "diaktifkan" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"disabledbydefault" = DWORD: 00000000 "diaktifkan" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="ecfbc-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="ecfbc-113">Jika Anda membuat perubahan dalam kunci registri di atas untuk mengaktifkan TLS 1,2, mulai ulang server agar perubahan tersebut diterapkan.</span><span class="sxs-lookup"><span data-stu-id="ecfbc-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="ecfbc-114">Pastikan juga Anda memiliki pembaruan Windows dan Exchange terbaru yang terinstal.</span><span class="sxs-lookup"><span data-stu-id="ecfbc-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="ecfbc-115">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="ecfbc-115">For more information, see:</span></span>

- [<span data-ttu-id="ecfbc-116">Panduan TLS Exchange Server, Bagian 1: bersiap untuk TLS 1,2-komunitas teknologi Microsoft</span><span class="sxs-lookup"><span data-stu-id="ecfbc-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="ecfbc-117">Panduan TLS Exchange Server Bagian 2: mengaktifkan TLS 1,2 dan mengidentifikasi klien yang tidak menggunakannya-komunitas teknologi Microsoft</span><span class="sxs-lookup"><span data-stu-id="ecfbc-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="ecfbc-118">Memahami skenario email jika versi TLS tidak dapat disepakati dengan Exchange Online-komunitas teknologi Microsoft</span><span class="sxs-lookup"><span data-stu-id="ecfbc-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
