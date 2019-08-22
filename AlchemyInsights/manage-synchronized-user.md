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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="7f141-102">Mampu mengatur alamat email utama atau mengubah atribut pengguna</span><span class="sxs-lookup"><span data-stu-id="7f141-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="7f141-103">Jika bantu directory synchronization diaktifkan untuk lingkungan Anda, beberapa atribut pengguna atau objek tidak dapat diubah menggunakan Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="7f141-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="7f141-104">Untuk sepenuhnya mengelola disinkronisasi pengguna dan semua atribut mereka, menggunakan direktori aktif lokal pengguna dan grup manajemen konsol Anda (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="7f141-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="7f141-105">Atau, Anda dapat mengubah pengguna individu atau atribut untuk disinkronisasi pengguna menggunakan powershell seperti ditunjukkan dalam contoh-contoh umum ini:</span><span class="sxs-lookup"><span data-stu-id="7f141-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="7f141-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7f141-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="7f141-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Pengguna uji" - LastName "Pengguna"-jabatan "Manajer"-Departemen "SDM"</span><span class="sxs-lookup"><span data-stu-id="7f141-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="7f141-108">Hapus-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7f141-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>