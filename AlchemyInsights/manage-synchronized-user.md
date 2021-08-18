---
title: Mengelola Pengguna yang Disinkronkan
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114781"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Tidak dapat mengatur alamat email utama, mengubah atribut pengguna, atau menghapus/menghapus pengguna yang disinkronkan

Jika sinkronisasi direktori diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak dapat diubah menggunakan pusat admin Microsoft 365.

Untuk mengelola semua atribut dan pengguna yang disinkronkan sepenuhnya, gunakan pengguna direktori aktif lokal dan konsol manajemen grup (adsiedit.msc) Anda.  

Alternatifnya, Anda bisa mengubah pengguna atau atribut individual untuk pengguna yang disinkronkan menggunakan powershell seperti yang diperlihatkan dalam contoh umum ini:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
