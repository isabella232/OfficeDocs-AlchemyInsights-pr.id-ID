---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312690"
---
# <a name="alert-policies"></a>Kebijakan pemberitahuan

Microsoft 365 berisi kebijakan pemberitahuan [default](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) yang memicu pemberitahuan untuk organisasi dengan langganan Microsoft 365 Enterprise atau Microsoft 365 E1/G1 Pemerintah AS, E3/G3, atau E5/G5. Oleh karena itu, admin mungkin menerima pemberitahuan email pemberitahuan yang dikirim oleh Office365Alerts@microsoft.com dengan baris subjek seperti "Pemberitahuan tingkat keparahan rendah: nama *kebijakan pemberitahuan*". Pemberitahuan pemberitahuan dikirim saat pemberitahuan dipicu untuk aktivitas umum, seperti saat pengguna:

- Buat aturan kotak masuk yang meneruskan email.
- Memberikan izin ke kotak surat mereka.
- Bagikan atau hapus sejumlah besar file dalam SharePoint berbagi file.
- Membuat pencarian eDiscovery dan mengekspor hasil pencarian.

Untuk meninjau dan bertindak pada pemberitahuan:

1. Lakukan salah satu langkah berikut ini:
   - Pada pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Peringatan**. Atau, untuk langsung masuk ke **halaman Peringatan,** gunakan <https://compliance.microsoft.com/compliancealerts> .
   - Di portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk **ke Insiden &** pemberitahuan \> **Pemberitahuan**. Atau, untuk langsung masuk ke **halaman Peringatan,** gunakan <https://security.microsoft.com/alerts> .
2. Klik pemberitahuan untuk menampilkan halaman flyout dengan informasi tentang pemberitahuan tersebut.

Anda dapat mengambil tindakan pada pemberitahuan, seperti menghapus aturan [kotak masuk yang mencurigakan.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Atau Anda bisa menutup pemberitahuan tersebut dengan mengklik **Atasi** pada halaman flyout pemberitahuan.

Untuk informasi selengkapnya tentang mengonfigurasi dan mengelola kebijakan pemberitahuan, lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Penting**: Peringatan pemberitahuan email dari Microsoft tidak akan pernah meminta Anda untuk melakukan hal berikut:

- Berikan kata sandi
- Memverifikasi detail keamanan akun Anda
- Mengautentikasi ulang diri Anda sendiri

Jika Anda menerima pesan email dengan tipe permintaan ini, pesan tersebut tidak dikirim oleh Microsoft dan seharusnya dianggap sebagai penipuan pengelabuan. Jika Anda menerima pesan dengan tipe permintaan ini, [laporkan pesan ke Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
