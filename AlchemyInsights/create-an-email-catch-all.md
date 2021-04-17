---
title: Buat email berisi semua
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816203"
---
# <a name="create-an-email-catch-all"></a>Buat email berisi semua

Penggunaan tangkapan semua tidak disarankan. Akan lebih baik jika memberikan informasi terpental kembali kepada pengirim yang memberi tahu pengirim bahwa pesan mereka tidak dapat terkirim sesuai alamat sehingga mereka dapat melakukan tindakan. Anda juga bisa membatasi kotak surat yang dipantau agar hanya menemukan alamat email yang sebelumnya valid. 

Semua tangkapan semua kotak surat akan menerima banyak spam dan pada akhirnya dapat mengisi jika tidak dipantau dengan jelas. (Terdapat batasan penerimaan.) 

Jika memutuskan untuk melanjutkan, ikuti langkah-langkah berikut:

1. Membuat grup distribusi dinamis & menyertakan "Semua Tipe Penerima."

2. Buat Kotak Surat khusus untuk menemukan email, misalnya, catchall@domain.com.

3. Untuk domain tertentu, setel DomainType ke "Internal Fonty". Jika nanti Anda menghapus semua tangkapan, pastikan untuk mengatur kembali domain ke Otoritatif.

4. Membuat Aturan Transpor Alur Email seperti berikut:

    - Jika Pengirim adalah "Di Luar Organisasi"
    - Alihkan pesan ke Catchall@domain.com
    - Kecuali jika penerima adalah anggota dari grup allusers@domain.com (Grup Distribusi berisi semua anggota)
    - Pastikan untuk memvalidasi bahwa kotak surat baru ditambahkan ke dalam Grup Distribusi Dinamis
