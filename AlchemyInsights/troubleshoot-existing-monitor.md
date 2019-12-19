---
title: Pemecahan masalah monitor yang ada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738572"
---
# <a name="troubleshoot-an-existing-monitor"></a>Memecahkan masalah monitor yang ada

Coba solusi ini untuk memecahkan masalah monitor. 

**Segarkan layar monitor Anda:**

Tekan tombol berikut pada saat yang sama: tombol Windows + Ctrl + Shift + B. Ini akan menyegarkan komunikasi dengan driver grafis Anda. Monitor Anda akan berkedip sebentar dan kembali setelah beberapa detik.

**Memecahkan masalah perangkat keras monitor:**

1. Cabut kabel yang menyambungkan PC ke monitor, lalu sambungkan kembali.
2. Lepaskan semua perangkat non-esensial dari PC Anda (seperti adaptor atau Dok).

**Jika Anda baru saja menginstal pembaruan di PC, Anda dapat memutar kembali driver tampilan:**

1. Pilih **mulai**, ketik **Device Manager**, dan pilih **Device Manager** dari hasil.
2. Luaskan bagian **Adapter tampilan** , klik kanan Adapter tampilan Anda, dan pilih **properti**.
3. Navigasikan ke tab **driver** dan pilih **Roll Back driver**. <br>
Catatan: jika ini tidak tersedia atau keabu-abuan, pilih **tidak** dari opsi di bawah ini untuk berpindah ke langkah berikutnya.
4. Anda mungkin harus memulai ulang PC sebelum perubahan ini diterapkan.

**Uninstall dan menginstal ulang driver tampilan Anda:**

1. Pilih **mulai**, ketik **Device Manager**, dan pilih **Device Manager** dari hasil.
2. Memperluas bagian **Adapter tampilan** , klik kanan Adapter tampilan Anda, ands pilih **uninstall perangkat**. 
3. Pilih kotak di samping **Hapus perangkat lunak pengandar untuk perangkat ini** dan pilih **bongkar**.<br>
Catatan: Anda mungkin diminta untuk me-restart komputer Anda pada tahap ini. Pastikan untuk menuliskan petunjuk yang tersisa sebelum Anda memulai ulang.
4. Buka Manajer perangkat lagi.
5. Perluas bagian **Adapter tampilan** , klik kanan pada Adapter tampilan Anda, dan pilih **Perbarui driver**.
6. Pilih **pencarian secara otomatis untuk memperbarui perangkat lunak pengandar** dan ikuti petunjuk penginstalan.