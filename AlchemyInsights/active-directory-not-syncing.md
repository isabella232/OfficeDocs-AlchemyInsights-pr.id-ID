---
title: Direktori aktif tidak disinkronkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697632"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="2ae6d-102">Direktori aktif tidak disinkronkan</span><span class="sxs-lookup"><span data-stu-id="2ae6d-102">Active Directory not syncing</span></span>

<span data-ttu-id="2ae6d-103">Jika Anda menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terkini," atau pemberitahuan status sinkronisasi direktori di portal admin Office mengatakan, "terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin ada yang tidak memiliki pengaturan yang salah atau izin yang tidak mencukupi untuk melakukan sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="2ae6d-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="2ae6d-104">Menginstal ulang AADConnect dengan menggunakan pengaturan kilat mungkin mengatasi masalah dengan cepat:</span><span class="sxs-lookup"><span data-stu-id="2ae6d-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="2ae6d-105">[Unduh versi terbaru dari AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="2ae6d-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="2ae6d-106">[Ikuti instruksi untuk penginstalan Ekspresikan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="2ae6d-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="2ae6d-107">Untuk informasi selengkapnya tentang akun Layanan AADConnect, lihat [AZURE AD Connect: akun dan izin](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="2ae6d-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
