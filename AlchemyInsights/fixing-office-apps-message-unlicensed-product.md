---
title: Tidak dapat mengaktifkan Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798683"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="45e5e-102">Tidak dapat mengaktifkan Office</span><span class="sxs-lookup"><span data-stu-id="45e5e-102">Unable to activate Office</span></span>

<span data-ttu-id="45e5e-103">**Catatan**: Jika Anda menggunakan versi Windows yang lebih lama (Misalnya, Windows 7), pastikan tls 1.2 diaktifkan sebagai default.</span><span class="sxs-lookup"><span data-stu-id="45e5e-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="45e5e-104">Untuk informasi selengkapnya, lihat Pembaruan untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP Windows .</span><span class="sxs-lookup"><span data-stu-id="45e5e-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="45e5e-105">Periksa apakah status langganan Anda sudah kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="45e5e-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="45e5e-106">Pastikan Anda memiliki langganan yang mengizinkan lisensi klien, seperti Office 365 Bisnis atau Bisnis Premium, dan [pastikan pengguna memiliki lisensi yang ditetapkan](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="45e5e-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="45e5e-107">Pastikan pengguna masuk ke Office menggunakan akun yang sama dengan lisensi yang ditetapkan.</span><span class="sxs-lookup"><span data-stu-id="45e5e-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="45e5e-108">Periksa [halaman Kondisi Layanan Office 365](/office365/enterprise/view-service-health) untuk melihat apakah ada masalah umum pada layanan.</span><span class="sxs-lookup"><span data-stu-id="45e5e-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="45e5e-109">Periksa firewall, perangkat lunak antivirus, dan pengaturan proksi Anda untuk memastikan agar akses aplikasi Microsoft 365 ke internet tidak terblokir.</span><span class="sxs-lookup"><span data-stu-id="45e5e-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="45e5e-110">Lihat [Rentang URL dan alamat IP Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL dan rentang alamat IP Office 365").</span><span class="sxs-lookup"><span data-stu-id="45e5e-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="45e5e-111">**Tips** Di komputer Windows, kami dapat mendiagnosis dan otomatis memperbaiki beberapa masalah masuk Office yang umum untuk Anda.</span><span class="sxs-lookup"><span data-stu-id="45e5e-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="45e5e-112">Unduh dan jalankan  **[Asisten Dukungan dan Pemulihan Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** untuk menggunakan alat otomatis kami.</span><span class="sxs-lookup"><span data-stu-id="45e5e-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="45e5e-113">Gunakan tindakan pemecahan masalah berikut:</span><span class="sxs-lookup"><span data-stu-id="45e5e-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="45e5e-114">Buka aplikasi Office, lalu [keluar](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) dari akun pengguna yang ada.</span><span class="sxs-lookup"><span data-stu-id="45e5e-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="45e5e-115">[Hapus](/microsoft-365/admin/manage/remove-licenses-from-users) dan [tetapkan kembali](/microsoft-365/admin/manage/assign-licenses-to-users) lisensi Office, kemudian [masuk ke Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) menggunakan akun pengguna yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="45e5e-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="45e5e-116">Jalankan [Pemecah Masalah Aktivasi](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="45e5e-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="45e5e-117">Atur ulang status aktivasi Office</span><span class="sxs-lookup"><span data-stu-id="45e5e-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Atur ulang status aktivasi Office")
- [<span data-ttu-id="45e5e-118">Lakukan Perbaikan Online Office</span><span class="sxs-lookup"><span data-stu-id="45e5e-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="45e5e-119">Untuk solusi pemecahan masalah lainnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="45e5e-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="45e5e-120">Produk Tanpa Lisensi dan kesalahan aktivasi di Office</span><span class="sxs-lookup"><span data-stu-id="45e5e-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="45e5e-121">Kesalahan "Maaf, kami tidak dapat terhubung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan Office</span><span class="sxs-lookup"><span data-stu-id="45e5e-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)