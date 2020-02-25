---
title: Direktori aktif tidak disinkronkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265199"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="48989-102">Direktori aktif tidak disinkronkan</span><span class="sxs-lookup"><span data-stu-id="48989-102">Active Directory not syncing</span></span>

<span data-ttu-id="48989-103">Jika Anda menerima galat sinkronisasi, seperti "tidak ada sinkronisasi baru", atau melihat status sinkronisasi direktori di portal admin Office mengatakan, "terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin AADConnect memiliki pengaturan yang salah atau tidak mencukupi izin untuk melakukan sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="48989-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="48989-104">Menginstal ulang AADConnect dengan menggunakan pengaturan Express dapat mengatasi masalah dengan cepat:</span><span class="sxs-lookup"><span data-stu-id="48989-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="48989-105">[Download versi terbaru dari AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="48989-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="48989-106">[Ikuti petunjuk untuk instalasi Ekspres](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="48989-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="48989-107">Untuk informasi selengkapnya tentang akun Layanan AADConnect, lihat [AZURE AD menyambung: akun dan izin](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="48989-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
