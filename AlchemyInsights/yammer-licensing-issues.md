---
title: Masalah lisensi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657279"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="0a0e8-102">Masalah lisensi Yammer</span><span class="sxs-lookup"><span data-stu-id="0a0e8-102">Yammer licensing issues</span></span>

<span data-ttu-id="0a0e8-103">Semua pengguna harus memiliki lisensi untuk menggunakan layanan Yammer Enterprise, namun secara default Yammer tidak mengharuskan pengguna memiliki lisensi untuk mengakses layanan.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="0a0e8-104">Saat administrator mengubah pengaturan untuk memblokir pengguna Microsoft 365 tanpa lisensi Yammer, pengguna tidak diberi lisensi Yammer Enterprise tidak bisa mengakses layanan Yammer.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="0a0e8-105">Untuk informasi selengkapnya, lihat [mengelola lisensi pengguna Yammer di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="0a0e8-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="0a0e8-106">Saat lisensi dihapus dari pengguna, petak Yammer tidak lagi ditampilkan, dan layanan lainnya bisa menggunakan penghapusan lisensi untuk menyembunyikan fitur.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="0a0e8-107">Dalam kasus lain, fitur masih bisa muncul tapi memerlukan penugasan lisensi untuk beroperasi.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="0a0e8-108">**Lisensi tidak diperbarui untuk pengguna**</span><span class="sxs-lookup"><span data-stu-id="0a0e8-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="0a0e8-109">Terkadang, pengguna diberi lisensi tetapi masih tidak dapat mengakses Yammer.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="0a0e8-110">Penundaan lebih mungkin terjadi ketika tugas lisensi massal sedang dalam proses.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="0a0e8-111">Pengguna Yammer mungkin tidak diperbarui dalam urutan yang sama seperti lisensi yang diubah di Azure AD karena sistem berjalan asinkron.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="0a0e8-112">Tunggu hingga 24 jam sebelum membuka kasus dukungan untuk melaporkan masalah sinkronisasi lisensi.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="0a0e8-113">**Penetapan lisensi massal**</span><span class="sxs-lookup"><span data-stu-id="0a0e8-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="0a0e8-114">Lisensi bisa ditetapkan melalui Pusat admin atau scripting PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="0a0e8-115">Untuk informasi selengkapnya, lihat [menetapkan lisensi kepada pengguna](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dan [menetapkan lisensi ke akun pengguna dengan Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="0a0e8-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="0a0e8-116">Dukungan Microsoft tidak menyediakan bantuan dengan membuat skrip, tapi dokumentasi tentang penetapan lisensi Yammer tersedia.</span><span class="sxs-lookup"><span data-stu-id="0a0e8-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="0a0e8-117">Untuk informasi selengkapnya, lihat [mengelola lisensi Yammer menggunakan Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="0a0e8-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>