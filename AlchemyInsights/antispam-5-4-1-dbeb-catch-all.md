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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672436"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Memperbaiki masalah pengiriman kode galat 550 5.4.1 akses relay ditolak

Masalah ini terjadi saat [memeriksa untuk melihat jika alamat email yang valid untuk mencegah bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) saat memasuki jaringan 365 Office. Coba langkah berikut:

1. Tentukan apakah masalah khusus untuk seluruh domain atau satu alamat email:
    - Seluruh domain: terkadang domain perlu disinkronkan; Coba [Atur domain ke internal dan kemudian kembali ke otoritatif](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Alamat email tunggal: terkadang alamat harus disinkronkan; mengubah alamat SMTP proxy dan kemudian mengubahnya kembali dapat membantu.
2. Tentukan apakah masalah khusus untuk grup atau folder publik. Untuk beberapa jenis objek, objek mungkin perlu secara manual dibuat di Azure Active Directory.

Jika Anda memerlukan bantuan tambahan, silakan buka tiket dukungan dan menentukan lingkup masalah (includidng jenis objek yang Anda kirim ke) sehingga kami dapat membantu Anda lebih baik.