---
title: Mengenkripsi pesan email tertentu secara otomatis dari office 365
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
ms.openlocfilehash: e050074f26025906561237c9ef487ed4743f93b1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322252"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Mengenkripsi pesan email tertentu secara otomatis dari office 365

1. Dari pusat [admin Exchange ,](https://outlook.office365.com/ecp/)pilih aliran email > **email**. 
2. Klik ikon **Baru (+),** lalu klik Terapkan Enkripsi Pesan Office 365 **dan perlindungan hak pada pesan.**
3. Di **Nama**, masukkan nama untuk aturan tersebut, seperti *Enkripsi semua pesan*.
4. Di **Terapkan aturan ini jika**, pilih **[Terapkan ke semua pesan]**. 
5. Di samping **Lakukan bidang berikut** ini, klik Pilih salah **satu.** 
6. Di menu **turun bawah templat RMS,** pilih **Enkripsi,** lalu klik **OK.** (Jika Anda tidak melihat opsi ini, artinya paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
7. Centang kotak **Audit aturan ini dengan tingkat keparahan,** lalu pilih tingkat yang diinginkan. Jika perusahaan Anda memiliki kewajiban kontraktual untuk mengirim semua email terenkripsi, saya merekomendasikan mengatur tingkatan ke **Tinggi.**
8. Di **bawah Pilih model untuk aturan ini,** klik **Terapkan.** 
9. Pilih salah satu pilihan opsional (dari daftar pilihan opsional yang bisa Anda buat pada titik ini, banyak di antaranya yang bisa dibiarkan dengan pengaturan default untuk memudahkan).
10. Klik **Simpan**.

**Penting:** Anda selalu dapat kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan enkripsi, lihat [Menentukan aturan alur email untuk mengenkripsi pesan email Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

