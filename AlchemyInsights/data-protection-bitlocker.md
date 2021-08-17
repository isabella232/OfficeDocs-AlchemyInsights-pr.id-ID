---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118597"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi Bitlocker dengan Intune

Kebijakan Perlindungan Titik Akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi Bitlocker untuk Windows Anda. Untuk informasi selengkapnya, lihat [Windows 10 (dan yang lebih baru) untuk melindungi perangkat menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Selain Kebijakan Proteksi Titik Akhir, ada juga Laporan Enkripsi yang menyediakan tampilan yang lebih mendetail tentang status enkripsi untuk perangkat. Laporan ini bisa diakses dari portal MEM di bawah **Perangkat > Monitor**, lalu di bawah **Konfigurasi** pilih [Enkripsi laporan](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jika anda merasa Bitlocker gagal diaktifkan seperti yang diharapkan atau profil yang digunakan untuk mengaktifkan Bitlocker berada dalam keadaan kesalahan, tinjau laporan enkripsi untuk mendapatkan pemahaman yang lebih baik tentang penyebab perilaku tersebut terjadi.

Untuk menemukan detail tentang cara menginterpretasikan laporan termasuk berbagai nilai status enkripsi, lihat [Memantau enkripsi perangkat dengan Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Anda harus menyadari bahwa banyak perangkat baru yang menjalankan Windows 10 mendukung enkripsi Bitlocker otomatis, yang dipicu tanpa aplikasi kebijakan MDM. Ini bisa mempengaruhi aplikasi kebijakan jika pengaturan non-default dikonfigurasi. Lihat FAQ berikut untuk detail selengkapnya.

Untuk informasi tentang memecahkan masalah bitlocker, lihat [Memecahkan masalah kebijakan BitLocker di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

T: Edisi produk Windows mendukung enkripsi perangkat menggunakan Kebijakan Proteksi Titik Akhir?<br>
A: Pengaturan dalam Kebijakan Perlindungan Titik Akhir Intune diimplementasikan menggunakan [CSP Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Tidak semua edisi atau build versi Windows mendukung CSP Bitlocker. <br><br>

T: Bagaimana Cara Bitlocker diaktifkan di perangkat tanpa memerlukan interaksi pengguna akhir?<br>
A: Selama prasyarat yang diperlukan terpenuhi, Anda dapat mengaktifkan Bitlocker "Enkripsi Tanpa Enkripsi" melalui Intune. Lihat detail persyaratan perangkat dan pengaturan kebijakan contoh untuk mengaktifkan enkripsi tanpa suara di dokumen berikut: Mengaktifkan Enkripsi [Bitlocker tanpa diam.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

T: Jika perangkat sudah dienkripsi dengan Bitlocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan penentu (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?<br>
J: Tidak. Untuk menerapkan pengaturanpher baru, drive harus didekripsi terlebih dahulu.<br><br>
**Catatan:** Untuk perangkat yang sudah terdaftar dengan Autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi, yang memungkinkan pengaturan berbasis kebijakan untuk digunakan sebagai tempat default OS.
 
T: Jika perangkat dienkripsi sebagai akibat dari aplikasi kebijakan Intune, apakah kebijakan tersebut akan didekripsi saat kebijakan tersebut dihapus?<br>
A: Penghapusan kebijakan terkait enkripsi NOT menghasilkan dekripsi drive yang dikonfigurasi.
 
T: Mengapa Kebijakan Kepatuhan Intune memperlihatkan bahwa perangkat saya tidak mengaktifkan Bitlocker?<br>
A: Pengaturan "Bitlocker diaktifkan" di Kebijakan Kepatuhan Intune menggunakan klien Windows Device Health Attestation (GDPR). Klien ini hanya mengukur status perangkat pada saat boot. Jadi, jika perangkat belum dinyalakan ulang setelah enkripsi Bitlocker selesai, layanan klienED TIDAK akan melaporkan Bitlocker sebagai aktif.
 
 