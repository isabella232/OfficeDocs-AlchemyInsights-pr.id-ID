---
title: Menyebarkan Teams mandiri atau dengan penginstalan baru atau yang Office sudah ada
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102205"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Menyebarkan Teams mandiri atau dengan penginstalan baru atau yang Office sudah ada

Microsoft Teams kini disertakan sebagai bagian dari ***penginstalan baru*** Aplikasi Microsoft 365 untuk perusahaan, Aplikasi Microsoft 365 untuk bisnis, Office untuk Mac. Untuk informasi selengkapnya, [lihat Kapan Microsoft Teams mulai disertakan dengan penginstalan baru Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Selain itu, mulai Versi 1906 dalam Saluran Saat  Ini, Teams akan ditambahkan ke penginstalan Aplikasi Microsoft 365 untuk perusahaan (dan Aplikasi Microsoft 365 untuk bisnis) yang sudah ada pada perangkat yang menjalankan Windows ketika Anda memperbarui penginstalan yang ada ke versi terbaru. Untuk informasi selengkapnya, [lihat Bagaimana dengan instalasi klien yang sudah Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jika tidak ingin menunggu jadwal peluncuran ini, Anda dapat menyebarkan Teams sebagai mandiri [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) untuk pengguna dengan mengikuti instruksi ini atau meminta pengguna menginstal Teams sendiri dari [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jika organisasi Anda belum siap untuk menyebarkan Teams, kami memiliki langkah-langkah yang dapat [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) dilakukan [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) untuk mengecualikan ***Teams*** dari penginstalan baru atau yang sudah Office. Jika ingin Teams diinstal tetapi tidak ingin Teams mulai secara otomatis bagi pengguna setelah terinstal, lihat Mencegah Microsoft Teams dimulai secara otomatis [setelah penginstalan.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Untuk ***menghapus Teams*** dari perangkat yang menjalankan Windows, lihat Menghapus [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Untuk pembersihan Microsoft Teams dari beberapa komputer atau pengguna target, [lihat Microsoft Teams pembersihan penyebaran baru](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jika Anda menggunakan komputer bersama, Remote Desktop Services (RDS), atau Virtual Desktop Infrastructure (VDI), lihat Lingkungan komputer bersama dan [VDI dengan Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jika Anda menggunakan Windows Office untuk Mac, [lihat Microsoft Teams penginstalan di Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Setelah Teams diinstal, aplikasi secara otomatis [diperbarui kira-kira](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) setiap dua minggu dengan pembaruan fitur dan kualitas baru. 