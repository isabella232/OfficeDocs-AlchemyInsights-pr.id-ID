---
title: Memecahkan masalah-pengguna tidak ditemukan di direktori
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754195"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="c00bf-102">Memecahkan masalah-pengguna tidak ditemukan di direktori</span><span class="sxs-lookup"><span data-stu-id="c00bf-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="c00bf-103">Jika pengguna menerima pesan galat "pengguna tidak dapat ditemukan" di dalam direktori.</span><span class="sxs-lookup"><span data-stu-id="c00bf-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="c00bf-104">Silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.</span><span class="sxs-lookup"><span data-stu-id="c00bf-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="c00bf-105">Langkah berikut ini dapat diselesaikan untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="c00bf-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="c00bf-106">Pastikan akun yang menerima undangan email adalah akun yang sama yang digunakan untuk masuk nanti.</span><span class="sxs-lookup"><span data-stu-id="c00bf-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="c00bf-107">Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs.</span><span class="sxs-lookup"><span data-stu-id="c00bf-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="c00bf-108">Untuk informasi lebih lanjut, lihat [cara mengelola alias untuk</a> akun Microsoft Anda untuk mengelola kantor 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="c00bf-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="c00bf-109">Browse ke setiap situs (s) di mana pengguna menerima galat.</span><span class="sxs-lookup"><span data-stu-id="c00bf-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="c00bf-110">Tambahkan "/_layouts/15/People.aspx/membershipgroupid = 0" (dalam tanda kutip ganda) ke akhir URL situs.</span><span class="sxs-lookup"><span data-stu-id="c00bf-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="c00bf-111">Contoh: https://_ lt_ "contoso">. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="c00bf-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="c00bf-112">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="c00bf-112">Select the user from the list.</span></span>

- <span data-ttu-id="c00bf-113">Klik **Hapus izin pengguna** dari pita.</span><span class="sxs-lookup"><span data-stu-id="c00bf-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="c00bf-114">Tambahkan kembali pengguna dan kirim ulang undangan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="c00bf-114">Add back the User and Resend the invite to the user.</span></span>

