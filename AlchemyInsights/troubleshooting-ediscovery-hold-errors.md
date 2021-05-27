---
title: Pemecahan masalah ediscovery menyimpan kesalahan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676152"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Pemecahan masalah ediscovery menyimpan kesalahan

Mengalami masalah dengan eDiscovery yang dialami? Berikut beberapa praktik terbaik untuk dipertimbangkan:

- Periksa status distribusi tahan.  Jika status Aktif **(Tertunda)** atau **Nonaktif (Tertunda),** tunggu hingga pendistribusian penangguhan selesai.
- Gabungkan eDiscovery menyimpan pembaruan ke dalam satu permintaan massal daripada memperbarui kebijakan berulang kali untuk setiap transaksi.
- Jalankan Set-CaseHoldPolicy <policyname> -RetryDistribution di Powershell Pusat Keamanan dan Kepatuhan. Untuk detailnya, [lihat Koneksi pusat & PowerShell Pusat Kepatuhan](/powershell/exchange/connect-to-scc-powershell).

Untuk langkah-langkah dalam memeriksa pengaturan ini dan praktik terbaik tambahan untuk mengurangi dan mengatasi masalah menyelenggarakan eDiscovery, lihat Memecahkan masalah [kesalahan tahan eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)
Untuk informasi tentang pemecahan masalah eDiscovery umum lainnya, lihat [Selidiki, memecahkan masalah, dan mengatasi masalah eDiscovery umum.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
