---
title: Secara otomatis mengenkripsi pesan email tertentu dari Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746133"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Secara otomatis mengenkripsi pesan email tertentu dari Office 365

1. Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**. 
2. Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.
3. Di **nama**, masukkan nama untuk aturan, seperti *Enkripsikan semua pesan*.
4. Dalam **menerapkan aturan ini**, pilih **[Terapkan ke semua pesan]**. 
5. Di samping bidang **lakukan berikut** , klik **pilih satu**. 
6. Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**. (Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
7. Periksa kotak centang **audit aturan ini dengan tingkat keparahan** , lalu pilih tingkat yang diinginkan. Jika perusahaan Anda memiliki kewajiban kontraktual untuk mengirim semua email terenkripsi, saya menyarankan untuk mengatur tingkat ke **tinggi**.
8. Di bawah **Pilih model untuk aturan ini**, klik **Terapkan**. 
9. Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).
10. Klik **Simpan**.

> [!IMPORTANT]
> Anda dapat selalu kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

