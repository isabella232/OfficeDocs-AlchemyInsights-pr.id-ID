---
title: Memindahkan pesan email ke kotak surat Arsip
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713649"
---
# <a name="move-email-to-the-archive-mailbox"></a>Memindahkan email ke kotak pesan arsip

1. Konfirmasikan bahwa **kotak pesan arsip** telah diaktifkan. Jika tidak, gunakan langkah dalam [artikel ini](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak surat Arsip.

2. Untuk mengarsipkan pesan secara otomatis ke kotak pesan arsip, tag penyimpanan dengan tindakan **Pindahkan ke arsip** harus ditetapkan ke diterapkan secara **otomatis ke seluruh Tag kotak pesan (default)**. Gunakan langkah di sini untuk membuat Tag: [tag default Arsip](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Selanjutnya, Tambahkan tag **Arsip** ke kebijakan retensi Anda. Di pusat admin Exchange, pilih **kebijakan retensi** > Tambahkan **tag Pindahkan ke arsip** ke kebijakan > **Simpan**.

4. Sekarang [tetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ke kotak pesan pengguna tertentu. Kebijakan yang sama akan diterapkan ke kotak surat **primer** dan **Arsip** .

Mungkin diperlukan untuk memaksa Managed folder Assistant (MFA) untuk menjalankan dan menerapkan pengaturan baru ke kotak surat pengguna. Jalankan perintah berikut saat [tersambung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) untuk memulai bantuan folder yang dikelola untuk kotak pesan tertentu:
  
Mulai-ManagedFolderAssistant-identitas<name of the mailbox>

Untuk informasi lebih lanjut tentang penyiapan kebijakan pengarsipan, lihat [menyiapkan kebijakan pengarsipan dan penghapusan untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  