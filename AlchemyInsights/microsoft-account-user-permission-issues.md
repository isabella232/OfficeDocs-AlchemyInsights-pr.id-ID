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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754195"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Memecahkan masalah-pengguna tidak ditemukan di direktori

Jika pengguna menerima pesan galat "pengguna tidak dapat ditemukan" di dalam direktori. Silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.

Langkah berikut ini dapat diselesaikan untuk memecahkan masalah.

- Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti. Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs. 

Untuk informasi lebih lanjut, lihat [cara mengelola alias untuk</a> akun Microsoft Anda untuk mengelola kantor 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Browse ke setiap situs (s) di mana pengguna menerima galat. 

Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (dalam tanda kutip ganda) ke akhir URL situs. 

Contoh: https://_ lt_ "contoso">. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.

- Pilih pengguna dari daftar.

- Klik **Hapus izin pengguna** dari pita. 
-  Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.

