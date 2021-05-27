---
title: Indikator tidak berfungsi menggunakan browser Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676470"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikator tidak berfungsi menggunakan browser Edge

Setelah Anda membuat Indikator, Indikator tidak digunakan oleh Edge (Smartscreen). Untuk informasi selengkapnya, [lihat Membuat indikator untuk IP dan URL/domain](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Langkah 1: Pastikan hal berikut ini

- Pastikan bahwa indikator sudah benar (tidak ada kesalahan ketik dalam IP/URL, tindakan yang benar, grup RBAC yang benar).
- Tunggu setidaknya 2 jam setelah membuat indikator untuk memperhitungkan latensi yang mungkin.
- Konfirmasi bahwa sistem telah onboarded ke Pertahanan Microsoft untuk Titik Akhir.
- Verifikasi bahwa sistem dapat berkomunikasi dengan Awan.
- Pastikan bahwa Smartscreen telah diaktifkan dan dapat dijangkau dengan masuk ke [situs uji](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Langkah 2: Memecahkan masalah yang potensial

- Pastikan klien memenuhi persyaratan. Untuk detailnya, [lihat Membuat indikator untuk IP dan URL/domain](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Pastikan Anda menjalankan versi terbaru browser Edge. Untuk mencari tahu versi terbaru, lihat [Mencari tahu versi uji Microsoft Edge Anda miliki](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Mulai ulang browser Edge.
- Navigasikan ke situs di mana Anda telah menyiapkan indikator. Jika situs tidak muncul seperti yang diharapkan, lanjutkan ke Langkah 3. 

## <a name="step-3-collect-data"></a>Langkah 3: Kumpulkan data

- Kumpulkan data **diagnostik MDEClientAnalyzer.** Untuk instruksinya, [lihat Masalah dengan mesin onboarding ke Pertahanan Microsoft untuk Titik Akhir](issues-with-onboarding-machines.md).
- Jika Anda telah nyaman menginstal dan mengumpulkan jejak Fiddler, lihat [Telerik Fiddler](http://www.telerik.com/fiddler).
- Jika Anda lebih memilih panduan dari Dukungan Microsoft, pilih ikon Dukungan di bawah ini untuk membuka kasus dukungan.
