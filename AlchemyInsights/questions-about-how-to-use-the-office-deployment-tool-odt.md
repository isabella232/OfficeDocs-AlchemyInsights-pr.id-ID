---
title: Pertanyaan tentang cara menggunakan alat penyebaran Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553543"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pertanyaan tentang cara menggunakan alat penyebaran Office (ODT)

Unduh alat penyebaran Office dari [Microsoft download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Setelah men-download file, jalankan mengekstrak sendiri berkas yang dapat dijalankan, yang berisi alat penyebaran Office yang dapat dijalankan (setup. exe) dan berkas konfigurasi contoh (Configuration. xml).
  
 **Untuk mengecualikan atau menghapus produk Office 365 ProPlus dari komputer klien:**
  
Saat menginstal Office 365 ProPlus, Anda dapat mengecualikan produk tertentu. Untuk melakukannya, ikuti langkah untuk menginstal Office dengan ODT, namun sertakan elemen ExcludeApp di file konfigurasi Anda. Sebagai contoh, berkas konfigurasi ini menginstal semua produk Office 365 ProPlus kecuali Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Ikhtisar alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

