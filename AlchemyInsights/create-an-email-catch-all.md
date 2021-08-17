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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080749"
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
