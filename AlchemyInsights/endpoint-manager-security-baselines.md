---
title: Manajer EndPoint - Baseline keamanan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421094"
---
# <a name="endpoint-manager---security-baselines"></a>Manajer EndPoint - Baseline keamanan

Baseline keamanan adalah grup Windows yang sudah dikonfigurasi sebelumnya yang membantu Anda menerapkan pengaturan keamanan yang direkomendasikan oleh tim keamanan yang relevan. Baseline ini dapat dikustomisasi untuk memberikan pengaturan dan nilai yang diinginkan saja. Untuk informasi selengkapnya tentang baseline keamanan, lihat [Menggunakan baseline keamanan untuk mengonfigurasi perangkat Windows 10 di Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Saat ini ada baseline untuk produk ini:

- Pengaturan Keamanan Windows MDM
- Pertahanan Microsoft untuk Keamanan EndPoint
- Microsoft Edge

Setiap garis dasar diperbarui secara berkala dan dirilis dalam versi bertahap. Setiap versi menambahkan dan atau menghapus pengaturan dari versi sebelumnya untuk memastikan bahwa garis dasar memenuhi panduan saat ini. Konsol dasar keamanan di Keamanan Titik Akhir memungkinkan versi yang berbeda dibandingkan dengan membuat perubahan dari versi ke versi terlihat.

Untuk panduan tentang cara paling efektif mengubah versi baseline yang digunakan, lihat Mengelola profil [garis dasar keamanan di Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Setelah menggunakan baseline keamanan, Anda bisa memantau status penggunaan dan meninjau pengaturan pada basis perangkat demi perangkat.

**Catatan:** Data pelaporan untuk baseline mungkin memakan waktu hingga 24 jam agar muncul dari penggunaan awal ke perangkat dan hingga 6 jam untuk pembaruan lebih lanjut. 

Penyebab paling umum dari pengaturan garis dasar yang tidak diterapkan adalah karena pengaturan yang sama yang digunakan di profil berbeda. Skenario ini dapat diselidiki untuk perangkat tertentu dengan memilih perangkat tersebut dari dalam node Status Perangkat di profil Garis Dasar Keamanan. Untuk detailnya, [lihat Mengatasi konflik untuk baseline keamanan.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)