---
title: Menggunakan alat penyebaran Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085835"
---
# <a name="using-the-office-deployment-tool-odt"></a>Menggunakan Office Deployment Tool (ODT)

Anda menggunakan Office Deployment Tool (ODT) untuk menggunakan Office versi 365 Office. Office Deployment Tool (setupodt.exe) dijalankan dari baris perintah dan menggunakan file XML konfigurasi untuk menentukan pengaturan apa yang diterapkan saat menyebarkan Office.
  
1. Unduh versi terbaru Office Deployment tool dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Gunakan [alat kustomisasi Office (Oct)](https://config.office.com) untuk memilih preferensi penggunaan dan membuat file XML konfigurasi. Ekspor file konfigurasi dan tempatkan secara lokal di folder yang sama tempat setupodt.exe berada.

    **Catatan:** Masalah penginstalan Office umumnya terjadi karena file konfigurasi yang salah dikonfigurasi atau tidak diformat. Untuk menghindari masalah tersebut, kami menyarankan agar Anda menggunakan alat kustomisasi Office untuk membuat file konfigurasi. Anda juga dapat mengimpor file konfigurasi yang sudah ada ke alat kustomisasi Office.

3. Dari wantian perintah yang ditinggikan, alihkan ke lokasi tempat setupodt.exe berada dan jalankan alat penyebaran Office dalam mode Unduh dan tentukan file konfigurasi yang baru saja Anda simpan. Dalam contoh ini, file konfigurasi bernama Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Jalankan alat penyebaran Office dalam mode konfigurasi dan tentukan file konfigurasinya.

```setupodt.exe /configure Configuration.xml```

**Catatan:** Anda harus menjalankan langkah ini dari komputer klien yang ingin Anda instal Office dan Anda harus memiliki izin administrator lokal di komputer tersebut.

Untuk mempelajari selengkapnya tentang menggunakan Office Deployment Tool untuk aplikasi Microsoft 365 Anda untuk skenario penggunaan perusahaan, lihat [gambaran umum tentang alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Untuk detail selengkapnya tentang cara menggunakan alat kustomisasi Office, lihat [gambaran umum alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
