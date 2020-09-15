---
title: Memecahkan masalah sinkronisasi kata sandi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664929"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="eaa6c-102">Memecahkan masalah sinkronisasi kata sandi</span><span class="sxs-lookup"><span data-stu-id="eaa6c-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="eaa6c-103">Untuk memecahkan masalah sinkronisasi kata sandi, mulai menggunakan tugas pemecahan masalah AAD ini untuk menentukan mengapa kata sandi tidak disinkronkan.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="eaa6c-104">Untuk memulai, masuk ke [Kelola sinkronisasi langsung](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="eaa6c-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="eaa6c-105">Buka sesi Windows PowerShell baru di server Azure AD Connect Anda, lalu pilih opsi **Jalankan sebagai administrator** .</span><span class="sxs-lookup"><span data-stu-id="eaa6c-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="eaa6c-106">Jalankan set-ExecutionPolicy Remotesanye atau set-ExecutionPolicy tidak terbatas.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="eaa6c-107">Mulai panduan Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="eaa6c-108">Masuk ke halaman tugas tambahan > **memecahkan masalah**  >  **berikutnya**.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="eaa6c-109">Pilih **Luncurkan** untuk membuka menu pemecahan masalah PowerShell.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="eaa6c-110">Pilih **memecahkan masalah sinkronisasi kata sandi**.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="eaa6c-111">Masalah biasanya adalah kata sandi tidak disinkronkan untuk akun pengguna tertentu.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="eaa6c-112">**Catatan** Sinkronisasi kata sandi gagal jika sinkronisasi kata sandi yang terakhir berhasil adalah beberapa waktu yang lalu.</span><span class="sxs-lookup"><span data-stu-id="eaa6c-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="eaa6c-113">Untuk bantuan selengkapnya tentang pemecahan masalah sinkronisasi kata sandi, lihat [memecahkan masalah sinkronisasi hash kata sandi dengan sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="eaa6c-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>