---
title: Pertanyaan tentang cara menggunakan Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086159"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pertanyaan tentang cara menggunakan Office Deployment Tool (ODT)

Unduh alat penyebaran Office dari [Pusat Unduhan Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Setelah mengunduh file, Jalankan file eksekusi ekstraksi mandiri, yang berisi alat penyebaran Office yang dapat dijalankan (setupodt.exe) dan file konfigurasi sampel (configuration.xml).
  
 **Untuk mengecualikan atau menghapus aplikasi Microsoft 365 untuk produk perusahaan dari komputer klien:**
  
Saat menginstal aplikasi Microsoft 365 untuk perusahaan, Anda bisa mengecualikan produk tertentu. Untuk melakukannya, ikuti langkah-langkah untuk menginstal Office dengan ODT, tapi sertakan elemen ExcludeApp dalam file konfigurasi Anda. Misalnya, file konfigurasi ini menginstal semua aplikasi Microsoft 365 untuk produk perusahaan kecuali Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Gambaran umum tentang alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

