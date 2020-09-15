---
title: Laporan log audit SharePoint klasik
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662211"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Log audit SharePoint dan OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Log audit klasik SharePoint

Audit warisan SPO dimigrasikan ke log audit terpadu (UAL). Semua Laporan Audit warisan SPO kini akan didukung melalui UAL, dan sinyal audit warisan telah dimigrasikan ke UAL.

Perubahan tombol:

* Pemangkasan tidak tersedia sebagai kapabilitas.
* Memilih acara tertentu untuk diaudit tidak tersedia. Rujuk ke [dokumen ini](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap acara yang diaudit yang tersedia secara default.
* Opsi **Lokasi** di bawah **laporan yang dikustomisasi** tidak tersedia.
* Opsi acara **membuka atau mengunduh dokumen** tidak tersedia.

[Mengonfigurasi pengaturan audit untuk kumpulan situs](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint dan OneDrive modern Unified log audit dari kepatuhan

* [Mengaktifkan/menonaktifkan pembuatan log audit terpadu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Tidak diperlukan konfigurasi tambahan dalam SharePoint atau OneDrive.

Menggunakan pencarian pembuatan log audit untuk memeriksa aktivitas file, folder, pengguna, izin:

* [Aktivitas file dan halaman](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivitas folder](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktivitas permintaan akses dan berbagi](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivitas sinkronisasi](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivitas administrasi situs](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Untuk informasi selengkapnya tentang cara mendapatkan kembali acara ini, lihat [mencari log audit](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
