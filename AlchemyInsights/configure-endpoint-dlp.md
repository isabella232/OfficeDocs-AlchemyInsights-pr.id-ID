---
title: Mengonfigurasi DLP Titik Akhir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892802"
---
# <a name="configure-endpoint-dlp"></a>Mengonfigurasi DLP Titik Akhir

DLP Titik Akhir Microsoft memungkinkan Anda memperluas kemampuan pemantauan dan proteksi DLP ke informasi sensitif di perangkat Windows 10. Setelah perangkat dimasukkan ke manajemen perangkat, Anda dapat membuat kebijakan DLP untuk menerapkan tindakan perlindungan pada item. Penjelajah Aktivitas dapat digunakan untuk memantau aktivitas bagi item sensitif. Untuk informasi selengkapnya, lihat [Onboarding perangkat ke manajemen perangkat](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Untuk memulai dengan DLP Titik Akhir:

- Pastikan Anda memiliki lisensi SKU/langganan yang sesuai. Untuk informasi selengkapnya, lihat [lisensi SKU/langganan](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Periksa izin yang diperlukan untuk mengaktifkan manajemen perangkat, mengakses halaman onboarding, atau mengaktifkan/menonaktifkan pemantauan perangkat. Untuk informasi selengkapnya, lihat [Izin](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Masukkan perangkat ke manajemen Perangkat dengan mengikuti prosedur perangkat onboarding. Untuk informasi selengkapnya, lihat [Perangkat onboarding](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Buat kebijakan DLP untuk melindungi item sensitif Anda. Untuk penjelasannya, lihat [Skenario kebijakan DLP titik akhir](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Untuk informasi selengkapnya tentang DLP Titik Akhir Microsoft, lihat [Pelajari tentang pencegahan kehilangan data Titik Akhir Microsoft 365 (pratinjau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Langkah-langkah Pengumpulan Data Penting, jika Dukungan diperlukan:**

1. Unduh [MDATP Client Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Jalankan alat tersebut sebagai Admin dari jendela cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Ketika diminta dengan **Masukkan jumlah menit untuk mengumpulkan penelusuran:**, masukkan jumlah menit yang diperlukan untuk menjalankan skenario.
1. Jalankan skenario.

Kumpulkan output file Zip untuk diberikan kepada agen Dukungan.
