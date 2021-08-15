---
title: 'Kesalahan: Aturan di komputer ini tidak cocok'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981116"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Kesalahan: Aturan di komputer ini tidak cocok

Untuk melihat status pembaruan masalah yang diketahui ini, [lihat Aturan di komputer ini tidak cocok dengan aturan di Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tim Outlook telah menerapkan perbaikan dalam Build 12928.10000. Perbaikan telah tersedia di Insider Fast dan akan masuk ke Saluran Bulanan pada akhir Juni 2020. Setelah mendapatkan build tetap, Anda mungkin mendapatkan perintah "Aturan mana yang ingin Anda pertahankan" untuk kali terakhir. Pilih Server saat diminta, lalu masuk kembali Outlook mengaktifkan kembali setiap aturan yang dinonaktifkan.

Hingga perbaikan tersedia, silakan gunakan solusi berikut ini:

**Penanganan** masalah : Dalam laporan terbaru, masalah terjadi pada pengguna yang hanya membuat aturan klien Outlook desktop. Jika Anda terus mengalami masalah, pertimbangkan untuk menghapus aturan lalu buat dan edit aturan hanya di OWA (Outlook Web App) hingga masalah ini diatasi.

Jika tidak dapat menghapus aturan secara manual, Anda dapat menjalankan perintah Outlook ketika memulai Outlook dengan menjalankan Outlook.exe /cleanrules. Ini akan menghapus aturan klien dan server. Ia akan menghapus semua aturan untuk semua akun di dalam Outlook Profil. Perintah ini didokumentasikan lebih lanjut dalam artikel Sakelar baris perintah.

