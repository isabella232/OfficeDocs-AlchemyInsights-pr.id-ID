---
title: Memperbaiki aplikasi Microsoft 365 tidak dapat menemukan pesan lisensi Office yang terkait
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747698"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Memperbaiki aplikasi Microsoft 365 "tidak dapat menemukan lisensi Office yang terkait"

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proksi Anda untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365. Lihat [URL dan rentang alamat IP Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Hapus dan [tetapkan ulang lisensi Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) untuk pengguna yang terpengaruh. 
3. Buka aplikasi Office dan keluar dari semua akun [pengguna yang sudah](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ada.
4. Masuk ke pengaturan Windows > **Accounts**akun  >  **& email**akun, dan Hapus semua akun kerja kecuali akun yang terpengaruh.
5. Masuk ke pengaturan Windows > **akun**  >  **mengakses kantor atau sekolah**, dan putuskan semua akun kerja kecuali akun yang terpengaruh.
6. Mereset status aktivasi Office. [Pelajari caranya](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Masuk](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) menggunakan akun pengguna yang terpengaruh.

Untuk solusi pemecahan masalah tambahan, lihat [produk tanpa lisensi dan kesalahan aktivasi di Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).