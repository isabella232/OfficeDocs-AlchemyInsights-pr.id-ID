---
title: Anti spam 5.4.1 DBEB Catch-All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717364"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="fc455-102">Memperbaiki masalah pengiriman untuk kode kesalahan 550 5.4.1 relay Access ditolak</span><span class="sxs-lookup"><span data-stu-id="fc455-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="fc455-103">Masalah ini terjadi ketika [memeriksa untuk melihat apakah alamat email valid untuk mencegah bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) saat memasukkan jaringan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fc455-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="fc455-104">Cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="fc455-104">Try the following:</span></span>

1. <span data-ttu-id="fc455-105">Tentukan apakah masalah spesifik untuk seluruh domain atau satu alamat email:</span><span class="sxs-lookup"><span data-stu-id="fc455-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="fc455-106">Seluruh domain: terkadang domain perlu disinkronkan; Coba [Atur domain ke internal lalu kembali ke otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="fc455-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="fc455-107">Alamat email tunggal: terkadang alamat perlu disinkronkan; mengubah alamat proksi SMTP lalu mengubahnya kembali bisa membantu.</span><span class="sxs-lookup"><span data-stu-id="fc455-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="fc455-108">Menentukan apakah masalah tersebut spesifik untuk grup atau folder publik.</span><span class="sxs-lookup"><span data-stu-id="fc455-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="fc455-109">Untuk beberapa tipe objek, objek mungkin harus dibuat secara manual di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc455-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="fc455-110">Jika Anda memerlukan bantuan tambahan, silakan buka tiket dukungan dan tentukan lingkup masalah (termasuk tipe objek yang Anda kirim) agar kami bisa membantu Anda lebih baik.</span><span class="sxs-lookup"><span data-stu-id="fc455-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>