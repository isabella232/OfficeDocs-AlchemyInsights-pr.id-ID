---
title: Mengatasi kesalahan tim sign-in AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357878"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Mengatasi kesalahan tim sign-in AADSTS9000411

Saat masuk ke Microsoft teams, Anda mungkin menerima pesan kesalahan: **Maaf, namun kami mengalami masalah saat masuk ke AADSTS9000411: permintaan tidak diformat dengan benar. Parameter "login_hint" diduplikasi.**

Untuk mengatasi masalah ini, pastikan klien Microsoft teams Anda diperbarui. Untuk informasi lebih lanjut tentang cara memperbarui klien, lihat [memperbarui Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Jika Anda tidak dapat memperbarui klien Anda untuk beberapa alasan, logoff klien akan menghapus sebagian besar data yang disimpan dalam cache. Namun, jika Anda masih mengalami masalah setelah logoff/logon, tutup tim dan Kosongkan tembolok klien Anda dengan melakukan hal berikut:
1. Tutup Microsoft teams.
2. Pergi ke:%AppData%\microsoft\teams dan menghapus semua berkas.
3. Buka kembali Microsoft teams.
