---
title: Menerapkan praktik terbaik untuk kueri berburu tingkat lanjut
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694271"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="143e8-102">Menerapkan praktik terbaik untuk kueri berburu tingkat lanjut</span><span class="sxs-lookup"><span data-stu-id="143e8-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="143e8-103">Untuk mendapatkan hasil lebih cepat dan menghindari waktu tunggu saat menjalankan kueri yang kompleks, Terapkan praktik terbaik ini:</span><span class="sxs-lookup"><span data-stu-id="143e8-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="143e8-104">Saat mencoba kueri baru, selalu gunakan batas untuk menghindari rangkaian hasil yang sangat besar.</span><span class="sxs-lookup"><span data-stu-id="143e8-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="143e8-105">Juga, gunakan `count` untuk membuat penilaian awal dari ukuran rangkaian hasil.</span><span class="sxs-lookup"><span data-stu-id="143e8-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="143e8-106">Gunakan filter waktu terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="143e8-106">Use time filters first.</span></span> <span data-ttu-id="143e8-107">Idealnya, Batasi kueri Anda hingga tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="143e8-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="143e8-108">Di awal kueri, tepat setelah filter waktu, tambahkan filter yang diharapkan untuk menghapus sebagian besar data.</span><span class="sxs-lookup"><span data-stu-id="143e8-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="143e8-109">Saat mencari token penuh, gunakan operator dan `has` bukan `contains` .</span><span class="sxs-lookup"><span data-stu-id="143e8-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="143e8-110">Menjalankan pencarian pada kolom tertentu dan bukan di seluruh kolom.</span><span class="sxs-lookup"><span data-stu-id="143e8-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="143e8-111">Saat bergabung ke tabel, tentukan tabel terlebih dahulu dengan lebih sedikit baris.</span><span class="sxs-lookup"><span data-stu-id="143e8-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="143e8-112">`project` hanya kolom yang diperlukan dari tabel yang sudah Anda ikuti.</span><span class="sxs-lookup"><span data-stu-id="143e8-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="143e8-113">Untuk mempelajari selengkapnya, lihat [praktik terbaik kueri berburu lanjutan](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="143e8-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
