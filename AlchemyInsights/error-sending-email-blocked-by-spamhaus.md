---
title: Kesalahan pengiriman email diblokir oleh SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783806"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="52701-102">Kesalahan mengirim email: host klien diblokir menggunakan SpamHaus</span><span class="sxs-lookup"><span data-stu-id="52701-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="52701-103">Alamat IP yang mengirim pesan ada di daftar blokir yang dimiliki oleh [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="52701-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="52701-104">Alasan diblokir oleh SpamHaus termasuk akun yang dikompromikan, Mesin disusupi berbagi alamat IP publik, dan kebijakan penyedia layanan internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="52701-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="52701-105">Kemungkinan perbaikan adalah:</span><span class="sxs-lookup"><span data-stu-id="52701-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="52701-106">Untuk pesan masuk yang diblokir tempat Anda mengontrol server email sumber, Anda harus menentukan penyebabnya dan menghapus blok dari situs web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="52701-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="52701-107">Untuk pesan masuk yang diblokir tempat alamat IP sumber milik orang lain, pemilik alamat harus menghapus blok dari situs web SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="52701-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="52701-108">Jika alamat IP berada di daftar blokir kebijakan (PBL), pemilik dapat menetapkan alamat IP statis berbeda atau menghapus alamat dari PBL.</span><span class="sxs-lookup"><span data-stu-id="52701-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="52701-109">Untuk pesan keluar yang diblokir dari domain Anda yang tersambung ke Microsoft, Anda bisa menerima kesalahan ini jika pesan dirutekan melalui layanan pihak ketiga.</span><span class="sxs-lookup"><span data-stu-id="52701-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="52701-110">Anda dapat menggunakan alat pencarian WHOIS untuk menemukan pemilik alamat IP yang diblokir.</span><span class="sxs-lookup"><span data-stu-id="52701-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
