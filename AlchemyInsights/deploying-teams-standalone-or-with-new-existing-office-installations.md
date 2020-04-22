---
title: Menyebarkan teams sebagai mandiri atau dengan penginstalan Office baru atau yang sudah ada
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704636"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Menyebarkan teams sebagai mandiri atau dengan penginstalan Office baru atau yang sudah ada

Microsoft teams sekarang disertakan sebagai bagian dari ***penginstalan baru*** Microsoft 365 aplikasi untuk perusahaan, Microsoft 365 aplikasi untuk bisnis, dan Office untuk Mac. Untuk informasi selengkapnya, lihat [Kapan Microsoft teams mulai disertakan dengan penginstalan Office baru?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Selain itu, dimulai dengan versi 1906 di bulanan saluran, tim akan ***ditambahkan ke penginstalan*** Microsoft 365 aplikasi untuk perusahaan (dan Microsoft 365 aplikasi untuk bisnis) di perangkat yang menjalankan Windows saat Anda memperbarui instalasi yang sudah ada ke versi terbaru. Untuk informasi lebih lanjut, lihat [bagaimana dengan instalasi Office yang ada?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jika tidak ingin menunggu jadwal peluncuran ini, Anda dapat menerapkan tim sebagai mandiri untuk pengguna dengan [mengikuti petunjuk](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ini atau Anda dapat meminta pengguna untuk menginstal tim sendiri [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Jika organisasi Anda belum siap untuk menggunakan teams, kami memiliki langkah yang dapat diambil untuk ***mengecualikan tim*** dari penginstalan Office [baru](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) atau [yang sudah ada](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) . Jika Anda ingin teams diinstal, namun tidak ingin tim memulai secara otomatis untuk pengguna setelah terinstal, lihat [mencegah Microsoft teams dimulai secara otomatis setelah penginstalan](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Untuk ***mencopot pemasangan teams*** dari perangkat yang menjalankan Windows, lihat [membongkar Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Untuk membersihkan Microsoft teams dari beberapa mesin target atau pengguna, lihat [penyebaran Microsoft teams dibersihkan](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jika Anda menggunakan komputer bersama, Layanan desktop jarak jauh (RDS), atau infrastruktur Desktop Virtual (VDI), lihat [lingkungan komputer bersama dan VDI dengan Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jika Anda menggunakan Office untuk Mac, lihat [penginstalan Microsoft teams di Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Setelah teams terinstal, [diperbarui secara otomatis](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) sekitar setiap dua minggu dengan fitur baru dan pembaruan kualitas. 