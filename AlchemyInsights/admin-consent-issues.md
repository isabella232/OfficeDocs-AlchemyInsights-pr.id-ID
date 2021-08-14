---
title: Masalah persetujuan admin
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952576"
---
# <a name="admin-consent-issues"></a>Masalah persetujuan admin

1. Aktifkan alur [kerja persetujuan admin](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) untuk mengizinkan pengguna meminta persetujuan administrator secara langsung dari layar persetujuan.

1. Jika Anda atau pengguna aplikasi Anda melihat kesalahan yang tidak diharapkan selama proses persetujuan, lihat artikel ini untuk langkah-langkah pemecahan masalah: Kesalahan yang tidak diharapkan saat melakukan persetujuan [terhadap aplikasi.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Pelajari selengkapnya tentang [persetujuan Admin di platform identitas Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)cara kerja perintah persetujuan, dan cara mengevaluasi permintaan untuk persetujuan admin tingkat [penyewa.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)

1. Aplikasi yang berintegrasi dengan platform identitas Microsoft mengikuti model otorisasi yang memberikan kontrol kepada pengguna dan administrator tentang bagaimana data dapat diakses. Implementasi model otorisasi telah diperbarui pada titik akhir platform identitas Microsoft, dan mengubah bagaimana aplikasi harus berinteraksi dengan pengguna platform identitas Microsoft. Lihat [Izin dan persetujuan di platform identitas Microsoft titik akhir](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) untuk mendapatkan gambaran umum tentang model otorisasi ini, termasuk lingkup, izin, dan persetujuan.