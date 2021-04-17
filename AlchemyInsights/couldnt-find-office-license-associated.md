---
title: Memperbaiki aplikasi Microsoft 365 Tidak dapat menemukan pesan terkait lisensi Office
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816491"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Memperbaiki pesan "Tidak dapat menemukan lisensi Office terkait" aplikasi Microsoft 365

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet ke aplikasi Microsoft 365. Lihat [Rentang alamat IP dan URL Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Hapus dan [daftarkan ulang lisensi Office untuk](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pengguna yang terpengaruh. 
3. Buka aplikasi Office, [lalu keluar dari](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) akun pengguna yang sudah ada.
4. Masuk ke Pengaturan Windows > **Akun**  >  **Email &,** dan hapus semua akun kerja kecuali akun yang terpengaruh.
5. Masuk ke Pengaturan Windows > **Akses Akun** kerja  >  **atau sekolah**, dan putuskan koneksi semua akun kerja kecuali akun yang terpengaruh.
6. Mereset status aktivasi Office. [Pelajari caranya.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Masuk menggunakan](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) akun pengguna yang terpengaruh.

Untuk solusi pemecahan masalah tambahan, [lihat Produk Tanpa Lisensi dan kesalahan aktivasi di Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).