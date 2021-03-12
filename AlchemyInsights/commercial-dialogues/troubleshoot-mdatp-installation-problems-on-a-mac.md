---
title: Memecahkan masalah penginstalan MDATP pada Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746301"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Memecahkan masalah penginstalan MDATP pada Mac

Jika penginstalan manual gagal, halaman **ringkasan** panduan penginstalan memperlihatkan kesalahan berikut:

"Terjadi galat selama penginstalan. Penginstal mengalami kesalahan yang menyebabkan penginstalan gagal. Hubungi produsen perangkat lunak untuk mendapatkan bantuan. "

Untuk penggunaan MDM, halaman juga memperlihatkan kegagalan penginstalan umum.

Meskipun kami tidak menampilkan kesalahan yang tepat kepada pengguna akhir, kami menyimpan file log dengan kemajuan instalasi, di **/Library/logs/Microsoft/mdatp/install.log**. Setiap sesi instalasi menambahkan file log ini. Untuk menampilkan hanya sesi instalasi terakhir, gunakan `sed` .

Untuk mempelajari selengkapnya, lihat [memecahkan masalah instalasi untuk Microsoft Defender ATP untuk Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
