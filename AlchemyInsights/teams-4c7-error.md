---
title: Kesalahan Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786672"
---
# <a name="4c7-error-in-microsoft-teams"></a>Kesalahan 4c7 di Microsoft Teams

Kesalahan ini terjadi karena Microsoft Teams memerlukan Autentikasi Forms. Ketika Anda menggunakan Active Directory Federation Services (AD FS), Autentikasi Formulir tidak diaktifkan untuk intranet secara default. Jika Autentikasi Terpadu Windows gagal, Anda akan diminta untuk masuk menggunakan Autentikasi Forms.

Untuk mengatasi masalah ini, aktifkan Autentikasi Forms dengan menggunakan snap-in KONSOL Manajemen Microsoft (MMC) AD FS di komputer yang memiliki salinan lokal Direktori Aktif. Untuk melakukan ini, ikuti langkah berikut: 

1. Di panel navigasi, telusuri ke **Kebijakan Autentikasi.**
2. Di **bawah Tindakan** di panel detail, pilih Edit **Autentikasi Utama Global.**
3. Pada tab **Intranet,** pilih **Autentikasi Formulir**.
4. Pilih **OK** (atau **Terapkan**).