---
title: Read-Only untuk Pesan pemeliharaan ketika mencoba menggunakan SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329451"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only untuk Pesan pemeliharaan ketika mencoba menggunakan SharePoint atau OneDrive

Pengguna mungkin menerima **pesan Baca-Saja untuk** Pemeliharaan ketika mencoba menggunakan SharePoint atau OneDrive untuk salah satu skenario berikut ini. 

-   Aktivitas pemeliharaan yang direncanakan atau aktif.  Periksa mereka dengan menavigasi ke [Pusat Pesan](https://portal.office.com/adminportal/home#/messagecenter).
-   Insiden layanan aktif berprioritas tinggi yang mungkin terjadi. Periksa penasihat/insiden dengan menavigasi ke Kesehatan [Layanan.](https://portal.office.com/adminportal/home#/servicehealth)
-   Skenario pemulihan normal-otomatis minor yang mungkin terjadi karena kejadian yang tidak diharapkan pada server yang mungkin berlangsung kurang dari 30 menit atau lebih. 
    
    Tidak ada postingan Pusat Pesan atau Kesehatan Layanan untuk pemulihan minor ini, tetapi Anda harus segera kembali ke normal.

Dalam beberapa kali kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah menyebabkan masalah tersebut, dan layanan telah dipulihkan, tetapi cache browser pengguna belum dibersihkan.

Silakan coba hapus cache browser sebelum menavigasi ke situs.

1. Di browser Microsoft Edge Anda, **pilih Pengaturan**, lalu pilih Privasi dan **Keamanan**.
2. Di **bawah Hapus penelusuran**, pilih Pilih yang akan **dihapus**.
3. Pilih **Cookie dan data situs web yang disimpan**, lalu pilih **Hapus**.

**Catatan**: Langkah-langkah ini mungkin berbeda ketika menggunakan browser lain seperti Mozilla Firefox atau Google Chrome.

**Catatan**: Opsi lain adalah membuka situs SharePoint anda OneDrive jendela InPrivate baru.