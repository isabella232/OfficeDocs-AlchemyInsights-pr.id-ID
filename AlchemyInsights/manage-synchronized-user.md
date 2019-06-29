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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="cec19-102">Mampu mengatur alamat email utama atau mengubah atribut pengguna</span><span class="sxs-lookup"><span data-stu-id="cec19-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="cec19-103">Jika bantu directory synchronization diaktifkan untuk lingkungan Anda beberapa atribut pengguna atau objek tidak dapat diubah menggunakan Admin Center.</span><span class="sxs-lookup"><span data-stu-id="cec19-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="cec19-104">Untuk sepenuhnya mengelola disinkronisasi pengguna dan semua atribut mereka, menggunakan direktori aktif lokal pengguna dan grup manajemen konsol Anda (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="cec19-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="cec19-105">Atau, Anda dapat mengubah pengguna individu atau atribut untuk disinkronisasi pengguna menggunakan powershell seperti ditunjukkan dalam contoh-contoh umum ini:</span><span class="sxs-lookup"><span data-stu-id="cec19-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="cec19-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cec19-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="cec19-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Pengguna uji" - LastName "Pengguna"-jabatan "Manajer"-Departemen "SDM"</span><span class="sxs-lookup"><span data-stu-id="cec19-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="cec19-108">Hapus-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cec19-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>