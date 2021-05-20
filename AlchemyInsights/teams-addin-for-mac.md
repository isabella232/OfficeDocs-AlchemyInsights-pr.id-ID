---
title: Teams add-in untuk Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582073"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="56f84-102">Teams add-in untuk Mac</span><span class="sxs-lookup"><span data-stu-id="56f84-102">Teams add-in for Mac</span></span>

<span data-ttu-id="56f84-103">Untuk memecahkan masalah add-in Teams yang hilang untuk pengguna sistem operasi Mac, ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="56f84-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="56f84-104">**Langkah 1:** Jika Anda memiliki Hybrid Exchange On-Premises (2016 CU3 atau yang lebih baru diperlukan), gunakan alat Test-HMA.ps1 untuk mengonfirmasi bahwa Autentikasi Modern Hibrid telah dikonfigurasi dengan benar.</span><span class="sxs-lookup"><span data-stu-id="56f84-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="56f84-105">Untuk informasi selengkapnya, lihat [Memvalidasi penyiapan Autentikasi Modern Hibrid untuk Outlook untuk iOS dan Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="56f84-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="56f84-106">**Catatan** Gunakan format alamat UPN (misalnya, username@contoso.com ), [bukan](mailto:username@contoso.com)domain \namapengguna.</span><span class="sxs-lookup"><span data-stu-id="56f84-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="56f84-107">Lakukan hal ini bahkan untuk pengguna dengan Exchange Online surat.</span><span class="sxs-lookup"><span data-stu-id="56f84-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="56f84-108">**Langkah 2:** Miliki pengguna untuk masuk ke **Akun**  >  **Alat**... di Outlook untuk Mac, dan temukan dan pilih akun tersebut.</span><span class="sxs-lookup"><span data-stu-id="56f84-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="56f84-109">Konfirmasi nama pengguna yang tercantum berada dalam format UPN (misalnya, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="56f84-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="56f84-110">**Langkah 3:** Konfirmasi bahwa pengguna berlisensi Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="56f84-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="56f84-111">Pengguna harus menggunakan langganan Office 365 untuk Mac, produk versi 16.24 atau lebih baru.</span><span class="sxs-lookup"><span data-stu-id="56f84-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>