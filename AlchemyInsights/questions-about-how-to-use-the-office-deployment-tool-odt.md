---
title: Pertanyaan tentang cara menggunakan Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959686"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pertanyaan tentang cara menggunakan Office Deployment Tool (ODT)

Unduh Office Deployment Tool dari [Pusat Unduhan Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Setelah mengunduh file, jalankan file yang dapat mengekstrak sendiri file yang dapat dieksekusi, yang berisi Office Deployment Tool yang dapat dijalankan (setup.exe) dan sampel file konfigurasi (configuration.xml).
  
 **Untuk mengecualikan atau menghapus Aplikasi Microsoft 365 untuk perusahaan produk dari komputer klien:**
  
Saat menginstal Aplikasi Microsoft 365 untuk perusahaan, Anda dapat mengecualikan produk tertentu. Untuk melakukannya, ikuti langkah-langkah untuk Office dengan ODT, tetapi sertakan elemen ExcludeApp dalam file konfigurasi Anda. Misalnya, file konfigurasi ini menginstal semua produk Aplikasi Microsoft 365 untuk perusahaan kecuali Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Gambaran umum Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

