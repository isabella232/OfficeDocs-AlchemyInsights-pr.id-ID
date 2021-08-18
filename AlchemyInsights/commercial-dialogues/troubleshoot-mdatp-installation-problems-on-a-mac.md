---
title: Memecahkan masalah penginstalan MDATP di Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091037"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Memecahkan masalah penginstalan MDATP di Mac

Jika penginstalan manual gagal, **halaman** Ringkasan panduan penginstalan akan memperlihatkan kesalahan berikut:

"Terjadi kesalahan selama instalasi. Penginstal mengalami kesalahan yang menyebabkan instalasi gagal. Hubungi produsen perangkat lunak untuk mendapatkan bantuan."

Untuk penyebaran MDM, halaman juga memperlihatkan kegagalan penginstalan umum.

Meskipun kami tidak menampilkan kesalahan yang persis sama bagi pengguna akhir, kami menyimpan file log dengan kemajuan penginstalan, di **/Pustaka/Log/Microsoft/mdatp/install.log**. Setiap sesi instalasi ditambahkan ke file log ini. Untuk membuat output sesi instalasi terakhir saja, gunakan `sed` .

Untuk mempelajari selengkapnya, lihat [Memecahkan masalah penginstalan bagi ATP Pertahanan Microsoft untuk Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
