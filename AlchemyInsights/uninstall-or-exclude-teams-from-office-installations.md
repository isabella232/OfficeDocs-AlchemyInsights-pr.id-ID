---
title: Menghapus instalan Teams tidak Office instalan
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007721"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Menghapus instalan Teams dari instalan baru atau Office yang sudah ada

Microsoft Teams disertakan sebagai bagian dari Aplikasi Microsoft 365 untuk perusahaan, Aplikasi Microsoft 365 untuk bisnis, dan Office untuk Mac.

- Gunakan [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) untuk mengeluarkan Teams dari instalasi baru Office.
- Untuk *menghapus* Teams dari perangkat yang menjalankan Windows, lihat Menghapus [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Untuk membersihkan Microsoft Teams beberapa komputer atau pengguna target, [lihat Microsoft Teams penggunaan baru](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Gunakan opsi [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) untuk mencegah Microsoft Teams menginstal secara otomatis dengan Office.
- Gunakan opsi [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *sebelum Teams* diinstal , untuk mencegah Microsoft Teams dimulai secara otomatis setelah penginstalan.

Jika Anda menggunakan Windows Office untuk Mac, [lihat Microsoft Teams penginstalan di Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).