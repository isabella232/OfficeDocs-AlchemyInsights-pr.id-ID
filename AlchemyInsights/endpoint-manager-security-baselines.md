---
title: EndPoint Manager - Garis dasar keamanan
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
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923557"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Garis dasar keamanan

Garis dasar keamanan adalah grup pengaturan Windows yang telah dikonfigurasi sebelumnya yang membantu Anda menerapkan pengaturan keamanan yang disarankan oleh tim keamanan terkait. Garis dasar ini dapat disesuaikan untuk menampilkan pengaturan dan nilai yang diinginkan saja. Untuk informasi selengkapnya tentang garis dasar keamanan, lihat [Menggunakan garis dasar keamanan untuk mengonfigurasi perangkat Windows 10 di Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Saat ini, garis dasar tersedia untuk produk berikut:

- Pengaturan Keamanan Windows MDM
- Pertahanan Microsoft untuk Keamanan Titik Akhir
- Microsoft Edge

Setiap garis dasar diperbarui secara berkala dan dirilis dalam versi bertahap. Setiap versi menambahkan dan atau menghapus pengaturan dari versi sebelumnya untuk memastikan bahwa garis dasar tersebut sesuai dengan panduan saat ini. Konsol Garis dasar keamanan di Keamanan Titik Akhir memungkinkan perbandingan berbagai versi dengan menjadikan perubahan dari versi ke versi terlihat.

Untuk panduan tentang cara paling efektif mengubah versi garis dasar mana yang disebarkan, lihat [Mengelola profil garis dasar keamanan di Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Setelah menyebarkan garis dasar keamanan, Anda dapat memantau status penyebaran dan meninjau pengaturan di masing-masing perangkat.

Karena baseline keamanan berisi banyak pengaturan, penting untuk meninjau perubahan konfigurasi dan melakukan pengujian untuk memastikan semua pengaturan sesuai dengan perangkat dan kebutuhan bisnis Anda.

**Catatan:** Data pelaporan garis dasar mungkin baru muncul 24 jam setelah penyebaran awal ke perangkat, dan hingga 6 jam untuk pembaruan selanjutnya. 

Penyebab paling umum mengapa pengaturan garis dasar tidak diterapkan adalah karena pengaturan yang sama sedang digunakan di profil berbeda. Skenario ini dapat diselidiki untuk perangkat tertentu dengan memilih perangkat tersebut dari dalam node Status Perangkat pada profil Garis Dasar Keamanan. Untuk selengkapnya, baca [Mengatasi konflik untuk garis dasar keamanan](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).