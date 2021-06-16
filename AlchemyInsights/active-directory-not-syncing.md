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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930978"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="71126-102">Direktori Aktif tidak tersinkron</span><span class="sxs-lookup"><span data-stu-id="71126-102">Active Directory not syncing</span></span>

<span data-ttu-id="71126-103">Jika Menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terbaru", atau pemberitahuan status sinkronisasi direktori di portal admin Office mengatakan, "Terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin AADConnect memiliki pengaturan yang salah atau izin tidak cukup untuk melakukan sinkronisasi.</span><span class="sxs-lookup"><span data-stu-id="71126-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="71126-104">Menginstal ulang AADConnect menggunakan pengaturan ekspres dapat mengatasi masalah dengan cepat:</span><span class="sxs-lookup"><span data-stu-id="71126-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="71126-105">[Unduh versi terbaru AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="71126-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="71126-106">[Ikuti instruksi untuk penginstalan ekspres.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="71126-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="71126-107">Azure AD Connect harus diinstal di Windows Server 2012 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="71126-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="71126-108">Server ini harus berupa domain bersama dan juga pengontrol domain atau server member.</span><span class="sxs-lookup"><span data-stu-id="71126-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="71126-109">Untuk daftar lengkap persyaratan Koneksi Azure AD dan prasyarat, tinjau Prasyarat [untuk Azure AD Koneksi](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="71126-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="71126-110">Untuk informasi selengkapnya tentang akun layanan AADConnect, lihat [Azure AD Koneksi: Akun dan izin](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="71126-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
