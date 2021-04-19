---
title: Aktifkan penyematan dialog lama untuk membuka laporan
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814267"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="1830c-102">Aktifkan penyematan dialog lama untuk membuka laporan</span><span class="sxs-lookup"><span data-stu-id="1830c-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="1830c-103">**Gejala**</span><span class="sxs-lookup"><span data-stu-id="1830c-103">**Symptom**</span></span>

<span data-ttu-id="1830c-104">Pengguna tidak dapat membuka laporan.</span><span class="sxs-lookup"><span data-stu-id="1830c-104">Users are unable to open reports.</span></span> <span data-ttu-id="1830c-105">"Terjadi kesalahan.</span><span class="sxs-lookup"><span data-stu-id="1830c-105">"Something has gone wrong.</span></span> <span data-ttu-id="1830c-106">Periksa detail teknis untuk detail selengkapnya."</span><span class="sxs-lookup"><span data-stu-id="1830c-106">Check technical details for more details."</span></span>

<span data-ttu-id="1830c-107">**Penyebab**</span><span class="sxs-lookup"><span data-stu-id="1830c-107">**Cause**</span></span>

<span data-ttu-id="1830c-108">Laporan gagal dimuat di UCI dengan kesalahan, "Deskriptor formulir null atau tidak ditentukan."</span><span class="sxs-lookup"><span data-stu-id="1830c-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="1830c-109">Laporan di UCI masih memerlukan dialog lama, sehingga sistem pelanggan harus mengaktifkan *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="1830c-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="1830c-110">**Solusi**</span><span class="sxs-lookup"><span data-stu-id="1830c-110">**Solution**</span></span>

1. <span data-ttu-id="1830c-111">Buka **Pengaturan >Administrasi > Pengaturan Sistem > tab Umum**.</span><span class="sxs-lookup"><span data-stu-id="1830c-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="1830c-112">Tetapkan "Aktifkan penyematan dialog lama tertentu di klien browser Antarmuka Terpadu" ke **Ya**.</span><span class="sxs-lookup"><span data-stu-id="1830c-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
