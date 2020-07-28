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
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="c8e6a-102">Bagan menunjukkan jumlah data yang berbeda dalam kisi</span><span class="sxs-lookup"><span data-stu-id="c8e6a-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="c8e6a-103">**Gejala**</span><span class="sxs-lookup"><span data-stu-id="c8e6a-103">**Symptom**</span></span>

<span data-ttu-id="c8e6a-104">Untuk grafik pada halaman dashboard, ketika Anda klik pada chart "..." dan klik "Lihat catatan", Anda menavigasi ke halaman grid untuk melihat semua catatan. Terkadang, jumlah catatan berubah.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="c8e6a-105">**Menyebabkan**</span><span class="sxs-lookup"><span data-stu-id="c8e6a-105">**Cause**</span></span>

<span data-ttu-id="c8e6a-106">Hal ini disebabkan oleh perbedaan tampilan antara bagan di halaman dasbor asli dan bagan di halaman Beranda kisi.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="c8e6a-107">**Solusi**</span><span class="sxs-lookup"><span data-stu-id="c8e6a-107">**Solution**</span></span>

1. <span data-ttu-id="c8e6a-108">Periksa tampilan dari halaman asli dan tampilan di kisi untuk melihat apakah mereka berbeda.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="c8e6a-109">Mengubah tampilan dalam kisi untuk mencocokkan tampilan di halaman asli.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="c8e6a-110">Jika tampilan yang benar tidak dapat ditemukan, biasanya itu berarti tampilan tidak diaktifkan di desainer aplikasi.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="c8e6a-111">Buka desainer aplikasi dari aplikasi tertentu, pilih entitas dan pandangannya, periksa tampilan yang ingin Anda Aktifkan, Simpan, publikasikan, dan tutup.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="c8e6a-112">Refresh halaman.</span><span class="sxs-lookup"><span data-stu-id="c8e6a-112">Refresh the page.</span></span>