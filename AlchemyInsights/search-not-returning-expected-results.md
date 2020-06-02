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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510575"
---
# <a name="content-search-not-returning-expected-results"></a>Pencarian konten tidak mengembalikan hasil yang diharapkan

Saat menjalankan pencarian konten dari Microsoft 365 keamanan & kepatuhan pusat, Anda mungkin menerima hasil pencarian tak terduga. Pertimbangkan hal berikut yang dapat memengaruhi hasil penelusuran Anda:

- **Lokasi konten dan kondisi penelusuran**: Pastikan Anda telah memilih lokasi konten yang tepat dan kondisi penelusuran. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membelah ke dalam beberapa pencarian.

- **Item yang diindeks sebagian**: [item yang diindeks sebagian](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam perkiraan hasil penelusuran. Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan pencarian.

- **Pencarian kegagalan**: ketika mencari sejumlah besar kotak pesan (lebih dari 100.000 kotak surat), Anda mungkin mendapatkan galat pencarian, dengan kode GALAT seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi pencarian hanya untuk lokasi konten yang gagal. Lihat [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) untuk informasi lebih lanjut.
