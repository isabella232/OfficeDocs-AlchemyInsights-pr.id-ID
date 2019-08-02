---
title: Penggelaran tim sebagai standalone atau dengan instalasi kantor baru atau yang ada
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054234"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Penggelaran tim sebagai standalone atau dengan instalasi kantor baru atau yang ada

Microsoft Teams sekarang dimasukkan sebagai bagian dari ***instalasi baru*** Office 365 ProPlus, Office 365 bisnis dan kantor untuk Mac. Untuk informasi lebih lanjut, lihat [Kapan Microsoft Teams mulai diikutsertakan dengan instalasi baru kantor?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Selain itu, dimulai dengan versi 1906 di saluran bulanan, tim akan ***ditambahkan ke instalasi yang sudah ada*** kantor 365 ProPlus (dan Office 365 bisnis) pada perangkat yang menjalankan Windows ketika Anda memperbarui instalasi yang ada ke versi terbaru. Untuk informasi lebih lanjut, lihat [apa tentang instalasi yang sudah ada kantor?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jika Anda tidak ingin menunggu jadwal peluncuran ini, Anda dapat menyebarkan tim sebagai standalone untuk pengguna Anda dengan [mengikuti petunjuk berikut](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) atau Anda dapat memiliki pengguna menginstal tim untuk diri mereka sendiri dari [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Jika organisasi Anda tidak siap untuk menyebarkan tim, kami memiliki langkah-langkah yang dapat Anda ambil untuk ***mengecualikan tim*** dari instalasi [baru](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) atau [yang ada](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) di kantor. Jika Anda ingin tim untuk diinstal, tetapi tidak ingin tim untuk memulai secara otomatis untuk pengguna setelah terinstall, melihat [Mencegah Microsoft tim dari dimulai secara otomatis setelah pemasangan](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Untuk ***menghapus tim*** dari perangkat yang menjalankan Windows, lihat [Uninstall Microsoft tim](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Untuk pembersihan Microsoft Teams dari beberapa mesin target atau pengguna, lihat [Microsoft tim penyebaran membersihkan](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jika Anda menggunakan komputer bersama, Remote Desktop Services (RDS) atau Virtual Desktop infrastruktur (VDI), melihat [bersama komputer dan VDI lingkungan dengan Microsoft tim](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jika Anda menggunakan Office for Mac, lihat [Microsoft tim instalasi pada Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Setelah tim diinstal, hal ini [akan secara otomatis diperbarui](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) kira-kira setiap dua minggu dengan fitur baru dan update kualitas. 