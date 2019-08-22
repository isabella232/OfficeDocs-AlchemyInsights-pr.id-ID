---
title: Mengelola disinkronisasi pengguna
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541999"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Mampu mengatur alamat email utama atau mengubah atribut pengguna

Jika bantu directory synchronization diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak dapat diubah menggunakan Microsoft 365 admin center.

Untuk sepenuhnya mengelola disinkronisasi pengguna dan semua atribut mereka, menggunakan direktori aktif lokal pengguna dan grup manajemen konsol Anda (adsiedit.msc).  

Atau, Anda dapat mengubah pengguna individu atau atribut untuk disinkronisasi pengguna menggunakan powershell seperti ditunjukkan dalam contoh-contoh umum ini: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Pengguna uji" - LastName "Pengguna"-jabatan "Manajer"-Departemen "SDM"
- Hapus-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com