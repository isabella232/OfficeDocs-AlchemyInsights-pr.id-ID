---
title: Pemecahan masalah Microsoft Defender untuk Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801446"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Pemecahan masalah Microsoft Defender untuk Office 365

- Apakah Anda melihat keterlambatan dalam pengiriman pesan? Gunakan opsi [pengiriman dinamis](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dalam kebijakan lampiran aman ATP Anda. Ini akan membantu menghindari keterlambatan pesan sekaligus melindungi penerima dari file berbahaya.

- Apakah Anda ingin melaporkan positif palsu atau negatif palsu ke Microsoft? Gunakan [link](https://www.microsoft.com/wdsi/filesubmission/) ini untuk mengirim file untuk dianalisis.

- Apakah Anda tahu bahwa Anda bisa mengaktifkan proteksi link aman untuk email internal yang dikirim antar penerima di dalam organisasi Anda? Ikuti langkah-langkah ini:

  1. Masuk ke [https://protection.office.com](https://protection.office.com) dan masuk dengan akun administrator global atau administrator keamanan.

  2. Di panel navigasi kiri di bawah **manajemen ancaman** , pilih **Policy** \> **link aman** kebijakan.

  3. Di **kebijakan yang berlaku untuk seluruh bagian organisasi** , pilih kebijakan dan klik **Edit** .

  4. Di bawah **pengaturan** , Aktifkan **Terapkan tautan aman ke pesan yang dikirim dalam organisasi** .
