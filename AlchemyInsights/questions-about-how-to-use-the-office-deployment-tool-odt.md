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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="0ac58-102">Pertanyaan tentang cara menggunakan alat penyebaran Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="0ac58-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="0ac58-103">Unduh alat penyebaran Office dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="0ac58-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="0ac58-104">Setelah men-download file, jalankan mengekstrak sendiri berkas yang dapat dijalankan, yang berisi alat penyebaran Office yang dapat dijalankan (setup. exe) dan berkas konfigurasi contoh (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="0ac58-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="0ac58-105">**Untuk mengecualikan atau menghapus Microsoft 365 aplikasi untuk produk perusahaan dari komputer klien:**</span><span class="sxs-lookup"><span data-stu-id="0ac58-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="0ac58-106">Saat memasang Microsoft 365 aplikasi untuk perusahaan, Anda dapat mengecualikan produk tertentu.</span><span class="sxs-lookup"><span data-stu-id="0ac58-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="0ac58-107">Untuk melakukannya, ikuti langkah untuk menginstal Office dengan ODT, namun sertakan elemen ExcludeApp di file konfigurasi Anda.</span><span class="sxs-lookup"><span data-stu-id="0ac58-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="0ac58-108">Sebagai contoh, berkas konfigurasi ini menginstal semua aplikasi Microsoft 365 untuk produk perusahaan kecuali Publisher:</span><span class="sxs-lookup"><span data-stu-id="0ac58-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="0ac58-109">Ikhtisar alat penyebaran Office</span><span class="sxs-lookup"><span data-stu-id="0ac58-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

