---
title: S/MIME di Outlook di web
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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010727"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mengenkripsi pesan email di Outlook

Microsoft 365 Enkripsi Pesan dibuat pada Microsoft Azure Manajemen Hak (Azure RMS), yang merupakan bagian dari Perlindungan Informasi Azure. Jika langganan Anda menyertakan Manajemen Hak Azure atau Perlindungan Informasi Azure, Anda tidak perlu melakukan tindakan apa pun untuk **mengaktifkan atau** mengaktifkan Layanan Manajemen Hak secara manual.

Berdasarkan umpan balik pelanggan, kami tidak akan lagi mengaktifkan Exchange email untuk mengenkripsi email keluar secara otomatis yang berisi tipe informasi sensitif tertentu di penyewa Anda secara default. Sebagai gantinya, kami menyediakan instruksi mendetail tentang bagaimana Anda dapat melakukannya sendiri. Untuk detail tambahan tentang cara membuat aturan transportasi untuk mengenkripsi informasi sensitif, lihat [artikel ini](https://aka.ms/OmeEtr).

- Jika menggunakan Outlook di Web (dulu **OWA**): Ketika menulis pesan email, cukup klik **Proteksi** di OWA. Ini akan menerapkan izin "Jangan teruskan". Klik **Ubah izin** dan pilih **Enkripsikan** untuk hanya mengenkripsi pesan.

- Jika menggunakan **klien Outlook**: Untuk mengirim pesan terenkripsi dari Outlook 2013 atau 2016, atau Outlook 2016 untuk Mac, pilih Izin Opsi , lalu pilih opsi proteksi yang Anda  >  perlukan.

- Untuk **mengenkripsi semua email yang** dikirim ke penerima tertentu atau organisasi mitra eksternal tertentu, Anda perlu membuat aturan transpor aliran email di Pusat Admin Exchange. Instruksi mendetail disediakan di [artikel dukungan ini.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

