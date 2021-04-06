---
title: Identifikasi masalah Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595851"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="f14c1-102">Identifikasi masalah Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="f14c1-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="f14c1-103">Diagnostik Desktop Virtual Windows hanya menggunakan satu cmdlet PowerShell tetapi berisi banyak parameter opsional untuk membantu mempersempit dan mengisolasi masalah.</span><span class="sxs-lookup"><span data-stu-id="f14c1-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="f14c1-104">Untuk memulai:</span><span class="sxs-lookup"><span data-stu-id="f14c1-104">To get started:</span></span> 

1. <span data-ttu-id="f14c1-105">Unduh dan impor modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f14c1-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="f14c1-106">Untuk detailnya, [lihat Cmdlet Desktop Virtual Windows untuk Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="f14c1-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="f14c1-107">Jalankan cmdlet berikut untuk masuk ke akun Anda:</span><span class="sxs-lookup"><span data-stu-id="f14c1-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="f14c1-108">Contoh: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="f14c1-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="f14c1-109">**CATATAN:** Semua kueri yang menggunakan PowerShell harus menyertakan parameter -UserName atau -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="f14c1-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="f14c1-110">Untuk kemampuan pemantauan, lihat [Menggunakan Analitik Log untuk fitur diagnostik](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="f14c1-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="f14c1-111">Untuk memfilter aktivitas diagnostik menurut pengguna, jalankan cmdlet berikut:</span><span class="sxs-lookup"><span data-stu-id="f14c1-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="f14c1-112">Contoh: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="f14c1-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="f14c1-113">Terdapat daftar filter yang dapat Anda jalankan untuk mendiagnosis masalah.</span><span class="sxs-lookup"><span data-stu-id="f14c1-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="f14c1-114">Untuk mempelajari selengkapnya tentang mendiagnosis masalah, lihat [Mengidentifikasi dan mendiagnosis masalah Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="f14c1-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="f14c1-115">Untuk mempelajari selengkapnya tentang kesalahan umum, [lihat Kesalahan umum sens](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f14c1-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
