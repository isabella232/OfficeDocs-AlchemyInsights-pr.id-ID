---
title: Laporan log audit SharePoint klasik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509603"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Log audit SharePoint dan OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Log audit klasik SharePoint

SPO warisan audit bermigrasi ke log audit terpadu (UAL). Semua Laporan Audit warisan SPO sekarang akan didukung melalui UAL, dan sinyal audit warisan telah dipindahkan ke UAL.

Perubahan utama:

* Pemangkasan ini tidak tersedia sebagai kemampuan.
* Memilih peristiwa tertentu untuk mengaudit tidak tersedia. Lihat [dokumen ini](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap dari peristiwa yang diaudit yang tersedia secara default.
* Opsi **Lokasi** di bawah **laporan kustom** tidak tersedia.
* **Membuka atau men-download dokumen** peristiwa opsi ini tidak tersedia.

[Mengkonfigurasi pengaturan audit untuk koleksi situs](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint dan OneDrive modern terpadu audit log dari kepatuhan

* [Mengaktifkan/menonaktifkan pencatatan audit terpadu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Tidak ada konfigurasi tambahan yang diperlukan dalam SharePoint atau OneDrive.

Menggunakan pencarian pengelogan audit untuk memeriksa aktivitas file, folder (s), pengguna, izin:

* [Aktivitas file dan halaman](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivitas folder](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Berbagi dan mengakses aktivitas permintaan](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivitas sinkronisasi](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Kegiatan administrasi situs](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Untuk informasi selengkapnya tentang cara mengambil peristiwa ini, lihat [pencarian audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
