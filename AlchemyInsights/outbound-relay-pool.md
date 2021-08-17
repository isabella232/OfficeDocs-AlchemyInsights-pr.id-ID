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
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883134"
---
# <a name="outbound-relay-pool"></a>Relay pool keluar

Microsoft membuat beberapa perubahan pada konfigurasi untuk melakukan relai atau meneruskan email melalui Microsoft 365. Pesan dalam skenario tertentu diteruskan atau diteruskan melalui Microsoft 365 menggunakan kelompok relay khusus. Pesan yang dikirim dengan menggunakan relay pool bisa berakhir di folder email sampah penerima. Untuk informasi selengkapnya, lihat [Kolam renang pengiriman keluar](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Untuk menghindari skenario menggunakan relay pool, pastikan bahwa pesan yang diteruskan/diteruskan memenuhi salah satu kriteria berikut ini:

- Pengirim keluar adalah domain yang diterima dari penyewa.
- Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.
- DomainKeys Identified Mail (DKIM) di domain pengirim P2 akan masuk ketika pesan masuk Microsoft 365.
 
Pesan yang memenuhi kriteria di atas tidak diteruskan melalui relay pool.

Jika catatan MX untuk domain Anda di arahkan ke server pihak ketiga atau lokal, gunakan pemfilteran yang disempurnakan untuk memastikan validasi SPF sudah benar untuk email masuk dan untuk menghindari mengirim email melalui relay pool.

**Bagaimana kami dapat mengetahui apakah kami terkena dampak dari relay pool?**

Jika email yang Anda teruskan atau relai menggunakan salah satu kriteria di atas, pesan tidak akan relay pool. Namun, jika pesan dikirim melalui relay pool, IP server keluar ada dalam rentang 40.95.0.0/16 dan nama server keluar **menyertakan rly** dalam nama.

