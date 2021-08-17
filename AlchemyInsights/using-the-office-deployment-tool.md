---
title: Menggunakan Office Deployment Tool
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083773"
---
# <a name="using-the-office-deployment-tool-odt"></a>Menggunakan Office Deployment Tool (ODT)

Anda menggunakan Office Deployment Tool (ODT) untuk Office 365 versi Office. Alat Office Penyebaran (setup.exe) dijalankan dari baris perintah dan menggunakan file XML konfigurasi untuk menentukan pengaturan apa yang diterapkan ketika menyebarkan Office.
  
1. Unduh versi terbaru Office Deployment Tool dari [Pusat Unduhan Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Gunakan Office [Customization Tool (OCT)](https://config.office.com) untuk memilih preferensi penggunaan Anda dan membuat file XML konfigurasi. Ekspor file konfigurasi dan letakkan secara lokal di folder yang sama tempat setup.exe berada.

    **Catatan:** Office penginstalan sering terjadi karena file konfigurasi yang salah konfigurasikan atau malformat. Untuk menghindari masalah tersebut, kami menyarankan Agar Anda menggunakan Office Customization Tool untuk membuat file konfigurasi. Anda juga bisa mengimpor file konfigurasi yang sudah ada ke Office Customization Tool.

3. Dari prompt perintah yang ditinggikan, beralihlah ke lokasi tempat setup.exe berada dan jalankan Office Deployment Tool dalam mode unduh dan tentukan file konfigurasi yang baru Saja Anda simpan. Dalam contoh ini, file konfigurasi dinamai Configuration.xml:

```setup.exe /download Configuration.xml```

4.Jalankan Office Deployment Tool dalam mode konfigurasi dan tentukan file konfigurasi.

```setup.exe /configure Configuration.xml```

**Catatan:** Anda harus menjalankan langkah ini dari komputer klien tempat Anda ingin menginstal Office dan Anda harus memiliki izin administrator lokal di komputer itu.

Untuk mempelajari selengkapnya tentang Office Deployment Tool untuk file Aplikasi Microsoft 365 untuk perusahaan penyebaran Anda, lihat Gambaran [umum Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Untuk detail selengkapnya tentang cara menggunakan Alat Office Kustomisasi, lihat [Gambaran Umum tentang Office Kustomisasi](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
