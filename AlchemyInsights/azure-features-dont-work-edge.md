---
title: Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812870"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Apa yang harus dilakukan jika fitur Azure tidak berfungsi dengan baik Microsoft Edge

Microsoft Edge memiliki masalah umum yang terkait dengan zona keamanan yang mungkin memengaruhi cara pengguna Azure masuk ke Windows admin lokal. Untuk informasi selengkapnya, lihat [Masalah umum di Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Jika mengalami masalah dalam menggunakan fitur Azure dengan Microsoft Edge, cobalah langkah berikut:

1. Pada menu Mulai, di bilah **Pencarian,** ketik **Opsi Internet**, lalu pilih opsi.
1. Di **Properti Internet**, pilih **tab** Keamanan.
1. Pilih **Situs tepercaya**, lalu pilih **Situs.**
1. Tambahkan URL gateway Anda, serta <https://login.microsoftonline.com> , dan , lalu pilih <https://login.live.com> **Tutup**.
1. Di **Properti Internet**, pilih tab Privasi. 
1. Di bagian Pemblokir Pop-up, pilih **Pengaturan**. Tambahkan URL gateway Anda, serta <https://login.microsoftonline.com> , dan , lalu pilih <https://login.live.com> **Tutup**.