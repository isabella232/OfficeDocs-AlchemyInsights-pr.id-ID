---
title: Add-in teams untuk Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670331"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="2d85d-102">Add-in teams untuk Mac</span><span class="sxs-lookup"><span data-stu-id="2d85d-102">Teams add-in for Mac</span></span>

<span data-ttu-id="2d85d-103">Untuk memecahkan masalah Add-in tim yang hilang untuk pengguna sistem operasi Mac, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="2d85d-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="2d85d-104">**Langkah 1:** Jika Anda memiliki Exchange hibrid di tempat (2016 CU3 atau yang lebih baru diperlukan), gunakan alat Test-HMA.ps1 untuk mengonfirmasi bahwa autentikasi modern hibrid dikonfigurasikan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="2d85d-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="2d85d-105">Untuk informasi selengkapnya, lihat [memvalidasi penyiapan autentikasi modern hibrid untuk Outlook untuk IOS dan Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="2d85d-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="2d85d-106">**Catatan** Gunakan format alamat UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)), bukan domain\username.</span><span class="sxs-lookup"><span data-stu-id="2d85d-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="2d85d-107">Lakukan ini bahkan untuk pengguna dengan kotak surat Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2d85d-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="2d85d-108">**Langkah 2:** Minta pengguna masuk ke akun **alat**  >  **Accounts**... di Outlook untuk Mac, dan temukan dan pilih akun.</span><span class="sxs-lookup"><span data-stu-id="2d85d-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="2d85d-109">Konfirmasi nama pengguna yang tercantum dalam format UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="2d85d-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="2d85d-110">**Langkah 3:** Konfirmasi pengguna adalah pengguna Microsoft teams berlisensi.</span><span class="sxs-lookup"><span data-stu-id="2d85d-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="2d85d-111">Pengguna harus menggunakan langganan Office 365 untuk Mac, produk versi 16,24 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="2d85d-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>