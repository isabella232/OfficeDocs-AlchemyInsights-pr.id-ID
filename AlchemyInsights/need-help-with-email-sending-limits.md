---
title: Butuh bantuan dengan batas pengiriman email?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357865"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="97f61-102">Butuh bantuan dengan batas pengiriman email?</span><span class="sxs-lookup"><span data-stu-id="97f61-102">Need help with email sending limits?</span></span>

<span data-ttu-id="97f61-103">Di bawah ini adalah **batas pengiriman oleh-desain** yang diberlakukan dalam layanan.</span><span class="sxs-lookup"><span data-stu-id="97f61-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="97f61-104">Informasi lebih lanjut tentang batas ini didokumentasikan [di sini](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="97f61-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="97f61-105">Untuk mencegah pengiriman pesan massal yang tidak diinginkan, kami menerapkan batas penerima per pengguna **untuk semua pesan keluar dan internal**.</span><span class="sxs-lookup"><span data-stu-id="97f61-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="97f61-106">Di semua SKU, batas ini adalah **10.000 Penerima per hari**.</span><span class="sxs-lookup"><span data-stu-id="97f61-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="97f61-107">Pelanggan yang perlu mengirimkan email komersial massal yang sah (misalnya, buletin pelanggan) harus menggunakan penyedia pihak ketiga yang mengkhususkan diri pada layanan ini.</span><span class="sxs-lookup"><span data-stu-id="97f61-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="97f61-108">**Catatan**: setelah batas penerima tercapai, pesan tidak dapat dikirim dari kotak pesan hingga jumlah penerima yang dikirimi pesan dalam 24 jam terakhir turun di bawah batas.</span><span class="sxs-lookup"><span data-stu-id="97f61-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="97f61-109">Pengguna tidak akan dapat mengirim pesan sampai titik tersebut.</span><span class="sxs-lookup"><span data-stu-id="97f61-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="97f61-110">Batas tingkat pesan **30 pesan per menit** diterapkan di semua SKU.</span><span class="sxs-lookup"><span data-stu-id="97f61-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="97f61-111">Ini menentukan berapa banyak pesan yang dapat dikirim pengguna dari akun Exchange Online mereka dalam jangka waktu tertentu.</span><span class="sxs-lookup"><span data-stu-id="97f61-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="97f61-112">**Jumlah maksimum penerima yang diizinkan di bidang kepada, cc, dan BCC** untuk satu pesan email, di semua SKU, adalah **1000 Penerima**.</span><span class="sxs-lookup"><span data-stu-id="97f61-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="97f61-113">Untuk menyesuaikan batas ini, buka [di sini](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="97f61-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
