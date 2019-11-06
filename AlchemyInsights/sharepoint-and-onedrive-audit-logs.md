---
title: Laporan log audit SharePoint klasik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992621"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Log audit SharePoint dan OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Log audit klasik SharePoint

SPO warisan audit bermigrasi ke log audit terpadu (UAL). Semua Laporan Audit warisan SPO sekarang akan didukung melalui UAL, dan sinyal audit warisan telah dipindahkan ke UAL.

Perubahan utama:

* Pemangkasan ini tidak tersedia sebagai kemampuan.
* Memilih peristiwa tertentu untuk mengaudit tidak tersedia. Lihat [dokumen ini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap dari peristiwa yang diaudit yang tersedia secara default.
* Opsi **Lokasi** di bawah **laporan kustom** tidak tersedia.
* **Membuka atau men-download dokumen** peristiwa opsi ini tidak tersedia.

[Mengkonfigurasi pengaturan audit untuk koleksi situs](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint dan OneDrive modern terpadu audit log dari kepatuhan

* [Mengaktifkan/menonaktifkan pencatatan audit terpadu](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Tidak ada konfigurasi tambahan yang diperlukan dalam SharePoint atau OneDrive.

Menggunakan pencarian pengelogan audit untuk memeriksa aktivitas file, folder (s), pengguna, izin:

* [Aktivitas file dan halaman](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Aktivitas folder](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Berbagi dan mengakses aktivitas permintaan](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivitas sinkronisasi](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Kegiatan administrasi situs](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Untuk informasi selengkapnya tentang cara mengambil peristiwa ini, lihat [pencarian audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
