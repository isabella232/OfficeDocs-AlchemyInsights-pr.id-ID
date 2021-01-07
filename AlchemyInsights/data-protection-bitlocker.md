---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778196"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi BitLocker dengan Intune

Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows. Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk memproteksi perangkat menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Selain kebijakan perlindungan titik akhir, ada juga laporan enkripsi yang memberikan tampilan status enkripsi yang lebih mendetail untuk perangkat. Laporan ini bisa diakses dari MEM portal di bawah **perangkat > monitor**, lalu di bawah **konfigurasi** pilih [laporan enkripsi](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jika Anda menemukan BitLocker gagal untuk diaktifkan seperti yang diharapkan atau bahwa profil yang digunakan untuk mengaktifkan BitLocker dalam keadaan kesalahan, silakan Tinjau laporan enkripsi untuk mendapatkan pemahaman yang lebih baik tentang mengapa perilaku tersebut terjadi.

Untuk menemukan detail tentang cara menginterpretasikan laporan termasuk berbagai nilai status enkripsi, lihat [memantau enkripsi perangkat dengan Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Anda harus mengetahui bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis, yang dipicu tanpa penerapan kebijakan MDM. Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non-default dikonfigurasikan. Lihat Tanya Jawab Umum berikut untuk detail selengkapnya.

Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah kebijakan BitLocker di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

P: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?<br>
A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan [CSP CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Tidak semua edisi atau Build Windows mendukung BitLocker CSP. <br><br>

P: Bagaimana cara BitLocker diaktifkan di perangkat tanpa memerlukan interaksi pengguna akhir?<br>
A: selama prasyarat yang diperlukan terpenuhi, dimungkinkan untuk mengaktifkan BitLocker "Silent Encryption" melalui Intune. Lihat detail persyaratan perangkat dan pengaturan kebijakan contoh untuk mengaktifkan enkripsi hening dalam dokumen berikut: [mengaktifkan diam-diam enkripsi BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?<br>
J: Tidak. Untuk menerapkan pengaturan penyandian baru, drive harus didekripsi terlebih dahulu.<br><br>
**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi, yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS.
 
P: jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune, Apakah perangkat akan didekripsi saat kebijakan tersebut dihapus?<br>
A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.
 
P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki BitLocker yang diaktifkan, meskipun itu?<br>
A: Pengaturan "BitLocker enabled" dalam kebijakan Intune Compliance menggunakan klien Windows Device Health Attestation (DHA). Klien ini hanya mengukur status perangkat pada waktu boot. Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.
 
 