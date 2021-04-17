---
title: Memperbaiki aplikasi Microsoft 365 Tidak dapat menemukan pesan terkait lisensi Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816491"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="7f0b9-102">Memperbaiki pesan "Tidak dapat menemukan lisensi Office terkait" aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7f0b9-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="7f0b9-103">Jika Anda menerima pesan ini, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="7f0b9-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="7f0b9-104">Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet ke aplikasi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="7f0b9-105">Lihat [Rentang alamat IP dan URL Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="7f0b9-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="7f0b9-106">Hapus dan [daftarkan ulang lisensi Office untuk](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pengguna yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="7f0b9-107">Buka aplikasi Office, [lalu keluar dari](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) akun pengguna yang sudah ada.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="7f0b9-108">Masuk ke Pengaturan Windows > **Akun**  >  **Email &,** dan hapus semua akun kerja kecuali akun yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="7f0b9-109">Masuk ke Pengaturan Windows > **Akses Akun** kerja  >  **atau sekolah**, dan putuskan koneksi semua akun kerja kecuali akun yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="7f0b9-110">Mereset status aktivasi Office.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-110">Reset the Office activation state.</span></span> <span data-ttu-id="7f0b9-111">[Pelajari caranya.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="7f0b9-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="7f0b9-112">[Masuk menggunakan](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) akun pengguna yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="7f0b9-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="7f0b9-113">Untuk solusi pemecahan masalah tambahan, [lihat Produk Tanpa Lisensi dan kesalahan aktivasi di Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="7f0b9-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>