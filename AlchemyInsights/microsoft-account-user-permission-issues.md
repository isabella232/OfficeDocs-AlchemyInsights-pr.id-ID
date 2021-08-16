---
title: Memecahkan masalah - Pengguna tidak ditemukan dalam direktori
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098173"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Memecahkan masalah - Pengguna tidak ditemukan dalam direktori

Jika pengguna menerima pesan kesalahan "pengguna tidak dapat ditemukan" di direktori, silakan coba lagi di mana Tipe Masalah adalah Pengguna yang tidak berada dalam direktori.

Langkah-langkah berikut ini dapat diselesaikan untuk memecahkan masalah tersebut.

- Pastikan akun yang menerima undangan email adalah akun yang digunakan untuk masuk nanti. Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs. 

Untuk informasi selengkapnya, [lihat Cara mengelola alias untuk akun Microsoft Anda untuk mengelola Microsoft 365 </a> masuk.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Telusuri ke setiap situs di mana pengguna menerima kesalahan. 

Tambahkan "/_layouts/15/people.aspx/membershipgroupid=0" (dalam tanda kutip ganda) ke akhir URL situs. 

Contoh: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pilih pengguna dari daftar.

- Klik **Hapus Izin Pengguna** dari Pita. 
-  Tambahkan kembali Pengguna dan Kirim ulang undangan kepada pengguna.

