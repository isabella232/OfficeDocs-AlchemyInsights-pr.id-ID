---
title: Menukar PowerShell dan menghentikan autentikasi dasar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015692"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="c1320-102">Menukar PowerShell dan menghentikan autentikasi dasar</span><span class="sxs-lookup"><span data-stu-id="c1320-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="c1320-103">Untuk informasi terbaru tentang cara menghubungkan Exchange Online PowerShell tanpa menggunakan Autentikasi Dasar, [klik di sini](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="c1320-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="c1320-104">Harap diperhatikan bahwa Autentikasi Dasar masih perlu diaktifkan pada komputer klien.</span><span class="sxs-lookup"><span data-stu-id="c1320-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="c1320-105">Modul PowerShell V2 baru menggunakan Autentikasi Modern untuk membuat koneksi guna memungkinkan semua Cmdlet V2 berbasis REST.</span><span class="sxs-lookup"><span data-stu-id="c1320-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="c1320-106">Selain cmdlet V2, modul ini juga memungkinkan akses ke Cmdlet PowerShell Jarak Jauh (RPS) versi lebih lama yang perlu membuat sesi PowerShell Jarak Jauh.</span><span class="sxs-lookup"><span data-stu-id="c1320-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="c1320-107">Membuat sesi RPS pada komputer Windows memerlukan Autentikasi Dasar WinRM yang diaktifkan di komputer klien meskipun modul menggunakan mekanisme Autentikasi Modern untuk mengautentikasi ke layanan.</span><span class="sxs-lookup"><span data-stu-id="c1320-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="c1320-108">Alur Autentikasi Dasar WinRM digunakan untuk mengangkut token Autentikasi Modern.</span><span class="sxs-lookup"><span data-stu-id="c1320-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="c1320-109">Jika Autentikasi Dasar WinRM dinonaktifkan di komputer klien, cmdlet V2 baru akan terus berfungsi (tetapi cmdlet RPS yang lebih lama tidak akan berfungsi).</span><span class="sxs-lookup"><span data-stu-id="c1320-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
