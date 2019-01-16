---
title: Pertanyaan tentang bagaimana menggunakan alat penyebaran kantor (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294412"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pertanyaan tentang bagaimana menggunakan alat penyebaran kantor (ODT)

Download Office penyebaran alat dari [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Setelah men-download file, menjalankan file eksekusi Self-extracting, yang berisi kantor alat penyebaran executable (setup.exe) dan sampel file konfigurasi (configuration.xml).
  
 **Untuk mengecualikan atau menghapus produk Office 365 ProPlus dari komputer klien:**
  
Ketika Anda menginstal Office 365 ProPlus, Anda dapat mengecualikan produk tertentu. Untuk melakukannya, ikuti langkah-langkah untuk menginstal Office dengan ODT, tetapi mencakup unsur ExcludeApp dalam file konfigurasi. Sebagai contoh, file konfigurasi ini menginstal semua produk Office 365 ProPlus kecuali penerbit:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Sekilas alat penyebaran kantor](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

