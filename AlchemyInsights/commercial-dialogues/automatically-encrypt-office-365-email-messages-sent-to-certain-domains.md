---
title: Secara otomatis mengenkripsi pesan email Office 365 yang dikirim ke domain tertentu
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746049"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Secara otomatis mengenkripsi pesan email Office 365 yang dikirim ke domain tertentu

1. Dari [Pusat admin Exchange](https://outlook.office365.com/ecp/), pilih **aturan > alur email**. 
2. Klik ikon **baru (+)** , lalu klik **Terapkan enkripsi pesan Office 365 dan perlindungan hak ke pesan**.
3. Di **nama**, masukkan nama untuk aturan tersebut, seperti *mengenkripsi pesan yang dikirim ke contoso.com*.
4. Dalam **menerapkan aturan ini**, pilih **penerima domain >**. 
5. Masukkan nama domain, seperti **contoso.com**.
6. Klik ikon **Tambahkan (+)** , lalu klik **OK**.
7. Di samping bidang **lakukan berikut** , klik **pilih satu**. 
8. Di menu turun bawah **Templat RMS** , pilih **Enkripsikan**, lalu klik **OK**. (Jika Anda tidak melihat opsi ini, itu berarti paket Anda tidak menyertakan enkripsi otomatis. Tapi Anda bisa menambahkannya!)
9. Pilih pilihan opsional apa pun (dari daftar pilihan opsional yang bisa Anda buat pada saat ini, banyak yang bisa dibiarkan dengan pengaturan default untuk kesederhanaan).
10. Klik **Simpan**.

> [!IMPORTANT]
> Anda dapat selalu kembali dan mengedit aturan ini nanti.

Untuk informasi selengkapnya tentang membuat aturan untuk enkripsi, lihat [menentukan aturan aliran email untuk mengenkripsi pesan email di Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)