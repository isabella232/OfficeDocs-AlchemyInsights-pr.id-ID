---
title: Bagan menunjukkan jumlah data yang berbeda dalam kisi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439353"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Bagan menunjukkan jumlah data yang berbeda dalam kisi

**Gejala**

Untuk grafik pada halaman dashboard, ketika Anda klik pada chart "..." dan klik "Lihat catatan", Anda menavigasi ke halaman grid untuk melihat semua catatan. Terkadang, jumlah catatan berubah.

**Menyebabkan**

Hal ini disebabkan oleh perbedaan tampilan antara bagan di halaman dasbor asli dan bagan di halaman Beranda kisi.  

**Solusi**

1. Periksa tampilan dari halaman asli dan tampilan di kisi untuk melihat apakah mereka berbeda.
2. Mengubah tampilan dalam kisi untuk mencocokkan tampilan di halaman asli.
3. Jika tampilan yang benar tidak dapat ditemukan, biasanya itu berarti tampilan tidak diaktifkan di desainer aplikasi.
4. Buka desainer aplikasi dari aplikasi tertentu, pilih entitas dan pandangannya, periksa tampilan yang ingin Anda Aktifkan, Simpan, publikasikan, dan tutup.
5. Refresh halaman.