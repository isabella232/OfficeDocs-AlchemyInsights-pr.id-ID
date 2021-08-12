---
title: Mengirim pesan email dengan menyediakan ID pesan jaringan
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929920"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Mengirim pesan email dengan menyediakan ID pesan jaringan

1. Di flyout **Pengiriman baru,** pilih **Email dan** ID **Pesan Jaringan**.
2. Ikuti langkah-langkah ini untuk menemukan ID pesan untuk pesan email Outlook:
    1. Klik ganda pesan email untuk membukanya.
    1. Pilih **Properti**  >  **File.**
    1. Buka Notepad dokumen Word kosong, lalu salin dan tempelkan konten yang ditemukan di kotak **Header internet** ke dokumen yang terbuka untuk visibilitas yang lebih baik.
    1. Temukan bidang **X-MS-Exchange-Organization-Network-Message-Id.** Nilai setelah **: adalah** ID yang diperlukan untuk pengiriman Anda.
3. Di **bawah Penerima,** jika email masuk ke folder email sampah untuk semua penerima email ini, pilih **Pilih Semua**. Jika tidak, pilih hanya pengguna yang melaporkan masalah.
4. Di **bawah Alasan pengiriman**, jika Anda memilih Seharusnya telah diblokir , tentukan apakah pesan harus diblokir sebagai **Spam**, **Phishing**, atau **Malware**, lalu pilih **Kirim**. 

Untuk mempelajari selengkapnya, [lihat Cara mengirimkan spam, URL, dan](https://go.microsoft.com/fwlink/?linkid=2101479)file yang dicurigai sebagai spam, URL, dan file ke Microsoft untuk memindai .
