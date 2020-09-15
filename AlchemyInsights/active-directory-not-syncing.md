---
title: Direktori aktif tidak disinkronkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697632"
---
# <a name="active-directory-not-syncing"></a>Direktori aktif tidak disinkronkan

Jika Anda menerima kesalahan sinkronisasi, seperti "tidak ada sinkronisasi terkini," atau pemberitahuan status sinkronisasi direktori di portal admin Office mengatakan, "terakhir disinkronkan lebih dari 3 hari yang lalu," mungkin ada yang tidak memiliki pengaturan yang salah atau izin yang tidak mencukupi untuk melakukan sinkronisasi.  

Menginstal ulang AADConnect dengan menggunakan pengaturan kilat mungkin mengatasi masalah dengan cepat:

1. [Unduh versi terbaru dari AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Ikuti instruksi untuk penginstalan Ekspresikan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Untuk informasi selengkapnya tentang akun Layanan AADConnect, lihat [AZURE AD Connect: akun dan izin](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
