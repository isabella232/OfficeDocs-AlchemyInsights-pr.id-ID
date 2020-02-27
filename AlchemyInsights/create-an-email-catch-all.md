---
title: Buat email menangkap semua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286196"
---
# <a name="create-an-email-catch-all"></a>Buat email menangkap semua

Penggunaan menangkap semua sangat dianjurkan. Lebih baik untuk memberikan bouncing kembali ke pengirim membiarkan pengirim tahu pesan mereka tidak dapat dikirim seperti yang dibahas sehingga mereka dapat mengambil tindakan. Anda juga dapat membatasi kotak pesan yang dipantau untuk hanya menangkap alamat email yang sebelumnya valid. 

Setiap menangkap semua kotak surat akan menerima banyak spam dan akhirnya dapat mengisi jika tidak diawasi dengan cermat. (Ada batas penerimaan.) 

Jika Anda memutuskan untuk melanjutkan, ikuti langkah berikut:

1. Membuat grup distribusi dinamis & mencakup "semua jenis penerima."

2. Buat kotak surat khusus untuk menangkap email, misalnya, catchall@domain.com.

3. Untuk domain tertentu, tetapkan DomainType ke "InternalRelay". Jika Anda kemudian menghapus menangkap semua, pastikan untuk mengatur domain kembali ke otoritatif.

4. Buat aturan transpor Mailflow sebagai berikut:

    - Jika pengirim adalah "di luar organisasi"
    - Mengalihkan pesan ke Catchall@domain.com
    - Kecuali jika Penerima adalah anggota allusers@domain.com (grup distribusi berisi semua anggota)
    - Pastikan untuk memvalidasi bahwa kotak pesan baru ditambahkan ke grup distribusi dinamis
