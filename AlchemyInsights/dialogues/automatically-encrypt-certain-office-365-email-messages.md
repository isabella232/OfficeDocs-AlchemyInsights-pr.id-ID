---
title: Secara otomatis mengenkripsi pesan email Office 365 tertentu
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526744"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Secara otomatis mengenkripsi pesan email Office 365 tertentu

Anda dapat secara otomatis mengenkripsi pesan yang dikirim pengguna ke orang atau organisasi tertentu. Untuk melakukan ini, lakukan langkah-langkah berikut:

1. Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**. 
2. Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.
3. Di **nama**, masukkan nama untuk aturan tersebut, seperti *mengenkripsi pesan yang dikirim ke DrToniRamos@gmail.com*.
4. Dalam **menerapkan aturan ini**, pilih **penerima > adalah orang ini**. 
5. Di jendela **pilih anggota** , pilih nama orang yang ingin Anda Terapkan aturan enkripsi, lalu klik **Tambahkan**. 
6. Bila Anda sudah selesai menambahkan pengguna, klik **OK**.
7. Di samping bidang **lakukan berikut** , klik **pilih satu**. 
8. Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**. (Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
9. Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).
10. Klik **Simpan**.

> [!IMPORTANT]
> Anda dapat selalu kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

