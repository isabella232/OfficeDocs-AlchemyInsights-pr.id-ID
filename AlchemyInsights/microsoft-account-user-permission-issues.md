---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768804"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Memecahkan masalah-pengguna tidak ditemukan di direktori

Jika pengguna menerima pesan galat "pengguna tidak dapat ditemukan" di dalam direktori, silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.

Langkah berikut ini dapat diselesaikan untuk memecahkan masalah.

- Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti. Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs. 

Untuk informasi lebih lanjut, lihat [cara mengelola alias untuk</a> akun Microsoft Anda untuk mengelola kantor 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Browse ke setiap situs (s) di mana pengguna menerima galat. 

Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (dalam tanda kutip ganda) ke akhir URL situs. 

Contoh: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pilih pengguna dari daftar.

- Klik **Hapus izin pengguna** dari pita. 
-  Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.

