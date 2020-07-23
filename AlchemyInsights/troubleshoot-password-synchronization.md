---
title: Memecahkan masalah sinkronisasi sandi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387880"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="cbb17-102">Memecahkan masalah sinkronisasi sandi</span><span class="sxs-lookup"><span data-stu-id="cbb17-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="cbb17-103">Untuk memecahkan masalah sinkronisasi sandi, mulai menggunakan tugas pemecahan masalah AAD menghubungkan ini untuk menentukan mengapa sandi tidak menyinkronkan.</span><span class="sxs-lookup"><span data-stu-id="cbb17-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="cbb17-104">Untuk memulai, buka [mengelola sinkronisasi langsung](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="cbb17-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="cbb17-105">Buka sesi Windows PowerShell baru di server Azure AD menyambung, dan pilih opsi **Jalankan sebagai administrator** .</span><span class="sxs-lookup"><span data-stu-id="cbb17-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="cbb17-106">Jalankan set-ExecutionPolicy Remotesanye atau set-ExecutionPolicy terbatas.</span><span class="sxs-lookup"><span data-stu-id="cbb17-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="cbb17-107">Mulai Wisaya Azure AD menyambung.</span><span class="sxs-lookup"><span data-stu-id="cbb17-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="cbb17-108">Buka halaman tugas tambahan > **memecahkan masalah**  >  **berikutnya**.</span><span class="sxs-lookup"><span data-stu-id="cbb17-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="cbb17-109">Pilih **Luncurkan** untuk membuka menu pemecahan masalah PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cbb17-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="cbb17-110">Pilih **memecahkan masalah sinkronisasi sandi**.</span><span class="sxs-lookup"><span data-stu-id="cbb17-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="cbb17-111">Masalah ini biasanya bahwa sandi tidak disinkronkan untuk akun pengguna tertentu.</span><span class="sxs-lookup"><span data-stu-id="cbb17-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="cbb17-112">**Notes** Sinkronisasi sandi gagal jika Sinkronisasi sandi berhasil terakhir adalah beberapa waktu yang lalu.</span><span class="sxs-lookup"><span data-stu-id="cbb17-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="cbb17-113">Untuk bantuan lebih lanjut pemecahan masalah sinkronisasi sandi, lihat [memecahkan masalah sinkronisasi hash sandi dengan AZURE AD menyambung sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="cbb17-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>