---
title: AntiSpam 5.4.1 DBEB menangkap-semua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707914"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="5a5b1-102">Memperbaiki masalah pengiriman kode galat 550 5.4.1 akses relay ditolak</span><span class="sxs-lookup"><span data-stu-id="5a5b1-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="5a5b1-103">Masalah ini terjadi saat [memeriksa untuk melihat jika alamat email yang valid untuk mencegah bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ketika memasuki jaringan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5a5b1-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="5a5b1-104">Coba langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="5a5b1-104">Try the following:</span></span>

1. <span data-ttu-id="5a5b1-105">Tentukan apakah masalah khusus untuk seluruh domain atau satu alamat email:</span><span class="sxs-lookup"><span data-stu-id="5a5b1-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="5a5b1-106">Seluruh domain: terkadang domain perlu disinkronkan; Coba [Atur domain ke internal dan kemudian kembali ke otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="5a5b1-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="5a5b1-107">Alamat email tunggal: terkadang alamat harus disinkronkan; mengubah alamat SMTP proxy dan kemudian mengubahnya kembali dapat membantu.</span><span class="sxs-lookup"><span data-stu-id="5a5b1-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="5a5b1-108">Tentukan apakah masalah khusus untuk grup atau folder publik.</span><span class="sxs-lookup"><span data-stu-id="5a5b1-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="5a5b1-109">Untuk beberapa jenis objek, objek mungkin perlu secara manual dibuat di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5a5b1-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="5a5b1-110">Jika Anda memerlukan bantuan tambahan, silakan buka tiket dukungan dan tentukan cakupan masalah (termasuk jenis objek yang Anda kirim ke) sehingga kami dapat membantu Anda dengan lebih baik.</span><span class="sxs-lookup"><span data-stu-id="5a5b1-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>