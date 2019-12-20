---
title: Tim 4c7 kesalahan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796184"
---
# <a name="4c7-error-in-microsoft-teams"></a>galat 4c7 di Microsoft teams

Galat ini terjadi karena Microsoft teams memerlukan otentikasi formulir. Ketika Anda menggunakan Active Directory Federation Services (AD FS), otentikasi formulir tidak diaktifkan untuk intranet secara default. Jika otentikasi Terpadu Windows gagal, Anda diminta untuk masuk menggunakan otentikasi formulir.

Untuk mengatasi masalah ini, aktifkan otentikasi formulir dengan menggunakan AD FS konsol manajemen Microsoft (MMC) snap-in di komputer yang memiliki salinan lokal direktori aktif. Untuk melakukan ini, ikuti langkah berikut: 

1. Di panel navigasi, Jelajahi **kebijakan otentikasi**.
2. Di bawah **tindakan** di panel rincian, pilih **mengedit otentikasi utama global**.
3. Pada tab **intranet** , pilih **bentuk otentikasi**.
4. Pilih **OK** (atau **Terapkan**).