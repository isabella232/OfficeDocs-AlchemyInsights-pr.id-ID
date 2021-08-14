---
title: Kesalahan alamat proksi saat membuat kotak surat bersama
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062911"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Kesalahan alamat proksi saat membuat kotak surat atau objek berkemampuan email lainnya

Jika Anda mencoba membuat objek dengan dukungan email (kotak surat, kotak surat bersama dll.) dan menerima kesalahan "Alamat proksi "SMTP:alias@domain.com" sudah digunakan...", alamat email yang Anda pilih sudah diambil oleh objek email aktif lain di organisasi Anda.
  
Anda harus menemukan pengguna, grup, kotak surat bersama atau folder publik yang memiliki alamat email ini dan menghapusnya atau mengubah alamat emailnya. Lalu Anda bisa membuat objek baru yang diaktifkan email dengan alamat email yang di bebaskan. Gunakan Cari di halaman Beranda untuk menemukannya. Anda juga bisa menggunakan perintah Exchange Online PowerShell berikut untuk mencarinya:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jika tidak ingin menghapus alamat email yang sudah ada, pilih alamat email baru untuk objek baru yang Anda buat.
  