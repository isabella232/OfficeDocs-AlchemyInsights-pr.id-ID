---
title: Read-Only untuk pemeliharaan pesan saat mencoba untuk menggunakan SharePoint atau OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620726"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only untuk pemeliharaan pesan saat mencoba untuk menggunakan SharePoint atau OneDrive

Pengguna dapat menerima pesan **Read-Only untuk pemeliharaan** saat mencoba untuk menggunakan SharePoint atau OneDrive untuk salah satu skenario berikut. 

-   Kegiatan pemeliharaan direncanakan atau aktif.  Memeriksa mereka dengan menavigasi ke [Pusat pesan](https://portal.office.com/adminportal/home#/messagecenter).
-   Layanan aktif prioritas tinggi, insiden yang mungkin terjadi. Periksa setiap nasihat/insiden dengan menavigasi ke [Layanan kesehatan](https://portal.office.com/adminportal/home#/servicehealth).
-   Kecil menyembuhkan pemulihan skenario yang mungkin terjadi karena setiap kejadian tak terduga di server yang mungkin bertahan selama kurang dari 30 menit atau lebih. 
    
    Ada tidak ada pusat pesan atau jasa kesehatan posts untuk pemulihan ini kecil tapi Anda harus kembali ke normal segera.

Pada beberapa kesempatan kami mengamati bahwa salah satu dari tiga skenario yang tercantum di atas telah menjadi penyebab, dan layanan telah dikembalikan, tetapi cache browser pengguna belum dibersihkan.

Silakan mencoba membersihkan browser cache sebelum menavigasi ke situs.

1. Di peramban Microsoft Edge, pilih **pengaturan**, dan kemudian pilih **privasi dan keamanan**.
2. **Jelas browsing**, pilih **memilih apa yang harus jelas**.
3. Pilih **kuki dan data situs web tersimpan**, dan pilih **jelas**.

>[!Note] 
> Langkah-langkah ini mungkin berbeda dengan menggunakan peramban lainnya, seperti Mozilla Firefox atau Google Chrome.

>[!Note] 
> Pilihan lain adalah untuk membuka situs SharePoint atau OneDrive di jendela InPrivate baru.