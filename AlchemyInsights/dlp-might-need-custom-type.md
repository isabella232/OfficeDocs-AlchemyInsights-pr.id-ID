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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446694"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP mungkin membutuhkan tipe kustom

**Penting**: Selama masa-masa yang berat ini, kami mengambil langkah untuk memastikan bahwa SharePoint Online dan layanan OneDrive tetap memiliki ketersediaan yang tinggi. Silakan kunjungi [Penyesuaian Fitur Sementara SharePoint Online](https://aka.ms/ODSPAdjustments) untuk informasi selengkapnya.

**DLP mungkin memerlukan tipe informasi kustom**

Dengan kebijakan pencegahan kehilangan data (DLP), Anda bisa mengidentifikasi dan melindungi data sensitif di organisasi Anda. Dalam beberapa skenario, Anda mungkin perlu membuat tipe informasi sensitif kustom Anda sendiri untuk melindungi data organisasi Anda. Untuk informasi selengkapnya, [lihat Pelajari tentang tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) dan Definisi entitas tipe informasi [sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Untuk informasi selengkapnya tentang cara membuat tipe dan kebijakan informasi sensitif kustom, lihat: 

**Mengkustomisasi tipe informasi sensitif bawaan**

Jika tipe informasi sensitif bawaan akan memenuhi kebutuhan Anda hanya dengan beberapa tweak, lihat Mengkustomisasi [tipe informasi sensitif bawaan.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Misalnya, Anda bisa menambahkan atau menghapus kata kunci, atau menambahkan atau menghapus bukti pendukung seperti tanggal atau alamat.

**Membuat tipe informasi sensitif kustom**

Tapi jika Anda perlu mengidentifikasi dan melindungi tipe informasi sensitif yang berbeda sekaligus, Anda dapat membuat tipe informasi sensitif kustom dalam pusat kepatuhan Microsoft 365. Untuk informasi selengkapnya, lihat [Mulai menggunakan tipe informasi sensitif kustom](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Membuat tipe informasi sensitif kustom di PowerShell Pusat & Kepatuhan**

Terakhir, jika antarmuka pengguna tidak menyediakan semua opsi yang diperlukan, Anda dapat membuat tipe informasi sensitif kustom dalam PowerShell Pusat Kepatuhan & Keamanan. Dengan memulai dengan file XML, Anda bisa menggunakan setiap opsi yang tersedia. Untuk informasi selengkapnya, lihat [Membuat tipe informasi sensitif kustom menggunakan PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Untuk menguji kebijakan Anda di mode uji terlebih dahulu, lihat [Menerapkan kebijakan](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) dalam mode uji dan [Membuat, menguji, dan menyelaraskan kebijakan DLP](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 