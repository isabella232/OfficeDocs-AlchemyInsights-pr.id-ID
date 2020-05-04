---
title: Menggunakan alat penyebaran Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010870"
---
# <a name="using-the-office-deployment-tool-odt"></a>Menggunakan alat penyebaran Office (ODT)

Anda menggunakan alat penyebaran Office (ODT) untuk menyebarkan Office 365 versi Office. Alat penyebaran Office (setup. exe) dijalankan dari baris perintah dan menggunakan konfigurasi XML file untuk menentukan apa pengaturan untuk menerapkan saat menyebarkan Office.
  
1. Download versi terbaru dari alat penyebaran Office dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Gunakan [alat kustomisasi Office (Oct)](https://config.office.com) untuk memilih preferensi penyebaran dan membuat file XML konfigurasi. Ekspor file konfigurasi dan tempatkan secara lokal pada folder yang sama di mana setup. exe berada.

    **Catatan:** Masalah penginstalan Office biasanya terjadi karena berkas konfigurasi yang salah dikonfigurasi atau terformat. Untuk menghindari masalah tersebut, kami sarankan Anda menggunakan alat kustomisasi Office untuk membuat berkas konfigurasi. Anda juga dapat mengimpor berkas konfigurasi yang ada ke alat kustomisasi Office.

3. Dari wantian perintah yang ditinggikan, beralih ke lokasi di mana setup. exe berada dan menjalankan alat penyebaran Office dalam mode download dan menentukan file konfigurasi yang baru saja Anda simpan. Dalam contoh ini, berkas konfigurasi bernama Configuration. xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Jalankan alat penyebaran Office dalam mode konfigurasi dan menentukan berkas konfigurasi.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Catatan:** Anda harus menjalankan langkah ini dari komputer klien di mana Anda ingin menginstal Office dan Anda harus memiliki izin administrator lokal di komputer.

Untuk mempelajari selengkapnya tentang cara menggunakan alat penyebaran Office untuk Microsoft 365 aplikasi untuk skenario penyebaran perusahaan, lihat [Ikhtisar alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Untuk rincian lebih lanjut tentang cara menggunakan alat kustomisasi Office, lihat [Ikhtisar alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
