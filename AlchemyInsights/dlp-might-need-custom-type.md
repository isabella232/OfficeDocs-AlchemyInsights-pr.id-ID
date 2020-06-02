---
title: DLP mungkin memerlukan jenis khusus
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507517"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin memerlukan jenis khusus

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**DLP mungkin memerlukan jenis informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda dapat mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** sendiri untuk melindungi data organisasi Anda.

Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.
  
 **Menyesuaikan jenis informasi sensitif internal**
  
Jika jenis informasi sensitif internal akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [menyesuaikan jenis informasi sensitif internal](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.
  
 **Membuat jenis informasi sensitif kustom**
  
Namun, jika Anda perlu mengidentifikasi dan melindungi berbagai jenis informasi sensitif sama sekali, Anda dapat [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.
  
**Membuat jenis informasi sensitif kustom di keamanan & kepatuhan pusat PowerShell**

Akhirnya, jika UI tidak menyediakan semua pilihan yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom di keamanan & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Dengan memulai dengan sebuah file XML, Anda dapat menggunakan setiap pilihan yang tersedia.
