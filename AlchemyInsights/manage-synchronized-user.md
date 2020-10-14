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
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451403"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Tidak dapat mengatur alamat email utama, mengubah atribut pengguna, atau menghapus/menghapus pengguna yang disinkronkan

Jika sinkronisasi direktori diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak bisa diubah menggunakan pusat admin Microsoft 365.

Untuk sepenuhnya mengelola pengguna yang disinkronkan dan semua atributnya, gunakan Active Directory lokal dan konsol manajemen grup (ADSIEDIT. MSC).  

Alternatifnya, Anda bisa mengubah pengguna atau atribut individual untuk pengguna yang disinkronkan menggunakan PowerShell seperti yang diperlihatkan dalam contoh umum ini:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
