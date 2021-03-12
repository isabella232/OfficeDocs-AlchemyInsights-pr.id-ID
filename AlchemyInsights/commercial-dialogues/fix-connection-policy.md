---
title: Memperbaiki kebijakan koneksi
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746749"
---
# <a name="fix-connection-policy"></a>Memperbaiki kebijakan koneksi

Email ditandai aman dan dikirim ke kotak masuk pengguna karena alamat IP pengirim ditandai aman di kebijakan filter koneksi. Untuk meninjau kebijakan, lakukan hal berikut:

1. Masuk ke [pusat kepatuhan & keamanan Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), lalu masuk ke kebijakan **manajemen ancaman**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Pada tab **kustom** , pilih **kebijakan filter koneksi**, lalu pilih **Edit kebijakan**.
3. Tinjau daftar **Perbolehkan IP** . Lihat apakah **daftar aman** diaktifkan.

    > [!NOTE]
    > Microsoft berlangganan ke sumber pihak ketiga pengirim tepercaya. Jika **daftar aman** diaktifkan, pengirim tepercaya ini tidak secara keliru ditandai sebagai spam. Saya merekomendasikan memilih opsi ini, karena akan mengurangi jumlah positif palsu (baik email yang diklasifikasikan sebagai spam) yang Anda terima.
