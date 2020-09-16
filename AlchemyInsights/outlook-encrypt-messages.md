---
title: S/MIME dalam Outlook di web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772265"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mengenkripsi pesan email di Outlook

Enkripsi pesan Microsoft 365 dibangun di Microsoft Azure Rights Management (Azure RMS), yang merupakan bagian dari proteksi informasi Azure. Jika langganan Anda meliputi manajemen hak Azure atau perlindungan informasi Azure, **Anda tidak perlu melakukan tindakan apa pun untuk mengaktifkan atau mengaktifkan** Layanan manajemen hak secara manual.

Berdasarkan umpan balik pelanggan, kami tidak lagi mengaktifkan aturan alur email Exchange untuk secara otomatis mengenkripsi email keluar yang berisi tipe informasi sensitif tertentu dalam penyewa Anda secara default. Sebagai gantinya, kami menyediakan instruksi mendetail tentang cara melakukannya sendiri. Untuk detail tambahan tentang cara membuat aturan transpor untuk mengenkripsi informasi sensitif, lihat [artikel ini](https://aka.ms/OmeEtr).

- Jika menggunakan Outlook di web (sebelumnya **OWA**): ketika menulis pesan email, cukup klik **proteksi** di OWA. Ini akan menerapkan izin "Jangan teruskan". Klik **Ubah izin** dan pilih **enkripsi** untuk mengenkripsi pesan saja.

- Jika menggunakan **klien Outlook**: untuk mengirim pesan yang dienkripsi dari Outlook 2013 atau 2016, atau Outlook 2016 untuk Mac, pilih **Options**  >  **izin**opsi, lalu pilih opsi proteksi yang Anda perlukan.

- Untuk secara **otomatis mengenkripsi semua email** yang dikirim ke penerima atau organisasi mitra eksternal tertentu, Anda perlu membuat aturan transpor aliran email di pusat admin Exchange. Instruksi mendetail disediakan dalam [artikel dukungan ini](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

