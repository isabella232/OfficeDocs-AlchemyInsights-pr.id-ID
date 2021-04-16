---
title: Menukar PowerShell dan menghentikan autentikasi dasar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813475"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="842a8-102">Menukar PowerShell dan menghentikan autentikasi dasar</span><span class="sxs-lookup"><span data-stu-id="842a8-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="842a8-103">Untuk informasi terbaru tentang cara menghubungkan Exchange Online PowerShell tanpa menggunakan Autentikasi Dasar, [klik di sini](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="842a8-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="842a8-104">Modul PowerShell V2 tidak menggunakan autentikasi dasar.</span><span class="sxs-lookup"><span data-stu-id="842a8-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="842a8-105">Harap diperhatikan bahwa Autentikasi Dasar masih perlu diaktifkan pada komputer klien.</span><span class="sxs-lookup"><span data-stu-id="842a8-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="842a8-106">Modul PowerShell V2 baru menggunakan Autentikasi Modern untuk membuat koneksi guna memungkinkan semua Cmdlet V2 berbasis REST.</span><span class="sxs-lookup"><span data-stu-id="842a8-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="842a8-107">Selain cmdlet V2, modul ini juga memungkinkan akses ke Cmdlet PowerShell Jarak Jauh (RPS) versi lebih lama yang perlu membuat sesi PowerShell Jarak Jauh.</span><span class="sxs-lookup"><span data-stu-id="842a8-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="842a8-108">Membuat sesi RPS pada komputer Windows memerlukan Autentikasi Dasar WinRM yang diaktifkan di komputer klien meskipun modul menggunakan mekanisme Autentikasi Modern untuk mengautentikasi ke layanan.</span><span class="sxs-lookup"><span data-stu-id="842a8-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="842a8-109">Alur Autentikasi Dasar WinRM digunakan untuk mengangkut token Autentikasi Modern.</span><span class="sxs-lookup"><span data-stu-id="842a8-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="842a8-110">Jika Autentikasi Dasar WinRM dinonaktifkan di komputer klien, cmdlet V2 baru akan terus berfungsi (tetapi cmdlet RPS yang lebih lama tidak akan berfungsi).</span><span class="sxs-lookup"><span data-stu-id="842a8-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
