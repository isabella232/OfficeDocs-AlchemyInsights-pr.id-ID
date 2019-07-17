---
title: Dynamics 365 - salah Dashboard menunjukkan dalam antarmuka yang bersatu Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747919"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Salah dashboard menunjukkan dalam antarmuka yang bersatu Dynamics 365

Ada beberapa alasan mengapa Anda mungkin melihat sebuah dashboard yang berbeda daripada yang Anda harapkan:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Pengguna telah menetapkan pengguna default dashboard 

Biasanya Anda dapat mengidentifikasi pengguna default dashboard diatur jika tombol **Set sebagai Default** tidak menunjukkan di bilah perintah dashboard. Pengguna default dashboard akan menimpa semua default dashboard, bahkan jika pengguna default dasbor tidak di app saat ini.

Menggunakan solusi berikut untuk unset dashboard default mereka.

1. Membuat dashboard pribadi baru.

2. Menetapkan dashboard yang baru sebagai default pengguna.

3. Menghapus dashboard itu.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboard terletak di sitemap

Anda dapat menetapkan dashboard default organisasi dengan memilih sebuah dashboard dan memilih 'Set sebagai Default' di bawah 'Menyesuaikan sistem'. Tapi dashboard didefinisikan dalam desain sitemap akan mengambil alih dashboard ini, jika pengguna memiliki akses ke sana.

Agar pengguna melihat dashboard Anda tetapkan sebagai default organisasi, Anda dapat:

* Menetapkan bahwa dashboard dalam sitemap

* Menghapus akses ke dashboard sitemap yang ditetapkan bagi para pengguna
