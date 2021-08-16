---
title: Dynamics 365 - Dasbor yang Salah Ditampilkan dalam Antarmuka Terpadu Dynamics 365
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101485"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dasbor yang salah ditampilkan dalam antarmuka terpadu Dynamics 365

Ada beberapa alasan mengapa Anda mungkin melihat dasbor berbeda dari dasbor yang Anda harapkan:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Pengguna telah menetapkan dasbor default pengguna 

Biasanya Anda dapat mengidentifikasi dasbor default pengguna diatur jika **tombol Atur Sebagai Default** tidak muncul di bilah perintah dasbor. Dasbor default pengguna akan menimpa semua dasbor default lainnya, bahkan jika dasbor default pengguna tidak berada di aplikasi saat ini.

Gunakan solusi berikut ini untuk membatalkan pengaturan dasbor default.

1. Buat dasbor pribadi baru.

2. Atur dasbor baru tersebut sebagai default pengguna.

3. Hapus dasbor tersebut.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dasbor diatur dalam peta situs

Anda mungkin telah mengatur dasbor default organisasi dengan memilih dasbor dan memilih 'Atur Sebagai Default' di bawah 'Kustomisasi Sistem'. Namun dasbor yang ditetapkan dalam desainer peta situs akan diutamakan dari dasbor ini, jika pengguna memiliki akses ke dasbor tersebut.

Untuk membuat pengguna melihat dasbor yang telah Anda atur sebagai default organisasi, Anda bisa:

* Atur dasbor tersebut di peta situs

* Menghapus akses ke dasbor peta situs yang ditentukan untuk pengguna tersebut
