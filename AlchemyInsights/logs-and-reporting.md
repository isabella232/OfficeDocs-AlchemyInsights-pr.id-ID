---
title: Log dan pelaporan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036004"
---
# <a name="logs-and-reporting"></a>Log dan pelaporan

[Tanya jawab umum pelaporan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) jawaban tanya jawab umum tentang pelaporan Azure Active Directory (Azure AD). Untuk informasi selengkapnya, lihat [pelaporan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**Memecahkan masalah dengan audit**

1. Jika Anda mengalami masalah saat melihat beberapa aktivitas audit dan aktivitas yang hilang ada dalam [Daftar](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)ini, silakan mengajukan tiket dukungan.
2. Jika Anda mengalami masalah dalam melihat setiap log audit dalam penyewa Anda, silakan file tiket dukungan.
3. Jika aktivitas audit Anda tidak muncul dengan segera di portal Azure, lihat [informasi latensi](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) kami dan file tiket dukungan jika keterlambatan melebihi latensi yang didokumentasikan.
4. [Penyimpanan log aktivitas Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Jika Anda tidak melihat semua audit untuk rentang tanggal yang Anda pilih, Anda bisa mengunduh hingga baris 250K (diurutkan menurut paling baru) dari masuk dari Azure portal. Untuk informasi selengkapnya, lihat [mengaudit aktivitas unduhan](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).

**Pemecahan masalah dengan masuk**

1. Anda hanya bisa melihat 30 hari terakhir data jika Anda memiliki lisensi Azure AD Premium (P1 atau P2) untuk penyewa Anda.
2. Masuk hanya tersedia untuk penyewa Premium Azure AD. Ini tidak tersedia untuk penyewa berlisensi gratis atau dasar.
3. Jika penyewa Anda memiliki lisensi P1 premium dan Anda tidak bisa melihat proses masuk, lihat [informasi latensi](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) kami dan file tiket dukungan jika keterlambatan melebihi latensi yang didokumentasikan.
4. Jika Anda tidak melihat semua masuk untuk rentang tanggal yang Anda pilih, perhatikan bahwa Anda bisa mengunduh hingga 250K baris (diurutkan menurut paling baru) dari masuk dari Azure portal. Untuk informasi selengkapnya, lihat [mengunduh aktivitas masuk](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**Memecahkan masalah laporan keamanan (pengguna berbendera berisiko, masuk berisiko)**

1. [Pengguna yang ditandai untuk laporan keamanan risiko](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Laporan masuk yang berisiko di portal Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Kejadian risiko Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
