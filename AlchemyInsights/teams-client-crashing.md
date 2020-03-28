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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030684"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="0a6ef-102">Klien Teams mengalami crash?</span><span class="sxs-lookup"><span data-stu-id="0a6ef-102">Teams client crashing?</span></span>

<span data-ttu-id="0a6ef-103">Jika klien Teams Anda mengalami crash, cobalah langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="0a6ef-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0a6ef-104">Jika Anda menggunakan aplikasi desktop Teams, [pastikan aplikasi sudah diperbarui sepenuhnya](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0a6ef-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0a6ef-105">Pastikan semua [URL dan rentang alamat Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dapat diakses.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0a6ef-106">Masuklah dengan akun admin Anda, lalu periksa [Dasbor Kesehatan Layanan](https://docs.microsoft.com/office365/enterprise/view-service-health) untuk memverifikasi bahwa tidak ada gangguan atau penurunan layanan.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="0a6ef-107">Sebagai langkah terakhir, Anda dapat mencoba membersihkan cache klien Teams Anda:</span><span class="sxs-lookup"><span data-stu-id="0a6ef-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="0a6ef-108">Keluarlah sepenuhnya dari klien desktop Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="0a6ef-109">Anda dapat mengklik kanan **Teams** dari Baki Ikon dan mengklik **Tutup**, atau menjalankan Manajer Tugas dan mengakhiri proses sepenuhnya.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="0a6ef-110">Buka File Explorer, lalu ketik %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="0a6ef-111">Setelah berada di direktori, Anda akan melihat beberapa folder berikut:</span><span class="sxs-lookup"><span data-stu-id="0a6ef-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="0a6ef-112">Dari dalam **Cache Aplikasi**, buka Cache dan hapus file apa pun di lokasi Cache: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="0a6ef-113">Dari dalam **Penyimpanan_blob**, hapus semua file: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="0a6ef-114">Dari dalam **Cache**, hapus semua file: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="0a6ef-115">Dari dalam **database**, hapus semua file: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="0a6ef-116">Dari dalam **GPUCache**, hapus semua file: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="0a6ef-117">Dari dalam **IndexedDB**, hapus file .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="0a6ef-118">Dari dalam **Penyimpanan Lokal**, hapus semua file: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="0a6ef-119">Terakhir, dari dalam **tmp**, hapus semua file: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="0a6ef-120">Mulai ulang klien Teams Anda.</span><span class="sxs-lookup"><span data-stu-id="0a6ef-120">Restart your Teams client.</span></span>
