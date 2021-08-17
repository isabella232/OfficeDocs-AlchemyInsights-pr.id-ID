---
title: Kebijakan Penyimpanan di Exchange Admin tidak berfungsi
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074935"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Kebijakan Penyimpanan di Exchange Admin

Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <-- di bagian atas halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dengan kebijakan penyimpanan.

Jika Anda mengalami masalah dengan kebijakan penyimpanan di Pusat Admin Exchange tidak berlaku untuk kotak surat atau item yang tidak berpindah ke kotak surat arsip, periksa hal berikut ini:

**Penyebab Akar:**

- **Asisten Folder** Terkelola belum memproses kotak surat pengguna. Asisten Folder Terkelola mencoba memproses setiap kotak surat di organisasi berbasis awan sekali setiap tujuh hari.

  **Solusi:** Jalankan Asisten Folder yang Dikelola.

- **RetentionHold** telah **diaktifkan** pada kotak surat. Jika kotak surat telah ditempatkan di Tempat Penyimpanan, kebijakan penyimpanan pada kotak surat tidak akan diproses selama waktu itu.

  **Solusi:** Periksa status pengaturan dan pembaruan Penyimpanan jika diperlukan. Untuk detailnya, lihat [Penyimpanan Kotak Surat.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Catatan:** Jika kotak surat lebih kecil dari 10 MB, Asisten Folder Yang Dikelola tidak akan memproses kotak surat secara otomatis.
 
Untuk informasi selengkapnya tentang kebijakan penyimpanan di Exchange Admin Tingkat Lanjut, lihat:

- [Tag penyimpanan dan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) atau Menambahkan atau menghapus tag [penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Cara mengidentifikasi tipe penyimpanan yang ditempatkan di kotak surat](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
