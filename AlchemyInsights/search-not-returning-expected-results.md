---
title: 1491-pencarian-tidak dikembalikan-diharapkan-hasil
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740477"
---
# <a name="content-search-not-returning-expected-results"></a>Pencarian konten tidak mengembalikan hasil yang diharapkan

Saat menjalankan pencarian konten dari pusat kepatuhan & keamanan Microsoft 365, Anda mungkin menerima hasil pencarian yang tidak diharapkan. Pertimbangkan hal-hal berikut yang bisa mempengaruhi hasil pencarian Anda:

- **Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten dan kondisi pencarian yang tepat. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk memisahkan dalam beberapa pencarian.

- **Item yang diindeks sebagian**:  [item yang diindeks sebagian](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dari kotak surat disertakan dalam hasil pencarian yang diperkirakan. Namun, sebagian item yang diindeks dari situs di SharePoint dan OneDrive tidak disertakan dalam perkiraan pencarian.

- **Kegagalan pencarian**: saat mencari sejumlah besar kotak surat (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan kesalahan pencarian, dengan kode kesalahan seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi pencarian untuk lokasi konten gagal. Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.
