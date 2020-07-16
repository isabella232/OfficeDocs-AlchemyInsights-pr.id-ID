---
title: Masalah lisensi heboh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148312"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="b481f-102">Masalah lisensi heboh</span><span class="sxs-lookup"><span data-stu-id="b481f-102">Yammer licensing issues</span></span>

<span data-ttu-id="b481f-103">Semua pengguna harus memiliki izin untuk menggunakan layanan heboh perusahaan, tetapi secara default heboh tidak mengharuskan pengguna memiliki lisensi untuk mengakses layanan.</span><span class="sxs-lookup"><span data-stu-id="b481f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="b481f-104">Ketika administrator perubahan pengaturan untuk memblokir Microsoft 365 pengguna tanpa lisensi heboh, pengguna tidak ditetapkan lisensi heboh perusahaan tidak dapat mengakses layanan heboh.</span><span class="sxs-lookup"><span data-stu-id="b481f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="b481f-105">Untuk informasi lebih lanjut, lihat [mengelola heboh pengguna lisensi di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b481f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="b481f-106">Ketika lisensi dihapus dari pengguna, ubin heboh tidak lagi ditampilkan, dan layanan lainnya dapat menggunakan penghapusan lisensi untuk menyembunyikan fitur.</span><span class="sxs-lookup"><span data-stu-id="b481f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="b481f-107">Dalam kasus lain, fitur masih dapat muncul tetapi memerlukan penetapan lisensi untuk beroperasi.</span><span class="sxs-lookup"><span data-stu-id="b481f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="b481f-108">**Lisensi tidak mendapatkan diperbarui untuk pengguna**</span><span class="sxs-lookup"><span data-stu-id="b481f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="b481f-109">Terkadang, pengguna ditetapkan lisensi tetapi masih tidak dapat mengakses heboh.</span><span class="sxs-lookup"><span data-stu-id="b481f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="b481f-110">Penundaan cenderung terjadi ketika penetapan lisensi massal sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="b481f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="b481f-111">Heboh pengguna mungkin tidak diperbarui dalam urutan yang sama sebagai lisensi diubah di Azure AD karena sistem berjalan asinkron.</span><span class="sxs-lookup"><span data-stu-id="b481f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="b481f-112">Tunggu hingga 24 jam sebelum membuka kasus dukungan untuk melaporkan masalah sinkronisasi lisensi.</span><span class="sxs-lookup"><span data-stu-id="b481f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="b481f-113">**Tugas lisensi massal**</span><span class="sxs-lookup"><span data-stu-id="b481f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="b481f-114">Lisensi dapat ditetapkan melalui Pusat admin atau skrip PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b481f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="b481f-115">Untuk informasi lebih lanjut, lihat [menetapkan lisensi untuk pengguna](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dan [menetapkan lisensi untuk account pengguna dengan Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="b481f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="b481f-116">Dukungan Microsoft tidak memberikan bantuan dengan membuat skrip, namun dokumentasi tentang penetapan lisensi Yammer tersedia.</span><span class="sxs-lookup"><span data-stu-id="b481f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="b481f-117">Untuk informasi lebih lanjut, lihat [mengelola heboh lisensi dengan menggunakan Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="b481f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>