---
title: Dynamics 365-salah Dasbor menunjukkan di Dynamics 365 antarmuka terpadu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528554"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Salah dashboard menunjukkan di antarmuka terpadu Dynamics 365

Ada beberapa alasan mengapa Anda mungkin melihat dasbor yang berbeda dari yang Anda harapkan:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Pengguna telah menetapkan dashboard default pengguna 

Biasanya Anda dapat mengidentifikasi dashboard default pengguna diatur jika **ditetapkan sebagai default** tombol tidak muncul di bilah perintah dasbor. Dasbor default pengguna akan menimpa semua dasbor default lainnya, meskipun dasbor default pengguna tidak ada di aplikasi saat ini.

Gunakan solusi berikut untuk Unset dashboard default mereka.

1. Buat dasbor pribadi baru.

2. Setel dasbor baru sebagai default pengguna.

3. Hapus dasbor tersebut.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dasbor diatur dalam peta situs

Anda mungkin telah menetapkan dashboard default organisasi dengan memilih dashboard dan memilih ' set AS default ' di bawah ' Customize The System '. Namun dasbor yang ditetapkan dalam perancang peta situs akan diutamakan daripada dasbor ini, jika pengguna memiliki akses ke dashboard tersebut.

Agar pengguna melihat dasbor yang Anda tetapkan sebagai default organisasi, Anda dapat:

* Menyetel dasbor di peta situs

* Hapus akses ke dasbor yang ditetapkan peta situs untuk pengguna tersebut
