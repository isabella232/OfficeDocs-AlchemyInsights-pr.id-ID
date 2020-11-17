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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="7eae5-102">Pertanyaan tentang cara menggunakan Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="7eae5-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7eae5-103">Unduh alat penyebaran Office dari [Pusat Unduhan Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="7eae5-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="7eae5-104">Setelah mengunduh file, Jalankan file eksekusi ekstraksi mandiri, yang berisi alat penyebaran Office yang dapat dijalankan (setupodt.exe) dan file konfigurasi sampel (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="7eae5-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="7eae5-105">**Untuk mengecualikan atau menghapus aplikasi Microsoft 365 untuk produk perusahaan dari komputer klien:**</span><span class="sxs-lookup"><span data-stu-id="7eae5-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="7eae5-106">Saat menginstal aplikasi Microsoft 365 untuk perusahaan, Anda bisa mengecualikan produk tertentu.</span><span class="sxs-lookup"><span data-stu-id="7eae5-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="7eae5-107">Untuk melakukannya, ikuti langkah-langkah untuk menginstal Office dengan ODT, tapi sertakan elemen ExcludeApp dalam file konfigurasi Anda.</span><span class="sxs-lookup"><span data-stu-id="7eae5-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="7eae5-108">Misalnya, file konfigurasi ini menginstal semua aplikasi Microsoft 365 untuk produk perusahaan kecuali Publisher:</span><span class="sxs-lookup"><span data-stu-id="7eae5-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="7eae5-109">Gambaran umum tentang alat penyebaran Office</span><span class="sxs-lookup"><span data-stu-id="7eae5-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

