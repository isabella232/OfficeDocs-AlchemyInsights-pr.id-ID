---
title: Beberapa objek memiliki alamat email yang sama sebagai identitas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439192"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Beberapa objek memiliki alamat email yang sama sebagai identitas

**Beberapa objek**

Salah satu dari alasan umum galat ini tidak dapat mengarahkan permintaan Outlook Web Access dengan benar di kehadiran beberapa objek yang memiliki alamat email yang sama sebagai identitas. Untuk menemukan objek ini, jalankan perintah berikut:

· Penerima Get<email address>

· Dapatkan-pengguna<email address>

· Get-pengguna <email address> -softdeleteduser

· Get-kontak<email address>

· Get-kotak surat <email address> -publicfolder

· Get-kotak surat <email address> -includesoftdeletedmailbox

· Get-kotak surat <email address> -inactivemailboxonly

Untuk mengatasi masalah ini, Hapus beberapa objek dengan identitas email yang sama dan pastikan bahwa ada satu objek dengan identitas email tertentu dan jenis Penerimanya adalah UserMailbox.

**Alamat yang sama digunakan untuk kotak surat bisnis dan konsumen**

Penyebab lain adalah ketika alamat yang sama digunakan untuk bisnis dan kotak surat konsumen. Dalam hal ini, pengguna harus mengubah alias konsumen utama mereka sampai Cafe mendukung skenario ini. Ini adalah kesalahan permanen yang tidak hilang tanpa intervensi.

Untuk detailnya, lihat [mengubah alamat email atau nomor telepon untuk akun Microsoft Anda](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).