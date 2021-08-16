---
title: DLP mungkin membutuhkan tipe kustom
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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030797"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin membutuhkan tipe kustom

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**DLP mungkin memerlukan tipe informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda bisa mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat tipe **informasi sensitif** kustom Anda sendiri untuk melindungi data organisasi Anda.

Misalnya, organisasi Anda mungkin perlu mengidentifikasi dan melindungi ID karyawan atau data lain dalam beberapa format khusus untuk organisasi Anda. Jika demikian, lihat artikel berikut ini untuk informasi selengkapnya.
  
 **Mengkustomisasi tipe informasi sensitif bawaan**
  
Jika tipe informasi sensitif bawaan akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, Anda bisa [mengkustomisasi tipe informasi sensitif bawaan.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Misalnya, Anda bisa menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.
  
 **Membuat tipe informasi sensitif kustom**
  
Tapi jika Anda perlu mengidentifikasi dan melindungi tipe informasi [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) sensitif yang berbeda sekaligus, Anda dapat membuat tipe informasi sensitif kustom di UI Pusat Kepatuhan & Keamanan.
  
**Membuat tipe informasi sensitif kustom di PowerShell Pusat & Kepatuhan**

Terakhir, jika UI tidak menyediakan semua opsi yang diperlukan, Anda dapat membuat tipe informasi sensitif kustom dalam PowerShell Pusat [Kepatuhan & Keamanan.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Dengan memulai dengan file XML, Anda bisa menggunakan setiap opsi yang tersedia.
