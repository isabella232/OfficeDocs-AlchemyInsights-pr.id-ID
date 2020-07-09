---
title: Print spooler masalah teratasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088399"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="3df01-102">Print spooler masalah teratasi</span><span class="sxs-lookup"><span data-stu-id="3df01-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="3df01-103">Jika perangkat Anda telah diperbarui dengan Windows 10 **OS membangun 19041,329**, Anda mungkin telah mengamati masalah di mana printer tertentu gagal untuk mencetak.</span><span class="sxs-lookup"><span data-stu-id="3df01-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="3df01-104">Spooler cetak mungkin membuang galat atau menutup tiba-tiba ketika mencoba untuk mencetak, dan output tidak berasal dari printer yang terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="3df01-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="3df01-105">Masalah ini diatasi di OS Build **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="3df01-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="3df01-106">**Investigasi berkelanjutan**</span><span class="sxs-lookup"><span data-stu-id="3df01-106">**Ongoing investigation**</span></span>

<span data-ttu-id="3df01-107">File lokal keamanan otoritas subsistem Layanan (LSASS) (**Isass.exe**) mungkin gagal pada beberapa perangkat dengan pesan galat, "proses sistem yang penting, C:\WINDOWS\system32\Isass.exe, gagal dengan kode status c0000008.</span><span class="sxs-lookup"><span data-stu-id="3df01-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="3df01-108">Mesin sekarang harus direstart ".</span><span class="sxs-lookup"><span data-stu-id="3df01-108">The machine must now be restarted".</span></span>  <span data-ttu-id="3df01-109">**Microsoft bekerja pada resolusi dan akan memberikan pembaruan pada peluncuran mendatang.**</span><span class="sxs-lookup"><span data-stu-id="3df01-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="3df01-110">Untuk informasi lebih lanjut, silakan periksa [Windows 10 versi 2004 masalah yang diketahui](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="3df01-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>