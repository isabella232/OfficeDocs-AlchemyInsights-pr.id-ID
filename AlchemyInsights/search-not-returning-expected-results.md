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
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551418"
---
# <a name="content-search-not-returning-expected-results"></a>Cari konten tidak kembali hasil yang diharapkan

Ketika menjalankan pencarian konten dari Office 365 keamanan & Compliance Center, Anda mungkin menerima hasil pencarian tak terduga. Pertimbangkan hal berikut yang dapat mempengaruhi hasil pencarian Anda:

- **Lokasi konten dan kondisi pencarian**: Pastikan Anda telah memilih lokasi konten yang tepat dan Cari kondisi. Jika Anda menjalankan pencarian besar (dengan banyak lokasi), pertimbangkan untuk membagi menjadi beberapa pencarian.

- **Sebagian diindeks item**: [sebagian diindeks item](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dari kotak pesan disertakan dalam hasil pencarian yang diperkirakan. Namun, sebagian diindeks item dari situs di SharePoint dan OneDrive tidak termasuk dalam perkiraan Cari.

- **Cari kegagalan**: ketika mencari sejumlah besar kotak pesan (kotak pesan lebih dari 100.000), Anda mungkin mendapatkan Cari kesalahan, dengan kode kesalahan seperti CS008-009 dan CS012-002). Dalam kasus ini, coba lagi hanya mencari lokasi konten yang gagal. Lihat [artikel ini](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) untuk informasi lebih lanjut.
