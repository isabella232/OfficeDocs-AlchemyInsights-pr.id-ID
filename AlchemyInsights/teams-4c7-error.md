---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049311"
---
# <a name="4c7-error-in-microsoft-teams"></a>Kesalahan 4c7 di Microsoft Teams

Kesalahan ini terjadi karena Microsoft Teams memerlukan Autentikasi Formulir. Ketika Anda menggunakan Active Directory Federation Services (AD FS), Autentikasi Formulir tidak diaktifkan untuk intranet secara default. Jika Windows Autentikasi Terpadu gagal, Anda akan diminta untuk masuk menggunakan Autentikasi Forms.

Untuk mengatasi masalah ini, aktifkan Autentikasi Forms dengan menggunakan snap-in KONSOL Manajemen Microsoft (MMC) AD FS di komputer yang memiliki salinan lokal Direktori Aktif. Untuk melakukan ini, ikuti langkah berikut: 

1. Di panel navigasi, telusuri ke **Kebijakan Autentikasi.**
2. Di **bawah Tindakan** di panel detail, pilih Edit **Autentikasi Utama Global.**
3. Pada tab **Intranet,** pilih **Autentikasi Formulir**.
4. Pilih **OK** (atau **Terapkan**).