---
title: Klien Teams mengalami crash?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354055"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="7d8e1-102">Klien Teams mengalami crash?</span><span class="sxs-lookup"><span data-stu-id="7d8e1-102">Teams client crashing?</span></span>

<span data-ttu-id="7d8e1-103">Jika klien Teams Anda mengalami crash, cobalah langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="7d8e1-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7d8e1-104">Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7d8e1-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7d8e1-105">Pastikan semua [Microsoft 365 URL dan kisaran alamat](https://docs.microsoft.com/microsoftteams/connectivity-issues) dapat diakses.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7d8e1-106">Masuk dengan akun admin penyewa Anda dan periksa [dasbor Kesehatan Layanan](https://docs.microsoft.com/office365/enterprise/view-service-health) Anda untuk memverifikasi bahwa tidak ada pemutusan atau degradasi layanan yang ada.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="7d8e1-107">Uninstall dan menginstal ulang teams aplikasi (link)</span><span class="sxs-lookup"><span data-stu-id="7d8e1-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="7d8e1-108">Browse ke folder%appdata%\Microsoft\teams\ di komputer Anda dan menghapus semua file dalam direktori tersebut.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="7d8e1-109">[Unduh dan instal aplikasi teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), dan jika memungkinkan, instal teams sebagai administrator (klik kanan Penginstal teams, lalu pilih "Jalankan sebagai administrator" jika tersedia).</span><span class="sxs-lookup"><span data-stu-id="7d8e1-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="7d8e1-110">Jika klien tim Anda masih mogok, Dapatkah Anda mereproduksi masalah?</span><span class="sxs-lookup"><span data-stu-id="7d8e1-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="7d8e1-111">Jika demikian:</span><span class="sxs-lookup"><span data-stu-id="7d8e1-111">If so:</span></span>

1. <span data-ttu-id="7d8e1-112">Gunakan langkah Recorder untuk menangkap langkah Anda.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="7d8e1-113">Tutup semua aplikasi yang tidak perlu atau rahasia.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="7d8e1-114">Peluncuran langkah Recorder dan mereproduksi masalah saat masuk dengan akun pengguna yang dipakai.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="7d8e1-115">[Mengumpulkan log tim yang menangkap langkah repro direkam](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="7d8e1-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="7d8e1-116">**Catatan**: Pastikan Anda menangkap alamat masuk dari pengguna yang terkena dampak.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="7d8e1-117">Mengumpulkan dump dan/atau kesalahan ember info (Windows).</span><span class="sxs-lookup"><span data-stu-id="7d8e1-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="7d8e1-118">Luncurkan Windows PowerShell di mesin tempat terjadinya crash dan jalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="7d8e1-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="7d8e1-119">Lampirkan file ke kasus dukungan Anda.</span><span class="sxs-lookup"><span data-stu-id="7d8e1-119">Attach the file to your support case.</span></span>
