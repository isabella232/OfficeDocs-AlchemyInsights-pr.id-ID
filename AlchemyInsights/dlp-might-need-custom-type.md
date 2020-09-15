---
title: DLP mungkin memerlukan tipe kustom
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712187"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin memerlukan tipe kustom

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**DLP mungkin memerlukan tipe informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda bisa mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat tipe informasi sensitif **kustom** Anda sendiri untuk melindungi data organisasi Anda.

Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format tertentu untuk organisasi Anda. Jika demikian, lihat artikel berikut ini untuk informasi selengkapnya.
  
 **Mengkustomisasi tipe informasi sensitif bawaan**
  
Jika tipe informasi sensitif bawaan akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [mengustomisasi tipe informasi sensitif bawaan](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Misalnya, Anda bisa menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti yang mendukung seperti tanggal atau alamat.
  
 **Membuat tipe informasi sensitif kustom**
  
Tapi jika Anda perlu mengidentifikasi dan melindungi tipe informasi sensitif yang berbeda secara bersamaan, Anda bisa [membuat tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.
  
**Membuat tipe informasi sensitif kustom di keamanan & pusat kepatuhan PowerShell**

Akhirnya, jika UI tidak menyediakan semua opsi yang Anda perlukan, Anda bisa [membuat tipe informasi sensitif kustom di pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Dengan memulai dengan file XML, Anda bisa menggunakan setiap opsi yang tersedia.
