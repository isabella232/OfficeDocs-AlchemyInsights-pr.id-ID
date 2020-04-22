---
title: 1491-pencarian-tidak-kembali-diharapkan-hasil
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709230"
---
# <a name="content-search-not-returning-expected-results"></a>Pencarian konten tidak mengembalikan hasil yang diharapkan

Saat menjalankan pencarian konten dari Microsoft 365 keamanan & kepatuhan pusat, Anda mungkin menerima hasil pencarian tak terduga. Pertimbangkan hal berikut yang dapat memengaruhi hasil penelusuran Anda:

- **Lokasi konten dan kondisi penelusuran**: Pastikan Anda telah memilih lokasi konten yang tepat dan kondisi penelusuran. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membelah ke dalam beberapa pencarian.

- **Item yang diindeks sebagian**: [item yang diindeks sebagian](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam perkiraan hasil penelusuran. Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan pencarian.

- **Pencarian kegagalan**: ketika mencari sejumlah besar kotak pesan (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan galat pencarian, dengan kode GALAT seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi pencarian hanya untuk lokasi konten yang gagal. Lihat [artikel ini](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) untuk informasi lebih lanjut.
