---
title: Memperbaiki Microsoft 365 Tidak dapat menemukan lisensi Office yang terkait dengan pesan
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
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069607"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Memperbaiki masalah Microsoft 365 "Tidak dapat menemukan lisensi Office terkait"

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet Microsoft 365 lain. Lihat [Microsoft 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Hapus dan [Office lisensi untuk](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pengguna yang terpengaruh. 
3. Buka buku aplikasi Office [dan keluar dari](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) akun pengguna yang sudah ada.
4. Masuk ke Windows Pengaturan >   >  **Akun Email &, dan** hapus semua akun kerja kecuali akun yang terpengaruh.
5. Masuk ke Windows Pengaturan > **Akun Akses kerja** atau sekolah ,  >  **lalu** putuskan sambungan semua akun kerja kecuali akun yang terpengaruh.
6. Mereset Office status aktivasi. [Pelajari caranya.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Masuk menggunakan](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) akun pengguna yang terpengaruh.

Untuk solusi pemecahan masalah tambahan, [lihat Produk Tanpa Lisensi dan kesalahan aktivasi Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).