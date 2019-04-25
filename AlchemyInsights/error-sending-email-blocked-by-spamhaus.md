---
title: Pengiriman email yang diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402262"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f9093-102">Pengiriman email: host klien yang diblokir menggunakan Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f9093-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f9093-103">Alamat IP yang mengirim pesan adalah pada daftar blokir yang dimiliki oleh [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f9093-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f9093-104">Alasan untuk diblokir oleh Spamhaus menyertakan account dikompromikan, dikompromikan mesin berbagi alamat IP publik, dan kebijakan Internet Service Provider (ISP).</span><span class="sxs-lookup"><span data-stu-id="f9093-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f9093-105">Perbaikan yang mungkin adalah:</span><span class="sxs-lookup"><span data-stu-id="f9093-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f9093-106">Diblokir inbound pesan ke Office 365 mana Anda kontrol sumber server email, Anda perlu untuk menentukan penyebab dan menghapus blok dari situs Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f9093-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="f9093-107">Diblokir inbound pesan ke Office 365 mana alamat IP sumber milik orang lain, pemilik alamat kebutuhan untuk menghapus blok dari situs Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f9093-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f9093-108">Jika alamat IP pada kebijakan blok daftar (PBL), pemilik dapat menetapkan alamat IP statis yang berbeda atau menghapus alamat dari PBL.</span><span class="sxs-lookup"><span data-stu-id="f9093-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="f9093-109">Untuk pesan keluar diblokir dari domain Office 365, Anda dapat menerima kesalahan ini jika pesan akan diteruskan melalui layanan pihak ke-3.</span><span class="sxs-lookup"><span data-stu-id="f9093-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f9093-110">Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.</span><span class="sxs-lookup"><span data-stu-id="f9093-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

