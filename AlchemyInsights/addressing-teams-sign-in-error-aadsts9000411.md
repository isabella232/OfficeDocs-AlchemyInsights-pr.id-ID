---
title: Mengatasi kesalahan masuk Teams AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821990"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Mengatasi kesalahan masuk Teams AADSTS9000411

Ketika masuk ke Microsoft Teams, Anda mungkin akan menerima kesalahan: Maaf, tetapi kami mengalami masalah dengan penandatanganan Anda di **AADSTS9000411: Permintaan tidak diformat dengan benar. Parameter "login_hint" diduplikasi.**

Untuk mengatasi masalah ini, pastikan klien Microsoft Teams Anda diperbarui. Untuk informasi selengkapnya tentang memperbarui klien, lihat [Memperbarui Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Jika Anda tidak bisa memperbarui klien Anda karena beberapa alasan, keluar dari klien akan menghapus sebagian besar data singgahan. Namun, jika masih mengalami masalah setelah logoff/masuk, keluar dari Teams dan hapus cache klien dengan melakukan hal berikut:
1. Tutup Microsoft Teams.
2. Masuk ke: %appdata%\microsoft\teams dan hapus semua file.
3. Buka kembali Microsoft Teams.
