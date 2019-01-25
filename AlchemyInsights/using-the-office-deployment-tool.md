---
title: Menggunakan alat penyebaran kantor
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474487"
---
# <a name="using-the-office-deployment-tool-odt"></a>Menggunakan alat penyebaran kantor (ODT)

Anda menggunakan alat penyebaran kantor (ODT) untuk menyebarkan versi Office 365 kantor. Kantor penyebaran alat (setup.exe) dijalankan dari baris perintah dan menggunakan file konfigurasi XML untuk menentukan pengaturan apa yang berlaku ketika deploying kantor.
  
1. Download versi terbaru dari Office penyebaran alat dari [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Gunakan [Alat kustomisasi Office (OCT)](https://config.office.com) untuk memilih preferensi penyebaran dan membuat file konfigurasi XML. Ekspor file konfigurasi dan tempat lokal di folder yang sama di mana setup.exe berada. 
    
    **Catatan:** Office instalasi masalah yang sering terjadi karena untuk misconfigured atau malformatted file konfigurasi. Untuk menghindari isu-isu tersebut, kami sarankan bahwa Anda menggunakan alat kustomisasi Office untuk membuat file konfigurasi. Anda juga dapat mengimpor file-file konfigurasi yang ada ke alat kustomisasi Office. 
    
3. Dari ditinggikan command prompt, beralih ke lokasi mana setup.exe berada dan menjalankan alat penyebaran kantor dalam download mode dan menentukan file konfigurasi yang baru saja diselamatkan. Dalam contoh ini, konfigurasi file bernama Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Menjalankan alat penyebaran kantor di mengkonfigurasi mode dan menentukan file konfigurasi.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Catatan:** Anda harus menjalankan langkah ini dari komputer klien yang Anda ingin menginstal Office dan Anda harus memiliki izin administrator lokal pada komputer. 
    
Untuk mempelajari lebih lanjut tentang menggunakan alat penyebaran kantor untuk skenario penggunaan Office 365 ProPlus Anda, lihat [ikhtisar dari kantor penyebaran alat](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Untuk detail lebih lanjut tentang cara menggunakan alat kustomisasi Office, lihat [Ikhtisar alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

