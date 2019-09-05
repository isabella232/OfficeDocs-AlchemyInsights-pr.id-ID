---
title: S/MIME di Outlook di web
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752863"
---
# <a name="encrypt-email-messages-in-outlook"></a>Mengenkripsi pesan email di Outlook

Enkripsi pesan Office 365 dibuat di Microsoft Azure Rights Management (Azure RMS), yang merupakan bagian dari perlindungan informasi Azure. Jika langganan Anda mencakup pengelolaan hak Azure atau perlindungan informasi Azure, **Anda tidak perlu melakukan tindakan apa pun untuk mengaktifkan atau** mengaktifkan layanan manajemen hak secara manual.

Berdasarkan umpan balik pelanggan, kami tidak akan lagi mengaktifkan aturan aliran surat Exchange untuk secara otomatis mengenkripsi email keluar yang berisi jenis informasi sensitif tertentu di penyewa Anda secara default. Sebaliknya, kami menyediakan petunjuk rinci tentang bagaimana Anda dapat melakukannya sendiri. Untuk rincian tambahan tentang cara membuat aturan transpor untuk mengenkripsi informasi sensitif, lihat [artikel ini](https://aka.ms/OmeEtr).

- Jika menggunakan Outlook di web (sebelumnya **OWA**): saat menulis pesan email, cukup klik **melindungi** di OWA. Ini akan menerapkan izin "Jangan maju". Klik **Ubah izin** dan pilih **enkripsi** untuk hanya mengenkripsi pesan.

- Jika menggunakan **klien Outlook**: untuk mengirim pesan terenkripsi dari Outlook 2013 atau 2016, atau Outlook 2016 untuk Mac, pilih **opsi** > **izin**, kemudian pilih opsi perlindungan yang Anda butuhkan.

- Untuk secara **otomatis mengenkripsi semua email** yang dikirim ke penerima tertentu atau organisasi mitra eksternal, Anda perlu membuat aturan transpor aliran surat di pusat admin Exchange. Petunjuk terperinci disediakan dalam [artikel dukungan ini](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

