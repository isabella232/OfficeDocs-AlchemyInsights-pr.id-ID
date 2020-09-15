---
title: Baca-saja untuk pemeliharaan pesan ketika mencoba menggunakan SharePoint atau OneDrive
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
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670835"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Baca-saja untuk pemeliharaan pesan ketika mencoba menggunakan SharePoint atau OneDrive

Pengguna mungkin menerima pesan **baca-saja untuk pemeliharaan** saat mencoba menggunakan SharePoint atau OneDrive untuk salah satu skenario berikut ini. 

-   Aktivitas pemeliharaan terencana atau aktif.  Periksalah dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).
-   Insiden Layanan aktif prioritas tinggi yang mungkin terjadi. Periksa saran/insiden dengan menavigasi ke [Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).
-   Skenario pemulihan otomatis yang kurang penyembuhan yang mungkin terjadi karena kejadian yang tidak diharapkan di server yang mungkin berlangsung kurang dari 30 menit atau lebih. 
    
    Tidak ada pusat pesan atau postingan Kesehatan Layanan untuk pemulihan kecil ini tetapi Anda harus kembali normal secepatnya.

Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah menjadi penyebabnya, dan layanan telah dipulihkan, namun tembolok browser pengguna belum dibersihkan.

Coba Kosongkan tembolok browser sebelum menavigasi ke situs.

1. Di browser Microsoft Edge, pilih **pengaturan**, lalu pilih **privasi dan keamanan**.
2. Di bawah **Hapus penelusuran**, pilih **pilih apa yang harus dihapus**.
3. Pilih **cookie dan data situs web yang disimpan**, lalu pilih **Hapus**.

>[!Note] 
> Langkah ini mungkin berbeda ketika menggunakan browser lain seperti Mozilla Firefox atau Google Chrome.

>[!Note] 
> Opsi lainnya adalah membuka situs SharePoint atau OneDrive di jendela InPrivate yang baru.