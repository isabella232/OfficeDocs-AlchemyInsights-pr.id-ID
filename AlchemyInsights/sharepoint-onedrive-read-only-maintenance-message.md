---
title: Baca-saja untuk pemeliharaan pesan saat berusaha menggunakan SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051284"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Baca-saja untuk pemeliharaan pesan saat berusaha menggunakan SharePoint atau OneDrive

Pengguna akan menerima **baca-saja untuk pesan pemeliharaan** saat mencoba menggunakan SharePoint atau OneDrive untuk salah satu dari skenario berikut ini. 

-   Kegiatan pemeliharaan yang direncanakan atau aktif.  Periksa untuk mereka dengan menavigasi ke [pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).
-   Sebuah kejadian layanan yang aktif dan prioritas tinggi yang mungkin terjadi. Periksa apakah ada saran/insiden dengan menavigasi ke [layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth).
-   Sebuah minor pemulihan Auto-penyembuhan skenario yang dapat terjadi karena setiap kejadian tak terduga pada server yang mungkin berlangsung selama kurang dari 30 menit atau lebih. 
    
    Ada tidak ada pusat pesan atau layanan kesehatan posting untuk pemulihan kecil ini tetapi Anda harus kembali normal segera.

Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah penyebabnya, dan layanan telah dipulihkan, tetapi cache browser pengguna belum dibersihkan.

Silakan mencoba untuk menghapus cache browser sebelum menavigasi ke situs.

1. Di browser Microsoft Edge Anda, pilih **pengaturan**, dan kemudian pilih **privasi dan keamanan**.
2. Di bawah **browsing yang jelas**, pilih **pilih apa yang harus jelas**.
3. Pilih **cookie dan data situs web yang disimpan**, lalu pilih **Hapus**.

>[!Note] 
> Langkah ini mungkin berbeda ketika menggunakan browser lain seperti Mozilla Firefox atau Google Chrome.

>[!Note] 
> Pilihan lain akan membuka situs SharePoint atau OneDrive di jendela InPrivate baru.