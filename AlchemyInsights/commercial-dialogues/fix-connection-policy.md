---
title: Perbaiki kebijakan koneksi
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988111"
---
# <a name="fix-connection-policy"></a>Perbaiki kebijakan koneksi

Email ditandai aman dan dikirimkan ke kotak masuk pengguna karena alamat IP pengirim ditandai aman dalam kebijakan Filter Koneksi. Untuk meninjau kebijakan, lakukan hal berikut:

1. Masuk ke [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)lalu masuk ke Threat **management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Pada tab **Kustom,** pilih **Kebijakan filter koneksi**, lalu pilih Edit **kebijakan**.
3. Meninjau daftar **IP yang** Diizinkan. Lihat apakah **Brankas ini** diaktifkan.

    > [!NOTE]
    > Microsoft berlangganan ke sumber pihak ketiga dari pengirim tepercaya. Jika **Brankas** ini diaktifkan, pengirim tepercaya ini tidak akan ditandai sebagai spam. Saya merekomendasikan untuk memilih opsi ini, karena akan mengurangi jumlah positif palsu (email baik yang diklasifikasikan sebagai spam) yang Anda terima.
