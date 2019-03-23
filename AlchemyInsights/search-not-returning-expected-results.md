---
title: 1491-Search-not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776085"
---
# <a name="content-search-not-returning-expected-results"></a>Cari konten tidak kembali hasil yang diharapkan

Ketika menjalankan pencarian konten dari Office 365 keamanan & Compliance Center, Anda mungkin menerima hasil pencarian tak terduga. Pertimbangkan hal berikut yang dapat mempengaruhi hasil pencarian Anda:

- **Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten yang tepat dan Cari kondisi. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membagi menjadi beberapa pencarian.

- **Sebagian diindeks item**: [sebagian diindeks item](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam hasil pencarian yang diperkirakan. Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan Cari.

- **Cari kegagalan**: ketika mencari sejumlah besar kotak pesan (kotak pesan lebih dari 100.000), Anda mungkin mendapatkan Cari kesalahan, dengan kode kesalahan seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi hanya mencari lokasi konten yang gagal. Lihat [artikel ini](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) untuk informasi lebih lanjut.
