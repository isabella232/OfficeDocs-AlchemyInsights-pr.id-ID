---
title: Masalah spooler cetak teratasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801844"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="f2fff-102">Masalah spooler cetak teratasi</span><span class="sxs-lookup"><span data-stu-id="f2fff-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="f2fff-103">Jika perangkat Anda diperbarui dengan Windows 10  **OS Build 19041,329**, Anda mungkin telah mengamati masalah ketika printer tertentu gagal mencetak.</span><span class="sxs-lookup"><span data-stu-id="f2fff-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="f2fff-104">Spooler cetak mungkin membuang kesalahan atau menutup secara tidak terduga saat mencoba mencetak, dan tidak ada output yang berasal dari printer yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="f2fff-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="f2fff-105">Masalah ini diatasi di OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="f2fff-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="f2fff-106">**Investigasi yang sedang berlangsung**</span><span class="sxs-lookup"><span data-stu-id="f2fff-106">**Ongoing investigation**</span></span>

<span data-ttu-id="f2fff-107">File local Security Authority Subsystem Service (LSASS) (**Isass.exe**) mungkin gagal pada beberapa perangkat dengan pesan kesalahan, "proses sistem penting, C:\WINDOWS\system32\Isass.exe, gagal dengan kode status c0000008.</span><span class="sxs-lookup"><span data-stu-id="f2fff-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="f2fff-108">Mesin harus dimulai ulang ".</span><span class="sxs-lookup"><span data-stu-id="f2fff-108">The machine must now be restarted".</span></span>  <span data-ttu-id="f2fff-109">**Microsoft sedang mengupayakan resolusi dan akan menyediakan pembaruan dalam rilis mendatang.**</span><span class="sxs-lookup"><span data-stu-id="f2fff-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="f2fff-110">Untuk informasi selengkapnya, lihat masalah yang  [diketahui Windows 10 versi 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="f2fff-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>