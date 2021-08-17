---
title: Mengidentifikasi aktivitas aturan kotak masuk dalam log audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891298"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Mengidentifikasi aktivitas aturan kotak masuk dalam log audit

Anda dapat menggunakan pencarian log audit dalam pusat kepatuhan Microsoft 365 menampilkan kejadian aturan kotak masuk (membuat, mengubah, dan menghapus aturan kotak masuk).

1. Lakukan salah satu langkah berikut ini:
   - Pada bagian pusat kepatuhan Microsoft 365 <https://compliance.microsoft.com> , masuk ke **Audit** \> **Solusi**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://compliance.microsoft.com/auditlogsearch> .
   - Pada portal Pertahanan Microsoft 365 di <https://security.microsoft.com> , masuk ke **Audit**. Atau, untuk langsung masuk ke **halaman Audit,** gunakan <https://security.microsoft.com/auditlogsearch> .

2. Pada tab **Pencarian** dari halaman **Audit,** konfigurasi pengaturan berikut ini:
   - **Rentang tanggal dan waktu**: Pilih rentang tanggal/waktu dalam **kotak** Mulai **dan** Akhir.
   - **Aktivitas**: Pilih satu atau beberapa nilai berikut:
     - **Aturan Kotak Masuk Barurule Membuat aturan kotak masuk Outlook Web App**
     - **Set-InboxRule Ubah aturan dari Outlook Web App**.
     - **Memperbarui aturan kotak masuk Outlook klien**

3. Bila Anda sudah selesai, klik **Cari.** Aktivitas akan muncul di halaman **Pencarian audit baru.**

4. Pilih aktivitas dalam hasil untuk membuka flyout detail. Informasi tentang pengaturan aturan kotak masuk ditampilkan di **bidang** Parameter.

Untuk informasi selengkapnya, lihat [Menentukan apakah pengguna telah membuat aturan kotak masuk](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
