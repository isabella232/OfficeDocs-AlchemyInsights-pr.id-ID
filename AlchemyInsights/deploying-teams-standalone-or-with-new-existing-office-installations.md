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
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320125"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Menyebarkan Teams mandiri atau dengan penginstalan baru atau yang Office sudah ada

Microsoft Teams kini disertakan sebagai bagian dari ***penginstalan baru*** Aplikasi Microsoft 365 untuk perusahaan, Aplikasi Microsoft 365 untuk bisnis, Office untuk Mac. Untuk informasi selengkapnya, [lihat Kapan Microsoft Teams mulai disertakan dengan penginstalan baru Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Selain itu, mulai Versi 1906 dalam Saluran Saat  Ini, Teams akan ditambahkan ke penginstalan Aplikasi Microsoft 365 untuk perusahaan (dan Aplikasi Microsoft 365 untuk bisnis) yang sudah ada pada perangkat yang menjalankan Windows ketika Anda memperbarui penginstalan yang sudah ada ke versi terbaru. Untuk informasi selengkapnya, [lihat Bagaimana dengan instalasi klien yang sudah Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Catatan**: Jika Anda tidak ingin menunggu jadwal peluncuran ini, Anda bisa menggunakan Teams sebagai [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) mandiri untuk pengguna Anda dengan mengikuti instruksi ini atau Anda bisa meminta pengguna Anda menginstal Teams sendiri dari [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jika organisasi Anda belum siap untuk menyebarkan Teams, kami memiliki langkah-langkah yang [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) dapat [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) dilakukan untuk mengecualikan ***Teams*** dari penginstalan baru atau yang sudah Office. Jika ingin Teams diinstal tetapi tidak ingin Teams mulai secara otomatis bagi pengguna setelah terinstal, lihat Mencegah Microsoft Teams dimulai secara otomatis setelah [penginstalan.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Untuk ***menghapus Teams*** dari perangkat yang menjalankan Windows, lihat Menghapus [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Untuk pembersihan Microsoft Teams dari beberapa komputer atau pengguna target, [lihat Microsoft Teams pembersihan penyebaran baru](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jika Anda menggunakan komputer bersama, Remote Desktop Services (RDS), atau Virtual Desktop Infrastructure (VDI), lihat Lingkungan komputer bersama dan [VDI dengan Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jika Anda menggunakan Windows Office untuk Mac, [lihat Microsoft Teams instalasi di Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Catatan**: Setelah Teams diinstal, fitur secara otomatis [diperbarui](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) kira-kira setiap dua minggu dengan pembaruan fitur dan kualitas baru. 