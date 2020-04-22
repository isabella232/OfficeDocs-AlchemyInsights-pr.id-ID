---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702741"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d1623-102">Memecahkan masalah-pengguna tidak ditemukan di direktori</span><span class="sxs-lookup"><span data-stu-id="d1623-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d1623-103">Jika pengguna menerima pesan galat "pengguna tidak dapat ditemukan" di dalam direktori, silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.</span><span class="sxs-lookup"><span data-stu-id="d1623-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d1623-104">Langkah berikut ini dapat diselesaikan untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="d1623-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d1623-105">Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti.</span><span class="sxs-lookup"><span data-stu-id="d1623-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d1623-106">Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs.</span><span class="sxs-lookup"><span data-stu-id="d1623-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d1623-107">Untuk informasi lebih lanjut, lihat [cara mengelola alias untuk</a> akun Microsoft Anda untuk mengelola Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="d1623-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d1623-108">Browse ke setiap situs (s) di mana pengguna menerima galat.</span><span class="sxs-lookup"><span data-stu-id="d1623-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d1623-109">Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (dalam tanda kutip ganda) ke akhir URL situs.</span><span class="sxs-lookup"><span data-stu-id="d1623-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d1623-110">Contoh: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="d1623-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d1623-111">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="d1623-111">Select the user from the list.</span></span>

- <span data-ttu-id="d1623-112">Klik **Hapus izin pengguna** dari pita.</span><span class="sxs-lookup"><span data-stu-id="d1623-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d1623-113">Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="d1623-113">Add back the User and Resend the invite to the user.</span></span>

