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
# <a name="print-spooler-issue-is-resolved"></a>Print spooler masalah teratasi

Jika perangkat Anda telah diperbarui dengan Windows 10 **OS membangun 19041,329**, Anda mungkin telah mengamati masalah di mana printer tertentu gagal untuk mencetak. Spooler cetak mungkin membuang galat atau menutup tiba-tiba ketika mencoba untuk mencetak, dan output tidak berasal dari printer yang terpengaruh. Masalah ini diatasi di OS Build **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigasi berkelanjutan**

File lokal keamanan otoritas subsistem Layanan (LSASS) (**Isass.exe**) mungkin gagal pada beberapa perangkat dengan pesan galat, "proses sistem yang penting, C:\WINDOWS\system32\Isass.exe, gagal dengan kode status c0000008. Mesin sekarang harus direstart ".  **Microsoft bekerja pada resolusi dan akan memberikan pembaruan pada peluncuran mendatang.**

Untuk informasi lebih lanjut, silakan periksa [Windows 10 versi 2004 masalah yang diketahui](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).