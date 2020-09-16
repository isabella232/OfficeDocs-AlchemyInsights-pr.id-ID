---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725410"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Memecahkan masalah-pengguna tidak ditemukan di direktori

Jika pengguna menerima pesan kesalahan "pengguna tidak dapat ditemukan" di direktori, coba lagi di mana tipe masalah adalah pengguna tidak ada di direktori.

Langkah-langkah berikut ini bisa diselesaikan untuk memecahkan masalah.

- Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti. Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs. 

Untuk informasi selengkapnya, lihat [cara mengelola alias untuk akun Microsoft Anda </a> untuk mengelola masuk Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Telusuri ke setiap situs tempat pengguna menerima kesalahan. 

Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (di dalam tanda kutip ganda) ke bagian akhir URL situs. 

Contoh: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pilih pengguna dari daftar.

- Klik **Hapus izin pengguna** dari pita. 
-  Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.

