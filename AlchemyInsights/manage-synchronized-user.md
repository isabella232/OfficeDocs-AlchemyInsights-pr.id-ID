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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380508"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Mampu mengatur alamat email utama atau mengubah atribut pengguna

Jika bantu directory synchronization diaktifkan untuk lingkungan Anda beberapa atribut pengguna atau objek tidak dapat diubah menggunakan Admin Center.
Untuk sepenuhnya mengelola disinkronisasi pengguna dan semua atribut mereka, menggunakan direktori aktif lokal pengguna dan grup manajemen konsol Anda (adsiedit.msc).  

Atau, Anda dapat mengubah pengguna individu atau atribut untuk disinkronisasi pengguna menggunakan powershell seperti ditunjukkan dalam contoh-contoh umum ini: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Pengguna uji" - LastName "Pengguna"-jabatan "Manajer"-Departemen "SDM"
- Hapus-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com