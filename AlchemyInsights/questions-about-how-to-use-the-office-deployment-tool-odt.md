---
title: Pertanyaan tentang cara menggunakan alat penyebaran Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698061"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pertanyaan tentang cara menggunakan alat penyebaran Office (ODT)

Unduh alat penyebaran Office dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Setelah men-download file, jalankan mengekstrak sendiri berkas yang dapat dijalankan, yang berisi alat penyebaran Office yang dapat dijalankan (setup. exe) dan berkas konfigurasi contoh (Configuration. xml).
  
 **Untuk mengecualikan atau menghapus Microsoft 365 aplikasi untuk produk perusahaan dari komputer klien:**
  
Saat memasang Microsoft 365 aplikasi untuk perusahaan, Anda dapat mengecualikan produk tertentu. Untuk melakukannya, ikuti langkah untuk menginstal Office dengan ODT, namun sertakan elemen ExcludeApp di file konfigurasi Anda. Sebagai contoh, berkas konfigurasi ini menginstal semua aplikasi Microsoft 365 untuk produk perusahaan kecuali Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Ikhtisar alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

