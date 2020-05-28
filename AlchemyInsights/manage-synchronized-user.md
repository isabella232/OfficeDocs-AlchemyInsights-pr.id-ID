---
title: Kelola pengguna yang disinkronkan
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407353"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Tidak dapat menetapkan alamat email utama, mengubah atribut pengguna, atau menghapus/menghapus pengguna disinkronkan

Jika sinkronisasi direktori diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak dapat diubah menggunakan Microsoft 365 Admin Center.

Untuk sepenuhnya mengelola disinkronkan pengguna dan semua atribut mereka, gunakan pengguna direktori aktif lokal dan grup konsol manajemen (ADSIEDIT. MSC).  

Atau, Anda dapat mengubah masing-masing pengguna atau atribut untuk disinkronkan pengguna menggunakan PowerShell seperti yang ditunjukkan dalam contoh umum ini: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
