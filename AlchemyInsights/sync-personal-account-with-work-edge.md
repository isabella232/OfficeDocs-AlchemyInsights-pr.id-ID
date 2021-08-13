---
title: Memungkinkan pengguna menyinkronkan akun pribadi dengan akun kerja di Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813398"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Memungkinkan pengguna menyinkronkan akun pribadi dengan akun kerja di Microsoft Edge

Pastikan Anda memenuhi kriteria ini:

- Enterprise State Roaming diaktifkan di pusat admin Azure Active Directory, yang memerlukan langganan ke Azure Active Directory Premium atau Enterprise Mobility + Security (EMS). Untuk informasi selengkapnya, lihat [Mengaktifkan Jelajah Status Perusahaan di Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Satu atau kedua kriteria berikut ini terpenuhi:
    - Layanan Perlindungan Informasi Azure diaktifkan untuk penyewa Anda. Untuk detailnya, [lihat Mengaktifkan perlindungan Manajemen Hak Azure dari pusat admin Microsoft 365](/azure/information-protection/activate-office365).
    - Fitur Azure Active Directory Roaming Perusahaan (ESR, Enterprise State Roaming) diaktifkan untuk semua pengguna atau penyewa. Untuk informasi selengkapnya, lihat [Apa itu jelajah status perusahaan?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Jika AIP dan ESR dinonaktifkan, pesan kesalahan menginformasikan pengguna bahwa sinkronisasi tidak tersedia untuk akun mereka.
