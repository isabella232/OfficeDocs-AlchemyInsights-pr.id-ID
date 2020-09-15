---
title: Membuat email menangkap semua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712989"
---
# <a name="create-an-email-catch-all"></a>Membuat email menangkap semua

Penggunaan menangkap semua sangat dianjurkan. Lebih baik untuk memberikan pentalan kembali ke pengirim yang memperbolehkan pengirim mengetahui pesan mereka tidak dapat dikirim seperti yang dibahas sehingga mereka dapat melakukan tindakan. Anda juga bisa membatasi kotak surat terpantau untuk hanya menangkap alamat email yang sebelumnya valid. 

Setiap kotak surat menangkap semua akan menerima spam yang baik dan mungkin akhirnya mengisi jika tidak diawasi secara ketat. (Ada batas penerimaan.) 

Jika Anda memutuskan untuk melanjutkan, ikuti langkah-langkah berikut:

1. Membuat grup distribusi dinamis & menyertakan "semua tipe Penerima."

2. Membuat kotak surat khusus untuk menangkap email, misalnya, catchall@domain.com.

3. Untuk domain tertentu, atur DomainType ke "InternalRelay". Jika nanti Anda menghapus semua tangkapan, pastikan untuk mengatur kembali domain ke otoritatif.

4. Membuat aturan transpor Mailflow sebagai berikut:

    - Jika pengirim adalah "di luar organisasi"
    - Mengalihkan pesan ke Catchall@domain.com
    - Kecuali jika Penerima adalah anggota allusers@domain.com (grup distribusi berisi semua anggota)
    - Pastikan untuk memvalidasi bahwa kotak surat baru ditambahkan ke dalam grup distribusi dinamis
