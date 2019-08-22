---
title: Memecahkan masalah - pengguna tidak ditemukan dalam direktori
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544866"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="09976-102">Memecahkan masalah - pengguna tidak ditemukan dalam direktori</span><span class="sxs-lookup"><span data-stu-id="09976-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="09976-103">Jika pengguna menerima kesalahan pesan "user tidak dapat ditemukan" dalam direktori.</span><span class="sxs-lookup"><span data-stu-id="09976-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="09976-104">Silakan coba lagi di mana jenis masalah adalah pengguna tidak dalam direktori.</span><span class="sxs-lookup"><span data-stu-id="09976-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="09976-105">Langkah-langkah berikut dapat diselesaikan untuk memecahkan masalah.</span><span class="sxs-lookup"><span data-stu-id="09976-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="09976-106">Pastikan account yang menerima undangan email account yang sama yang digunakan untuk masuk lagi.</span><span class="sxs-lookup"><span data-stu-id="09976-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="09976-107">Pastikan pengguna menggunakan akun yang sama untuk menerima undangan dan masuk ke situs.</span><span class="sxs-lookup"><span data-stu-id="09976-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="09976-108">Untuk info lebih lanjut, lihat [bagaimana mengelola alias untuk Microsoft account</a> untuk mengelola login Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="09976-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="09976-109">Browse ke setiap situs di mana pengguna menerima kesalahan.</span><span class="sxs-lookup"><span data-stu-id="09976-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="09976-110">Tambahkan "/ _layouts/15/people.aspx/membershipgroupid=0" (dalam tanda kutip ganda) ke bagian akhir URL situs.</span><span class="sxs-lookup"><span data-stu-id="09976-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="09976-111">Contoh: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="09976-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="09976-112">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="09976-112">Select the user from the list.</span></span>

- <span data-ttu-id="09976-113">Klik **Hapus izin pengguna** dari pita.</span><span class="sxs-lookup"><span data-stu-id="09976-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="09976-114">Tambahkan kembali pengguna dan mengirim undangan ke pengguna.</span><span class="sxs-lookup"><span data-stu-id="09976-114">Add back the User and Resend the invite to the user.</span></span>

