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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823970"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="ac39d-102">Tidak dapat mengatur alamat email utama, mengubah atribut pengguna, atau menghapus/menghapus pengguna yang disinkronkan</span><span class="sxs-lookup"><span data-stu-id="ac39d-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="ac39d-103">Jika sinkronisasi direktori diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak dapat diubah menggunakan pusat admin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ac39d-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="ac39d-104">Untuk mengelola semua atribut dan pengguna yang disinkronkan sepenuhnya, gunakan pengguna direktori aktif lokal dan konsol manajemen grup (adsiedit.msc) Anda.</span><span class="sxs-lookup"><span data-stu-id="ac39d-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="ac39d-105">Alternatifnya, Anda bisa mengubah pengguna atau atribut individual untuk pengguna yang disinkronkan menggunakan powershell seperti yang diperlihatkan dalam contoh umum ini:</span><span class="sxs-lookup"><span data-stu-id="ac39d-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
