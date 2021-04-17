---
title: Catch-all DBEB 5.4.1 AntiSpam 5.4.1
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821450"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ffff2-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="ffff2-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ffff2-103">Masalah ini terjadi [ketika memeriksa apakah alamat email valid untuk mencegah pantulan](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ketika masuk ke jaringan Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ffff2-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ffff2-104">Cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="ffff2-104">Try the following:</span></span>

1. <span data-ttu-id="ffff2-105">Tentukan apakah masalah ber spesifik untuk seluruh domain atau satu alamat email:</span><span class="sxs-lookup"><span data-stu-id="ffff2-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ffff2-106">Seluruh domain: Terkadang domain perlu disinkronkan; coba [pengaturan domain untuk Internal lalu kembali ke Otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ffff2-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ffff2-107">Satu alamat email: Terkadang alamat perlu disinkronkan; mengubah alamat proksi smtp lalu mengubahnya kembali bisa membantu.</span><span class="sxs-lookup"><span data-stu-id="ffff2-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ffff2-108">Tentukan apakah masalah ber spesifik untuk grup atau folder publik.</span><span class="sxs-lookup"><span data-stu-id="ffff2-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ffff2-109">Untuk beberapa tipe objek, objek mungkin harus dibuat secara manual di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ffff2-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ffff2-110">Jika membutuhkan bantuan tambahan, silakan buka tiket dukungan dan tentukan lingkup masalah (termasuk tipe objek yang Anda kirimi) agar kami dapat membantu Anda dengan lebih baik.</span><span class="sxs-lookup"><span data-stu-id="ffff2-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>