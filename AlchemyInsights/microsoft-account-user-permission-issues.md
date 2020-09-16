---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725410"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="8cf64-102">Memecahkan masalah-pengguna tidak ditemukan di direktori</span><span class="sxs-lookup"><span data-stu-id="8cf64-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="8cf64-103">Jika pengguna menerima pesan kesalahan "pengguna tidak dapat ditemukan" di direktori, coba lagi di mana tipe masalah adalah pengguna tidak ada di direktori.</span><span class="sxs-lookup"><span data-stu-id="8cf64-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="8cf64-104">Langkah-langkah berikut ini bisa diselesaikan untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="8cf64-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="8cf64-105">Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti.</span><span class="sxs-lookup"><span data-stu-id="8cf64-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="8cf64-106">Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs.</span><span class="sxs-lookup"><span data-stu-id="8cf64-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="8cf64-107">Untuk informasi selengkapnya, lihat [cara mengelola alias untuk akun Microsoft Anda </a> untuk mengelola masuk Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="8cf64-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="8cf64-108">Telusuri ke setiap situs tempat pengguna menerima kesalahan.</span><span class="sxs-lookup"><span data-stu-id="8cf64-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="8cf64-109">Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (di dalam tanda kutip ganda) ke bagian akhir URL situs.</span><span class="sxs-lookup"><span data-stu-id="8cf64-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="8cf64-110">Contoh: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="8cf64-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="8cf64-111">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="8cf64-111">Select the user from the list.</span></span>

- <span data-ttu-id="8cf64-112">Klik **Hapus izin pengguna** dari pita.</span><span class="sxs-lookup"><span data-stu-id="8cf64-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="8cf64-113">Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="8cf64-113">Add back the User and Resend the invite to the user.</span></span>

