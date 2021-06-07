---
title: Masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794006"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux

Artikel ini memandu Anda dalam langkah-langkah mengidentifikasi masalah kinerja pertahanan Microsoft untuk Titik Akhir di Linux.

Penting untuk memverifikasi terlebih dahulu bahwa masalah yang Anda alami telah diatasi dengan [versi terbaru.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Untuk memulai penyelidikan, lihat [Memecahkan masalah kinerja Pertahanan Microsoft untuk Titik Akhir di Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Pengecualian

Pengecualian bisa membantu mengurangi masalah kinerja. Tinjau pengecualian Anda sebelum memulai sehingga setiap risiko tambahan diketahui dan didokumentasikan.

Untuk informasi selengkapnya, [lihat Mengonfigurasi dan memvalidasi pengecualian bagi Pertahanan Microsoft untuk Titik Akhir di Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Jika Anda memiliki beberapa file & folder untuk dikecualikan dan semuanya berada di puncak yang sama, mungkin sebaiknya jangan sertakan titik naik. Dimulai dengan rilis Februari 101.22.80, Anda dapat tidak menyertakan seluruh puncak gunung.

Misalnya, jika /mnt/backup adalah mountpoint, Anda dapat menambahkan /mnt/backup ke daftar pengecualian dengan menjalankan perintah ini:

`$ mdatp exclusion folder add –path /mnt/backup`

**Catatan**: Menambahkan pengecualian meningkatkan risiko malware yang tidak terdeteksi dan harus ditangani serta diterapkan dengan hati-hati.

## <a name="need-help"></a>Perlu Bantuan?

Untuk membantu Anda dengan cara yang paling efisien, kumpulkan data diagnostik sebelum membuka kasus dukungan.
