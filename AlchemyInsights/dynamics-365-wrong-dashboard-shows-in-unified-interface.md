---
title: Dynamics 365-dasbor yang salah ditampilkan di antarmuka terpadu Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711278"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dasbor yang salah ditampilkan di antarmuka terpadu Dynamics 365

Ada beberapa alasan mengapa Anda melihat dasbor yang berbeda dari yang Anda duga:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Pengguna telah mengatur dasbor default pengguna 

Biasanya Anda bisa mengidentifikasi dasbor default pengguna diatur jika tombol **Atur sebagai default** tidak muncul di bilah perintah dasbor. Dasbor default pengguna akan menimpa semua dasbor default lainnya, meskipun dasbor default pengguna tidak ada di aplikasi saat ini.

Gunakan solusi berikut untuk membuka dasbor default mereka.

1. Membuat dasbor pribadi baru.

2. Setel dasbor baru sebagai default pengguna.

3. Hapus dasbor tersebut.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dasbor diatur dalam peta situs

Anda mungkin telah menetapkan dasbor default organisasi dengan memilih dasbor dan memilih ' setel sebagai default ' di bawah ' kustomisasi sistem '. Tapi dasbor yang ditentukan dalam desainer Sitemap akan lebih diutamakan daripada dasbor ini, jika pengguna memiliki akses ke dasbor tersebut.

Untuk meminta pengguna melihat dasbor yang telah Anda setel sebagai default organisasi, Anda bisa:

* Mengatur dasbor tersebut dalam peta situs

* Menghapus akses ke dasbor yang ditentukan Sitemap untuk pengguna tersebut
