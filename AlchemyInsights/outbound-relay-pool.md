---
title: Relay pool keluar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381717"
---
# <a name="outbound-relay-pool"></a>Relay pool keluar

Microsoft membuat beberapa perubahan pada konfigurasi untuk melakukan relai atau meneruskan email melalui Microsoft 365. Pesan dalam skenario tertentu diteruskan atau diteruskan melalui Microsoft 365 menggunakan kelompok relay khusus. Pesan yang dikirim dengan menggunakan relay pool mungkin berakhir di folder email sampah penerima. Untuk informasi selengkapnya, lihat [Kolam renang pengiriman keluar](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Untuk menghindari skenario menggunakan relay pool, pastikan bahwa pesan yang diteruskan/diteruskan memenuhi salah satu kriteria berikut ini:

- Pengirim keluar adalah domain yang diterima dari penyewa.
- Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.
- DomainKeys Identified Mail (DKIM) di domain pengirim P2 akan masuk ketika pesan masuk ke Microsoft 365.
 
Pesan yang memenuhi kriteria di atas tidak diteruskan melalui relay pool.

Jika catatan MX untuk domain Anda di arahkan ke server pihak ketiga atau lokal, gunakan pemfilteran yang disempurnakan untuk memastikan validasi SPF sudah benar untuk email masuk dan untuk menghindari mengirim email melalui relay pool.

**Bagaimana kami dapat mengetahui apakah kami terkena dampak dari relay pool?**

Jika email yang Anda teruskan atau relai menggunakan salah satu kriteria di atas, pesan tidak akan diteruskan melalui relay pool. Namun, jika pesan dikirim melalui relay pool, IP server keluar ada dalam rentang 40.95.0.0/16 dan nama server keluar **menyertakan rly** dalam nama.

