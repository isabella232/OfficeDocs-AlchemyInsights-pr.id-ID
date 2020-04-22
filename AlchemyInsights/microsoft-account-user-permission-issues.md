---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702741"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Memecahkan masalah-pengguna tidak ditemukan di direktori

Jika pengguna menerima pesan galat "pengguna tidak dapat ditemukan" di dalam direktori, silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.

Langkah berikut ini dapat diselesaikan untuk memecahkan masalah.

- Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti. Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs. 

Untuk informasi lebih lanjut, lihat [cara mengelola alias untuk</a> akun Microsoft Anda untuk mengelola Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Browse ke setiap situs (s) di mana pengguna menerima galat. 

Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (dalam tanda kutip ganda) ke akhir URL situs. 

Contoh: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pilih pengguna dari daftar.

- Klik **Hapus izin pengguna** dari pita. 
-  Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.

