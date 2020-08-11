---
title: Add-in teams untuk Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629659"
---
# <a name="teams-add-in-for-mac"></a>Add-in teams untuk Mac

Untuk memecahkan masalah Add-in tim yang hilang untuk pengguna sistem operasi Mac, ikuti langkah-langkah berikut:

**Langkah 1:** Jika Anda memiliki Exchange hibrid di tempat (2016 CU3 atau yang lebih baru diperlukan), gunakan alat Test-HMA.ps1 untuk mengonfirmasi bahwa autentikasi modern hibrid dikonfigurasikan dengan benar. Untuk informasi selengkapnya, lihat [memvalidasi penyiapan autentikasi modern hibrid untuk Outlook untuk IOS dan Android](https://aka.ms/AA980zq).  

**Catatan** Gunakan format alamat UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)), bukan domain\username. Lakukan ini bahkan untuk pengguna dengan kotak surat Exchange Online.

**Langkah 2:** Minta pengguna masuk ke akun **alat**  >  **Accounts**... di Outlook untuk Mac, dan temukan dan pilih akun. Konfirmasi nama pengguna yang tercantum dalam format UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)).

**Langkah 3:** Konfirmasi pengguna adalah pengguna Microsoft teams berlisensi. Pengguna harus menggunakan langganan Office 365 untuk Mac, produk versi 16,24 atau yang lebih baru.