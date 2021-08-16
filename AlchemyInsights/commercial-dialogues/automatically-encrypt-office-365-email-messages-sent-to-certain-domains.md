---
title: Mengenkripsi pesan email Office 365 dikirim ke domain tertentu secara otomatis
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082189"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Mengenkripsi pesan email Office 365 dikirim ke domain tertentu secara otomatis

1. Dari pusat [admin Exchange ,](https://outlook.office365.com/ecp/)pilih aliran email > **email**. 
2. Klik ikon **Baru (+),** lalu klik Terapkan Enkripsi Pesan Office 365 **dan proteksi hak ke pesan.**
3. Di **Nama**, masukkan nama untuk aturan, seperti Enkripsi *pesan yang dikirim ke contoso.com*.
4. Di **Terapkan aturan ini jika**, pilih Penerima > domain **adalah**. 
5. Masukkan nama domain, seperti nama **contoso.com**.
6. Klik **ikon Tambahkan (+),** lalu klik **OK.**
7. Di samping **Lakukan bidang berikut** ini, klik Pilih salah **satu.** 
8. Di menu **turun bawah templat RMS,** pilih **Enkripsi,** lalu klik **OK.** (Jika Anda tidak melihat opsi ini, artinya paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
9. Pilih salah satu pilihan opsional (dari daftar pilihan opsional yang bisa Anda buat pada titik ini, banyak di antaranya yang bisa dibiarkan dengan pengaturan default untuk memudahkan).
10. Klik **Simpan**.

> [!IMPORTANT]
> Anda selalu bisa kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan enkripsi, lihat [Menentukan aturan alur email untuk mengenkripsi pesan email Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)