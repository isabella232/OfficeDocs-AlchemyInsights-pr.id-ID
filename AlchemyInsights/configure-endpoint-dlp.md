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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657932"
---
# <a name="configure-endpoint-dlp"></a>Mengonfigurasi DLP Titik Akhir

DLP Titik Akhir Microsoft memungkinkan Anda memperluas kemampuan pemantauan dan proteksi DLP ke informasi sensitif di perangkat Windows 10. Setelah perangkat dimasukkan ke manajemen perangkat, Anda dapat membuat kebijakan DLP untuk menerapkan tindakan perlindungan pada item. Penjelajah Aktivitas dapat digunakan untuk memantau aktivitas bagi item sensitif. Untuk informasi selengkapnya, lihat [Onboarding perangkat ke manajemen perangkat](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Untuk memulai dengan DLP Titik Akhir:

- Pastikan Anda memiliki lisensi SKU/langganan yang sesuai. Untuk informasi selengkapnya, lihat [lisensi SKU/langganan](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Periksa izin yang diperlukan untuk mengaktifkan manajemen perangkat, mengakses halaman onboarding, atau mengaktifkan/menonaktifkan pemantauan perangkat. Untuk informasi selengkapnya, lihat [Izin](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Masukkan perangkat ke manajemen Perangkat dengan mengikuti prosedur perangkat onboarding. Untuk informasi selengkapnya, lihat [Perangkat onboarding](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Buat kebijakan DLP untuk melindungi item sensitif Anda. Untuk penjelasannya, lihat [Skenario kebijakan DLP titik akhir](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Untuk informasi selengkapnya tentang DLP Titik Akhir Microsoft, lihat [Pelajari tentang pencegahan kehilangan data Titik Akhir Microsoft 365 (pratinjau)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Langkah-langkah Pengumpulan Data Penting, jika Dukungan diperlukan:**

1. Unduh [MDATP Client Analyzer Preview.](https://aka.ms/betamdatpanalyzer)
1. Jalankan alat tersebut sebagai Admin dari jendela cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Ketika diminta dengan **Masukkan jumlah menit untuk mengumpulkan penelusuran:**, masukkan jumlah menit yang diperlukan untuk menjalankan skenario.
1. Jalankan skenario.

Kumpulkan output file Zip untuk diberikan kepada agen Dukungan.
