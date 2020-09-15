---
title: Kesalahan teams 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700206"
---
# <a name="4c7-error-in-microsoft-teams"></a>kesalahan 4c7 di Microsoft teams

Kesalahan ini terjadi karena Microsoft teams memerlukan autentikasi formulir. Saat Anda menggunakan Active Directory Federation Services (AD FS), autentikasi formulir tidak diaktifkan untuk intranet secara default. Jika autentikasi Terpadu Windows gagal, Anda akan diminta untuk masuk menggunakan autentikasi formulir.

Untuk mengatasi masalah ini, Aktifkan autentikasi formulir dengan menggunakan snap-in konsol manajemen Microsoft (MMC) AD FS di komputer yang memiliki salinan direktori aktif lokal. Untuk melakukan ini, ikuti langkah berikut: 

1. Di panel navigasi, telusuri ke **kebijakan autentikasi**.
2. Di bawah **tindakan** di panel detail, pilih **Edit autentikasi utama global**.
3. Pada tab **intranet** , pilih **autentikasi formulir**.
4. Pilih **OK** (atau **Terapkan**).