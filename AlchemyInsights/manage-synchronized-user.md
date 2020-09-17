---
title: Mengelola pengguna yang disinkronkan
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777680"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Tidak dapat mengatur alamat email utama, mengubah atribut pengguna, atau menghapus/menghapus pengguna yang disinkronkan

Jika sinkronisasi direktori diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak bisa diubah menggunakan pusat admin Microsoft 365.

Untuk sepenuhnya mengelola pengguna yang disinkronkan dan semua atributnya, gunakan Active Directory lokal dan konsol manajemen grup (ADSIEDIT. MSC).  

Alternatifnya, Anda bisa mengubah pengguna atau atribut individual untuk pengguna yang disinkronkan menggunakan PowerShell seperti yang diperlihatkan dalam contoh umum ini: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
