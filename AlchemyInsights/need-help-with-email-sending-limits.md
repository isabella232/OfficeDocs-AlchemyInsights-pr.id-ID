---
title: Perlu bantuan tentang batas pengiriman email?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836282"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="f9b19-102">Perlu bantuan tentang batas pengiriman email?</span><span class="sxs-lookup"><span data-stu-id="f9b19-102">Need help with email sending limits?</span></span>

<span data-ttu-id="f9b19-103">Berikut adalah **batas pengiriman berdasarkan desain** yang diterapkan dalam layanan.</span><span class="sxs-lookup"><span data-stu-id="f9b19-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="f9b19-104">Informasi selengkapnya tentang batas ini didokumentasikan [di sini](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="f9b19-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="f9b19-105">Untuk mencegah pengiriman pesan massal yang tidak diminta, kami menerapkan **batas tarif penerima per pengguna untuk semua pesan keluar dan internal**.</span><span class="sxs-lookup"><span data-stu-id="f9b19-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="f9b19-106">Di semua SKU, batasnya adalah **10.000 penerima per hari**.</span><span class="sxs-lookup"><span data-stu-id="f9b19-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="f9b19-107">Pelanggan yang perlu mengirim email komersial massal yang sah (misalnya, buletin pelanggan) harus menggunakan penyedia pihak ketiga yang berspesialisasi dalam layanan ini.</span><span class="sxs-lookup"><span data-stu-id="f9b19-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="f9b19-108">**Catatan**: Setelah batas tarif penerima tercapai, pesan tidak dapat dikirim dari kotak surat hingga jumlah penerima yang dikirimi pesan dalam 24 jam terakhir turun di bawah batas.</span><span class="sxs-lookup"><span data-stu-id="f9b19-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="f9b19-109">Pengguna tidak akan dapat mengirim pesan hingga titik tersebut.</span><span class="sxs-lookup"><span data-stu-id="f9b19-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="f9b19-110">Batas kecepatan pesan **30 pesan per menit** diterapkan di semua SKU.</span><span class="sxs-lookup"><span data-stu-id="f9b19-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="f9b19-111">Hal ini menentukan berapa banyak pesan yang dapat dikirim pengguna dari akun Exchange Online mereka dalam jangka waktu tertentu.</span><span class="sxs-lookup"><span data-stu-id="f9b19-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="f9b19-112">**Jumlah maksimum penerima yang diizinkan dalam bidang Kepada, Cc, dan Bcc** untuk satu pesan email, di semua SKU, adalah **1000 penerima**.</span><span class="sxs-lookup"><span data-stu-id="f9b19-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="f9b19-113">Untuk menyesuaikan batas ini, buka [di sini](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="f9b19-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
