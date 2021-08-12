---
title: Memecahkan masalah bergabung di Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939922"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Memecahkan masalah bergabung di Azure AD

1. Jika Anda menyiapkan pendaftaran perangkat untuk kali pertama, pastikan Anda telah meninjau Pengenalan pada manajemen perangkat di [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) yang akan memandu Anda tentang cara mendapatkan Perangkat di bawah kontrol ke Azure AD. 
1. Jika mendaftarkan perangkat ke Azure AD secara langsung dan mendaftarkan perangkat ke Intune, Pastikan Anda telah mengonfigurasi [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) dan lisensinya tersedia terlebih dahulu.
1. Pastikan Anda memiliki wewenang untuk melakukan operasi di Azure AD. Hanya administrator global di Microsoft Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat.
1. Untuk melakukan implementasi bergabung di Azure AD, lihat [Merencanakan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Untuk detail selengkapnya tentang mengatasi masalah umum dengan bergabung di Azure AD, lihat [FAQ Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) dan untuk perangkat Windows 10 pro, lihat Tidak dapat bergabung ke Windows 10 Pro komputer ke Azure AD - Perlu memutakhirkan ke - Microsoft [Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
