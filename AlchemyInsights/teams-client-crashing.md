---
title: Klien Teams mengalami crash?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826274"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="1f770-102">Klien Teams mengalami crash?</span><span class="sxs-lookup"><span data-stu-id="1f770-102">Teams client crashing?</span></span>

<span data-ttu-id="1f770-103">Jika klien Teams Anda mengalami crash, cobalah langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="1f770-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="1f770-104">Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="1f770-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="1f770-105">Pastikan semua rentang [alamat dan URL Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) mudah diakses.</span><span class="sxs-lookup"><span data-stu-id="1f770-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="1f770-106">Masuk dengan akun admin penyewa Anda dan periksa Dasbor [Kesehatan Layanan Anda untuk](https://docs.microsoft.com/office365/enterprise/view-service-health) memastikan bahwa tidak ada gangguan atau degradasi layanan.</span><span class="sxs-lookup"><span data-stu-id="1f770-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="1f770-107">Menghapus instalan dan menginstal ulang Aplikasi Teams (tautan)</span><span class="sxs-lookup"><span data-stu-id="1f770-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="1f770-108">Telusuri ke folder %appdata%\Microsoft\teams\ di komputer Anda dan hapus semua file dalam direktori tersebut.</span><span class="sxs-lookup"><span data-stu-id="1f770-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="1f770-109">[Unduh dan instal Aplikasi Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)dan jika memungkinkan, instal Teams sebagai administrator (klik kanan penginstal Teams, lalu pilih "Jalankan sebagai administrator" jika tersedia).</span><span class="sxs-lookup"><span data-stu-id="1f770-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="1f770-110">Jika klien Teams masih mengalami crash, dapatkah Anda mereproduksi masalah?</span><span class="sxs-lookup"><span data-stu-id="1f770-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="1f770-111">Jika demikian:</span><span class="sxs-lookup"><span data-stu-id="1f770-111">If so:</span></span>

1. <span data-ttu-id="1f770-112">Gunakan Perekam Langkah untuk merekam langkah Anda.</span><span class="sxs-lookup"><span data-stu-id="1f770-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="1f770-113">Tutup SEMUA aplikasi yang tidak diperlukan atau rahasia.</span><span class="sxs-lookup"><span data-stu-id="1f770-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="1f770-114">Luncurkan Perekam Langkah dan mereproduksi masalah saat masuk dengan akun pengguna yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="1f770-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="1f770-115">[Kumpulkan log tim yang merekam langkah-langkah profesional yang direkam.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="1f770-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="1f770-116">**Catatan**: Pastikan Anda mencatat alamat masuk pengguna yang terkena dampak.</span><span class="sxs-lookup"><span data-stu-id="1f770-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="1f770-117">Kumpulkan buang dan/atau Info wadah kesalahan (Windows).</span><span class="sxs-lookup"><span data-stu-id="1f770-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="1f770-118">Luncurkan Windows Powershell di komputer tempat crash terjadi dan jalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="1f770-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="1f770-119">Lampirkan file ke kasus dukungan Anda.</span><span class="sxs-lookup"><span data-stu-id="1f770-119">Attach the file to your support case.</span></span>
