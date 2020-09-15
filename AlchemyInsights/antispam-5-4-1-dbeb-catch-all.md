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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Memperbaiki masalah pengiriman untuk kode kesalahan 550 5.4.1 relay Access ditolak

Masalah ini terjadi ketika [memeriksa untuk melihat apakah alamat email valid untuk mencegah bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) saat memasukkan jaringan Microsoft. Cobalah hal berikut:

1. Tentukan apakah masalah spesifik untuk seluruh domain atau satu alamat email:
    - Seluruh domain: terkadang domain perlu disinkronkan; Coba [Atur domain ke internal lalu kembali ke otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Alamat email tunggal: terkadang alamat perlu disinkronkan; mengubah alamat proksi SMTP lalu mengubahnya kembali bisa membantu.
2. Menentukan apakah masalah tersebut spesifik untuk grup atau folder publik. Untuk beberapa tipe objek, objek mungkin harus dibuat secara manual di Azure Active Directory.

Jika Anda memerlukan bantuan tambahan, silakan buka tiket dukungan dan tentukan lingkup masalah (termasuk tipe objek yang Anda kirim) agar kami bisa membantu Anda lebih baik.