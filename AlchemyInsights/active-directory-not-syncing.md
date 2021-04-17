---
title: Direktori Aktif tidak tersinkron
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822854"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e01d2-102">Direktori Aktif tidak tersinkron</span><span class="sxs-lookup"><span data-stu-id="e01d2-102">Active Directory not syncing</span></span>

<span data-ttu-id="e01d2-103">Jika Anda menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terbaru," atau perhatikan status sinkronisasi direktori di portal admin Office mengatakan, "Terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin AADConnect memiliki pengaturan yang salah atau izin tidak cukup untuk melakukan sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="e01d2-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e01d2-104">Menginstal ulang AADConnect dengan menggunakan pengaturan ekspres dapat mengatasi masalah dengan cepat:</span><span class="sxs-lookup"><span data-stu-id="e01d2-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e01d2-105">[Unduh versi terbaru AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="e01d2-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e01d2-106">[Ikuti instruksi untuk penginstalan ekspres.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="e01d2-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e01d2-107">Untuk informasi selengkapnya tentang akun layanan AADConnect, lihat [Azure AD Connect: Akun dan izin](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e01d2-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
