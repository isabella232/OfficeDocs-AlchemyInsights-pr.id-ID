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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068026"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Log audit SharePoint dan OneDrive

**SharePoint dan OneDrive modern terpadu audit log dari kepatuhan**

- [Mengaktifkan/menonaktifkan pencatatan audit terpadu](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Tidak ada konfigurasi tambahan yang diperlukan dalam SharePoint atau OneDrive.

- Menggunakan pencarian pengelogan audit untuk memeriksa aktivitas file, folder (s), pengguna, izin:

    - [Aktivitas file dan halaman](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Aktivitas folder](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Berbagi dan mengakses aktivitas permintaan](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Aktivitas sinkronisasi](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Kegiatan administrasi situs](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Untuk informasi selengkapnya tentang cara mengambil peristiwa ini, lihat [pencarian audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Log audit klasik SharePoint**

Kami bermigrasi SPO warisan audit untuk terpadu audit log (UAL). Ini pada dasarnya berarti bahwa semua SPO warisan audit laporan sekarang akan didukung melalui UAL, dan warisan audit sinyal telah dipindahkan ke UAL.

Perubahan utama:

- Pemangkasan sebagai kemampuan tidak tersedia.
- Bagian di mana Anda memilih peristiwa khusus untuk mengaudit tidak tersedia. Silakan lihat [dokumen ini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) untuk daftar lengkap dari peristiwa yang diaudit yang tersedia secara default.
- Opsi "lokasi" di bawah **laporan kustom** tidak tersedia. 
- "Membuka atau men-download dokumen" peristiwa ini tidak tersedia. 

