---
title: Memecahkan masalah pekerjaan Layanan Impor terhenti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125111"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="167fb-102">Memecahkan masalah pekerjaan Layanan Impor terhenti</span><span class="sxs-lookup"><span data-stu-id="167fb-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="167fb-103">Jika Anda mengalami masalah dengan pekerjaan Impor layanan terhenti atau gagal, periksa dan coba hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="167fb-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="167fb-104">Tinjau ukuran file PST.</span><span class="sxs-lookup"><span data-stu-id="167fb-104">Review the size of of the PST file.</span></span> <span data-ttu-id="167fb-105">Ukuran maksimal file PST yang direkomendasikan untuk impor adalah 20GB.</span><span class="sxs-lookup"><span data-stu-id="167fb-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="167fb-106">Jika Anda menduga item yang dilewati karena kerusakan, jalankan Scanpst.exe untuk mendiagnosis dan memperbaiki kesalahan dalam file PST.</span><span class="sxs-lookup"><span data-stu-id="167fb-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="167fb-107">Jika Anda melihat kesalahan "MapiExceptionShutoffQuotaExceeded" selama mengimpor, pastikan kotak surat target memiliki kapasitas yang memadai untuk mengimpor file PST yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="167fb-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="167fb-108">Untuk informasi selengkapnya tentang pemecahan masalah pekerjaan impor PST, lihat [Memecahkan masalah pekerjaan impor PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="167fb-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="167fb-109">Untuk informasi tentang cara memperbaiki masalah saat mengimpor PST ke dalam Outlook, lihat Memperbaiki masalah pengi impor [file .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="167fb-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>