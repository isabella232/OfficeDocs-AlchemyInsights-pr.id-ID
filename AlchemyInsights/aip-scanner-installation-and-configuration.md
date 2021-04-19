---
title: 'Pemindai AIP: penginstalan dan konfigurasi'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821666"
---
# <a name="aip-scanner-installation-and-configuration"></a>Pemindai AIP: penginstalan dan konfigurasi

**Untuk menginstal pemindai AIP, ikuti panduan yang disarankan:**

1. Jika Anda memutakhirkan dan tidak melakukan penginstalan yang bersih, pastikan Anda telah mengikuti panduan untuk memutakhirkan pemindai Perlindungan Informasi Azure dan untuk klien label yang terpadu, lihat memutakhirkan pemindai [Perlindungan](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)Informasi [Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Verifikasi bahwa Anda mematuhi semua [persyaratan pengaturan infrastruktur jaringan dan Firewall.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Pastikan kebijakan [Anda diatur ke](https://docs.microsoft.com/azure/information-protection/configure-policy) label otomatis atau memiliki label default di kebijakan tersebut.
4. Pastikan bahwa tipe file yang relevan dikonfigurasi untuk label/proteksi seperti yang dijelaskan dalam [Tipe file yang didukung oleh klien Perlindungan Informasi Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Selain itu, jika ingin mengubah perilaku default, ikuti panduan berikut: [Mengubah tingkat proteksi default file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verifikasi bahwa akun pengguna yang dikonfigurasi untuk menjalankan layanan pemindai memiliki izin untuk mengakses semua penyimpanan yang dikonfigurasi.
6. Jika Anda masih mengalami masalah, silakan ekspor log pemindai dan tambahkan ke tiket dukungan Anda.

**Mengekspor log Pemindai Perlindungan Informasi Azure**

1. Navigasikan ke %localappdata%\Microsoft\MSIP di bawah konteks pengguna yang menjalankan layanan pemindai.
2. Zip semua konten di bawah folder MSIP.
3. Simpan log ke lokasi pilihan, lalu lampirkan ke permintaan layanan Anda.
4. Anda juga bisa menggunakan [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Untuk informasi tambahan, lihat:**
- [Menyebarkan pemindai Perlindungan Informasi Azure untuk mengklasifikasikan dan melindungi file secara otomatis](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Menentukan dan menggunakan parameter Token untuk Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Menjalankan siklus penemuan dan menampilkan laporan untuk pemindai](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Tinjau dokumentasi Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Persyaratan untuk Perlindungan Informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Unduh klien Perlindungan Informasi Azure](https://www.microsoft.com/download/details.aspx?id=53018)
