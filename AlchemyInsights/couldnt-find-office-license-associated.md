---
title: Memperbaiki aplikasi Microsoft 365 tidak dapat menemukan lisensi Office terkait pesan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580444"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Memperbaiki aplikasi Microsoft 365 "tidak dapat menemukan lisensi Office terkait" pesan

Jika Anda menerima pesan ini, cobalah berikut ini:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Microsoft 365. Lihat [Microsoft 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Menghapus dan [menetapkan ulang lisensi Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) untuk pengguna yang dipakai. 
3. Buka aplikasi Office dan keluar dari akun [pengguna yang ada](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) .
4. Pergi ke pengaturan **Windows > akun**  >  **email &** akun, dan Hapus semua akun kerja kecuali akun yang terpengaruh.
5. Buka pengaturan Windows > **akun**  >  **akses kerja atau sekolah**, dan putuskan semua akun kerja kecuali akun yang terpengaruh.
6. Reset status aktivasi Office. [Pelajari caranya](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Masuk](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) menggunakan akun pengguna yang terpengaruh.

Untuk solusi pemecahan masalah tambahan, lihat [produk tidak berlisensi dan kesalahan aktivasi di Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).