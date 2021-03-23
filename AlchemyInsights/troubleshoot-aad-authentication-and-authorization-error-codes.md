---
title: Memecahkan masalah kode kesalahan autentikasi dan autentikasi Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036508"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Memecahkan masalah kode kesalahan autentikasi dan autentikasi Azure AD

Untuk mengatasi kode kesalahan dan autentikasi AAD (AADSTS), lakukan langkah-langkah berikut ini:

1. **Menangani kode kesalahan dalam aplikasi Anda**

- **Spesifikasi OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 , memberikan panduan tentang cara menangani kesalahan selama autentikasi menggunakan porsi kesalahan dari respons kesalahan.

    - **kesalahan**: string kode kesalahan yang bisa digunakan untuk mengelompokkan tipe kesalahan yang terjadi, dan harus digunakan untuk bereaksi terhadap kesalahan.
    - Bidang **kesalahan** memiliki beberapa nilai yang memungkinkan-Tinjau link dokumentasi protokol dan spesifikasi OAuth 2,0 untuk informasi selengkapnya tentang kesalahan tertentu dan cara bereaksi terhadapnya.

- Berikut ini adalah contoh respons kesalahan:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Informasi kode kesalahan pencarian saat ini**

- Kode kesalahan dan pesan dapat berubah. Untuk informasi terbaru, lihat https://login.microsoftonline.com/error halaman untuk menemukan deskripsi kesalahan, perbaikan, dan beberapa solusi yang disarankan.
- Anda juga dapat mencari dan memecahkan masalah [kode kesalahan Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) yang tercantum dalam [kode kesalahan pengesahan dan autentikasi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Mendapatkan bantuan**

- [Opsi dukungan dan bantuan untuk pengembang](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -jika Anda memerlukan jawaban untuk pertanyaan atau bantuan dalam memecahkan masalah yang tidak tercakup dalam dokumentasi kami, mungkin ada waktu untuk menghubungi pakar untuk bantuan. Artikel ini menyediakan beberapa saran untuk menjawab pertanyaan Anda saat Anda mengembangkan aplikasi yang berintegrasi dengan platform identitas Microsoft.








