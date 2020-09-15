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
# <a name="print-spooler-issue-is-resolved"></a>Masalah spooler cetak teratasi

Jika perangkat Anda diperbarui dengan Windows 10  **OS Build 19041,329**, Anda mungkin telah mengamati masalah ketika printer tertentu gagal mencetak. Spooler cetak mungkin membuang kesalahan atau menutup secara tidak terduga saat mencoba mencetak, dan tidak ada output yang berasal dari printer yang terpengaruh. Masalah ini diatasi di OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigasi yang sedang berlangsung**

File local Security Authority Subsystem Service (LSASS) (**Isass.exe**) mungkin gagal pada beberapa perangkat dengan pesan kesalahan, "proses sistem penting, C:\WINDOWS\system32\Isass.exe, gagal dengan kode status c0000008. Mesin harus dimulai ulang ".  **Microsoft sedang mengupayakan resolusi dan akan menyediakan pembaruan dalam rilis mendatang.**

Untuk informasi selengkapnya, lihat masalah yang  [diketahui Windows 10 versi 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).