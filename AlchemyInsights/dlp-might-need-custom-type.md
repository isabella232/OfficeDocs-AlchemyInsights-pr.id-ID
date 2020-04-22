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
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704492"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin memerlukan jenis khusus

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**DLP mungkin memerlukan jenis informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda dapat mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** sendiri untuk melindungi data organisasi Anda.

Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.
  
 **Menyesuaikan jenis informasi sensitif internal**
  
Jika jenis informasi sensitif internal akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [menyesuaikan jenis informasi sensitif internal](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.
  
 **Membuat jenis informasi sensitif kustom**
  
Namun, jika Anda perlu mengidentifikasi dan melindungi berbagai jenis informasi sensitif sama sekali, Anda dapat [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.
  
**Membuat jenis informasi sensitif kustom di keamanan & kepatuhan pusat PowerShell**

Akhirnya, jika UI tidak menyediakan semua pilihan yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom di keamanan & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Dengan memulai dengan sebuah file XML, Anda dapat menggunakan setiap pilihan yang tersedia.
