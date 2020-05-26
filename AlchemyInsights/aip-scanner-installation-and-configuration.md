---
title: 'AIP scanner: instalasi dan konfigurasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358099"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP scanner: instalasi dan konfigurasi

**Untuk memasang pemindai AIP, ikuti pedoman yang disarankan**:

1. Jika Anda meningkatkan dan tidak melakukan instalasi bersih, pastikan Anda telah mengikuti panduan untuk [meningkatkan pemindai perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) dan untuk klien pelabelan terpadu, lihat [meningkatkan pemindai perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verifikasi bahwa Anda mematuhi semua [firewall dan persyaratan pengaturan infrastruktur jaringan](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Pastikan kebijakan Anda [ditetapkan](https://docs.microsoft.com/azure/information-protection/configure-policy) ke pelabelan otomatis atau memiliki label default dalam kebijakan.
4. Pastikan bahwa jenis berkas yang relevan dikonfigurasi untuk label/perlindungan seperti yang dijelaskan dalam [jenis berkas yang didukung oleh klien perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Selain itu, jika Anda ingin mengubah perilaku default, ikuti panduan berikut: [mengubah tingkat perlindungan default file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verifikasikan bahwa akun pengguna yang dikonfigurasi untuk menjalankan layanan pemindai memiliki izin untuk mengakses semua repositori yang dikonfigurasi.
6. Jika Anda masih mengalami masalah, silakan ekspor log pemindai dan menambahkannya ke tiket dukungan Anda.

**Ekspor log perlindungan informasi Azure**

1. Navigasikan ke%localappdata%\Microsoft\MSIP di bawah konteks pengguna yang menjalankan layanan pemindai.
2. Zip semua isi di bawah MSIP folder.
3. Simpan log ke pilihan lokasi Anda, dan pasangkan ke permintaan layanan Anda.
4. Anda juga dapat menggunakan [ekspor-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Untuk informasi tambahan, lihat**:
- [Menyebarkan pemindai perlindungan informasi Azure untuk secara otomatis mengklasifikasikan dan melindungi file](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Tentukan dan Gunakan token parameter untuk set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Menjalankan penemuan siklus dan melihat laporan untuk pemindai](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Tinjau dokumentasi perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Persyaratan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Unduh klien perlindungan informasi Azure](https://www.microsoft.com/download/details.aspx?id=53018)
