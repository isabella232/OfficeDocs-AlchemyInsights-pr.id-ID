---
title: Teams mengalami crash
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187724"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="3b1b1-102">Teams mengalami crash</span><span class="sxs-lookup"><span data-stu-id="3b1b1-102">Teams client crashing</span></span>

<span data-ttu-id="3b1b1-103">Jika klien Teams Anda mengalami crash, cobalah langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="3b1b1-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="3b1b1-104">Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="3b1b1-105">Pastikan semua rentang [Microsoft 365 URL dan alamat mudah](/microsoftteams/connectivity-issues) diakses.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="3b1b1-106">Masuk dengan akun admin penyewa Anda dan periksa Dasbor [Kesehatan Layanan Anda untuk](/office365/enterprise/view-service-health) memastikan bahwa tidak ada gangguan atau degradasi layanan.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="3b1b1-107">Menghapus instalasi dan menginstal ulang Teams Aplikasi</span><span class="sxs-lookup"><span data-stu-id="3b1b1-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="3b1b1-108">Telusuri ke folder %appdata%\Microsoft\Teams\ di komputer Anda dan hapus semua file dalam direktori tersebut.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="3b1b1-109">[Unduh dan instal Aplikasi Teams](https://www.microsoft.com/microsoft-teams/download-app), dan jika memungkinkan, instal Teams sebagai administrator (klik kanan penginstal Teams, lalu pilih Jalankan sebagai **administrator** jika tersedia).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="3b1b1-110">Jika klien Teams mengalami crash, cobalah untuk mereproduksi masalah.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="3b1b1-111">Jika Anda bisa:</span><span class="sxs-lookup"><span data-stu-id="3b1b1-111">If you can:</span></span>

1. <span data-ttu-id="3b1b1-112">Gunakan Perekam Langkah untuk merekam langkah Anda.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="3b1b1-113">Tutup SEMUA aplikasi yang tidak diperlukan atau rahasia.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="3b1b1-114">Luncurkan Perekam Langkah dan mereproduksi masalah saat masuk dengan akun pengguna yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="3b1b1-115">[Kumpulkan log tim yang merekam langkah-langkah profesional yang direkam.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="3b1b1-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="3b1b1-116">**Catatan**: Pastikan Anda mencatat alamat masuk pengguna yang terkena dampak.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="3b1b1-117">Kumpulkan buang dan/atau Info wadah kesalahan (Windows).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="3b1b1-118">Luncurkan Windows Powershell di komputer tempat crash terjadi dan jalankan perintah berikut (setelah setiap perintah, tekan Enter):</span><span class="sxs-lookup"><span data-stu-id="3b1b1-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="3b1b1-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="3b1b1-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="3b1b1-120">Setelah file teks dibuat dan muncul di layar Anda, simpan file dan lampirkan ke permintaan layanan.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
