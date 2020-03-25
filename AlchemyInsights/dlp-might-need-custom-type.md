---
title: DLP mungkin memerlukan jenis khusus
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932661"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin memerlukan jenis khusus

**Penting**: banyak SharePoint online dan OneDrive pelanggan menjalankan aplikasi penting bisnis terhadap layanan yang berjalan di latar belakang. Ini termasuk migrasi konten, pencegahan kehilangan data (DLP), dan solusi pencadangan. Selama waktu yang belum pernah terjadi sebelumnya, kami mengambil langkah untuk memastikan bahwa SharePoint online dan layanan OneDrive tetap sangat tersedia dan dapat diandalkan untuk pengguna yang bergantung pada layanan lebih dari sebelumnya dalam skenario kerja jarak jauh.

Untuk mendukung tujuan ini, kami telah menerapkan batas pelambatan yang lebih ketat pada aplikasi latar belakang (migrasi, DLP dan solusi cadangan) selama jam siang hari kerja. Anda harus mengharapkan bahwa aplikasi ini akan mencapai throughput yang sangat terbatas selama waktu ini. Namun, selama jam malam dan akhir pekan untuk wilayah ini, Layanan akan siap untuk memproses volume permintaan yang jauh lebih tinggi dari aplikasi latar belakang.

**DLP mungkin memerlukan jenis informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda dapat mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat jenis informasi sensitif **kustom** sendiri untuk melindungi data organisasi Anda.

Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi id karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut untuk informasi lebih lanjut.
  
 **Menyesuaikan jenis informasi sensitif internal**
  
Jika jenis informasi sensitif internal akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda dapat [menyesuaikan jenis informasi sensitif internal](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Misalnya, Anda dapat menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.
  
 **Membuat jenis informasi sensitif kustom**
  
Namun, jika Anda perlu mengidentifikasi dan melindungi berbagai jenis informasi sensitif sama sekali, Anda dapat [membuat jenis informasi sensitif kustom](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) di UI pusat kepatuhan & keamanan.
  
**Membuat jenis informasi sensitif kustom di keamanan & kepatuhan pusat PowerShell**

Akhirnya, jika UI tidak menyediakan semua pilihan yang Anda butuhkan, Anda dapat [membuat jenis informasi sensitif kustom di keamanan & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Dengan memulai dengan sebuah file XML, Anda dapat menggunakan setiap pilihan yang tersedia.
