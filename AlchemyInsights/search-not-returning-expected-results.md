---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052713"
---
# <a name="content-search-not-returning-expected-results"></a>Pencarian Konten tidak mengembalikan hasil yang diharapkan

Ketika menjalankan Pencarian Konten dari pusat Microsoft 365 & Kepatuhan, Anda mungkin menerima hasil pencarian yang tidak diharapkan. Pertimbangkan hal-hal berikut yang dapat mempengaruhi hasil pencarian Anda:

- **Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten dan kondisi pencarian yang tepat. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membaginya menjadi beberapa pencarian.

- **Item terindeks sebagian:**  [Item yang diindeks sebagian dari](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kotak surat disertakan dalam perkiraan hasil pencarian. Namun, item yang diindeks sebagian dari situs SharePoint dan OneDrive tidak disertakan dalam perkiraan pencarian.

- Kegagalan **pencarian:** Saat mencari banyak kotak surat (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan kesalahan pencarian, dengan kode kesalahan seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi pencarian hanya untuk lokasi konten yang gagal. Lihat  [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi selengkapnya.
