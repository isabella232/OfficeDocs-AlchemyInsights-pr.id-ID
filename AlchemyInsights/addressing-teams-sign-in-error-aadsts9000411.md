---
title: Menangani Teams masuk AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953030"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Menangani Teams masuk AADSTS9000411

Ketika masuk ke Microsoft Teams, Anda mungkin menerima kesalahan: Maaf, tetapi kami mengalami masalah dengan penandatanganan Anda di **AADSTS9000411: Permintaan tidak diformat dengan benar. Parameter "login_hint" diduplikasi.**

Untuk mengatasi masalah ini, pastikan klien Microsoft Teams Anda diperbarui. Untuk informasi selengkapnya tentang memperbarui klien Anda, lihat [Memperbarui Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Jika Anda tidak bisa memperbarui klien Anda karena beberapa alasan, keluar dari klien akan menghapus sebagian besar data singgahan. Namun, jika Anda masih mengalami masalah setelah logoff/masuk, keluar Teams dan kosongkan cache klien Anda dengan melakukan hal berikut:
1. Tutup Microsoft Teams.
2. Masuk ke: %appdata%\microsoft\teams dan hapus semua file.
3. Buka Microsoft Teams kembali.
