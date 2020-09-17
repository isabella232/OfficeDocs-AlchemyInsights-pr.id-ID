---
title: Memindahkan pesan email ke kotak surat Arsip
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799783"
---
# <a name="move-email-to-the-archive-mailbox"></a>Memindahkan email ke kotak surat Arsip

Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <--di bagian atas Halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dalam memindahkan email ke kotak surat arsip mereka.

1. Konfirmasi bahwa **kotak surat Arsip** telah diaktifkan. Jika tidak, gunakan langkah-langkah dalam [artikel ini](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) untuk mengaktifkan kotak surat Arsip.

2. Untuk mengarsipkan pesan secara otomatis ke kotak surat arsip, tag penyimpanan dengan tindakan **Pindahkan ke arsip** harus diatur untuk diterapkan secara **otomatis ke seluruh Tag kotak surat (default)**. Gunakan langkah-langkah di sini untuk membuat Tag: [tag default Arsip](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Berikutnya, Tambahkan tag **Arsip** ke kebijakan penyimpanan Anda. Di pusat admin Exchange, pilih **kebijakan penyimpanan** > Tambahkan **tag Pindahkan ke arsip** ke kebijakan > **Simpan**.

4. Sekarang [tetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ke kotak surat pengguna tertentu. Kebijakan yang sama akan diterapkan ke kotak surat **Arsip** dan **utama** .

Mungkin diperlukan untuk memaksa bantuan folder yang dikelola (MFA) untuk menjalankan dan menerapkan pengaturan baru ke kotak surat pengguna. Jalankan perintah berikut ini saat [tersambung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) untuk memulai bantuan folder yang dikelola untuk kotak surat tertentu:
  
Mulai-ManagedFolderAssistant-identitas <name of the mailbox>

Untuk informasi selengkapnya tentang menyiapkan kebijakan arsip, lihat [menyetel kebijakan arsip dan penghapusan untuk kotak surat](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  