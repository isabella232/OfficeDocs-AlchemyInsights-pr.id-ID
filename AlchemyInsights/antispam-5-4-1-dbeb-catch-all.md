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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix delivery issues for error code 550 5.4.1 Relay Access Denied

Masalah ini terjadi [ketika memeriksa apakah alamat email valid untuk mencegah pantulan](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ketika masuk ke jaringan Microsoft. Cobalah hal berikut:

1. Tentukan apakah masalah ber spesifik untuk seluruh domain atau satu alamat email:
    - Seluruh domain: Terkadang domain perlu disinkronkan; coba [pengaturan domain untuk Internal lalu kembali ke Otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Satu alamat email: Terkadang alamat perlu disinkronkan; mengubah alamat proksi smtp lalu mengubahnya kembali bisa membantu.
2. Tentukan apakah masalah ber spesifik untuk grup atau folder publik. Untuk beberapa tipe objek, objek mungkin harus dibuat secara manual di Azure Active Directory.

Jika membutuhkan bantuan tambahan, silakan buka tiket dukungan dan tentukan lingkup masalah (termasuk tipe objek yang Anda kirimi) agar kami dapat membantu Anda dengan lebih baik.