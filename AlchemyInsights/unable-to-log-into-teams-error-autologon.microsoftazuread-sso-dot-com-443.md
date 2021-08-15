---
title: Tidak dapat masuk ke Teams karena kesalahan autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038403"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Tidak dapat masuk ke Teams karena kesalahan autologon.microsoftazuread-sso dot com: 443

Jika SSO Tanpa Hambatan diaktifkan sebagai otentikasi O365, URL "autologon.microsoftazuread-sso.com" mungkin perlu ditambahkan ke Situs Intranet.  Jika sebelumnya sudah ditambahkan ke Situs Tepercaya dan SSO Tanpa Hambatan sedang digunakan, situs harus dihapus dari Situs Tepercaya.

Tinjau [Daftar Periksa Pemecahan Masalah SSO Tanpa Hambatan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Ikuti langkah-langkah ini untuk menambahkan URL ke daftar Situs Intranet:

1. Buka Internet Explorer dengan mengklik tombol **Mulai**. Dalam kotak pencarian, ketik Internet Explorer, lalu klik **Internet Explorer** dalam daftar hasil.
2. Klik **Alat**, lalu klik **Opsi Internet**.
3. Klik tab **Keamanan**.
4. Sekarang klik **Situs Intranet Lokal** lalu klik tombol **situs** lalu tombol **Tingkat Lanjut**.
5. Masukkan URL Situs Web dan klik **Tambahkan**.
6. Setelah selesai, klik **Tutup**.

Untuk informasi selengkapnya, lihat [Dokumentasi untuk penyebaran SSO Tanpa Hambatan untuk O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (mencakup proses berbasis Kebijakan untuk menambahkan URL ke Situs Intranet di Langkah 3).
