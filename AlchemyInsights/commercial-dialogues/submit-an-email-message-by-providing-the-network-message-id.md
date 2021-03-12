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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745519"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Mengirim pesan email dengan menyediakan ID pesan jaringan

1. Dalam Flyout **penyerahan baru** , pilih **email** dan **id pesan jaringan**.
2. Ikuti langkah-langkah ini untuk menemukan ID pesan untuk pesan email di Outlook:
    1. Klik ganda pesan email untuk membukanya.
    1. Pilih   >  **properti** file.
    1. Buka Notepad atau dokumen Word kosong, lalu salin dan tempel konten yang ditemukan di kotak **header Internet** ke dalam dokumen yang terbuka untuk visibilitas yang lebih baik.
    1. Temukan bidang **id pesan-jaringan-X-MS-Exchange-organisasi** . Nilai setelah **:** adalah id yang Anda perlukan untuk pengiriman Anda.
3. Di bawah **penerima**, jika email mendarat di folder email sampah untuk semua penerima email ini, pilih **Pilih Semua**. Jika tidak, pilih hanya pengguna yang melaporkan masalahnya.
4. Di **bawah alasan untuk penyerahan**, jika Anda **memilih seharusnya diblokir**, Tentukan apakah pesan tersebut seharusnya diblokir sebagai **spam**, **phishing**, atau **malware**, lalu pilih **kirim**.

Untuk mempelajari selengkapnya, lihat [cara mengirimkan dugaan spam, Phish, URL, dan file ke Microsoft untuk pemindaian](https://go.microsoft.com/fwlink/?linkid=2101479).
