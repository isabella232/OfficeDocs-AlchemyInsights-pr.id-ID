---
title: Kesalahan saat mengirim email yang diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813727"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ce454-102">Terjadi kesalahan saat mengirimkan email: Host klien diblokir menggunakan Spamhaus</span><span class="sxs-lookup"><span data-stu-id="ce454-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ce454-103">Alamat IP yang mengirimkan pesan tersebut berada dalam daftar blokir milik [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="ce454-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ce454-104">Alasan pemblokiran yang dilakukan oleh Spamhaus meliputi akun dibobol, komputer yang menggunakan alamat IP publik yang sama dibobol, dan kebijakan Penyedia Layanan Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="ce454-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ce454-105">Perbaikan yang dapat dilakukan adalah:</span><span class="sxs-lookup"><span data-stu-id="ce454-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ce454-106">Untuk pesan masuk yang diblokir tempat Anda mengontrol server email sumber, Anda harus menentukan penyebabnya dan menghapus blokir dari situs web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ce454-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ce454-107">Untuk pesan masuk yang diblokir yang alamat IP sumbernya merupakan milik orang lain, pemilik alamat harus menghapus blokir dari situs web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ce454-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ce454-108">Jika alamat IP berada dalam Daftar Blokir Kebijakan (PBL), pemilik dapat menetapkan alamat IP statis lain atau menghapus alamat dari PBL.</span><span class="sxs-lookup"><span data-stu-id="ce454-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ce454-109">Untuk pesan keluar yang diblokir dari domain Anda yang tersambung ke Microsoft, Anda dapat menerima kesalahan ini jika pesan dirutekan melalui layanan pihak ke-3.</span><span class="sxs-lookup"><span data-stu-id="ce454-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ce454-110">Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.</span><span class="sxs-lookup"><span data-stu-id="ce454-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
