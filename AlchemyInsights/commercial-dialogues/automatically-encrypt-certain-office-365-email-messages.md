---
title: Mengenkripsi pesan email tertentu Office 365 secara otomatis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949570"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Mengenkripsi pesan email tertentu Office 365 secara otomatis

Anda bisa secara otomatis mengenkripsi pesan yang dikirim pengguna ke orang atau organisasi eksternal tertentu. Untuk melakukannya, lakukan langkah-langkah berikut:

1. Dari pusat [admin Exchange ,](https://outlook.office365.com/ecp/)pilih aliran email > **email**. 
2. Klik ikon **Baru (+),** lalu klik Terapkan Enkripsi Pesan Office 365 **dan proteksi hak ke pesan.**
3. Di **Nama**, masukkan nama untuk aturan, seperti Enkripsi *pesan yang dikirim ke DrToniRamos@gmail.com*.
4. Di **Terapkan aturan ini jika**, pilih Penerima > adalah orang **ini**. 
5. Di **jendela Pilih** Anggota, pilih nama orang yang Anda inginkan menerapkan aturan enkripsi, lalu klik **tambahkan**. 
6. Bila sudah selesai menambahkan pengguna, klik **OK.**
7. Di samping **Lakukan bidang berikut** ini, klik Pilih salah **satu.** 
8. Di menu **turun bawah templat RMS,** pilih **Enkripsi,** lalu klik **OK.** (Jika Anda tidak melihat opsi ini, artinya paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
9. Pilih salah satu pilihan opsional (dari daftar pilihan opsional yang bisa Anda buat pada titik ini, banyak di antaranya yang bisa dibiarkan dengan pengaturan default untuk memudahkan).
10. Klik **Simpan**.

> [!IMPORTANT]
> Anda selalu bisa kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan enkripsi, lihat [Menentukan aturan alur email untuk mengenkripsi pesan email Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

