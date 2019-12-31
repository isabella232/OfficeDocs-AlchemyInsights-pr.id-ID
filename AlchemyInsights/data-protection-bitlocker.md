---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908713"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi BitLocker dengan Intune

 Intune Endpoint Protection Policy dapat digunakan untuk mengkonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows. Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk melindungi perangkat yang menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 dukungan otomatis BitLocker enkripsi, yang dipicu tanpa penerapan kebijakan MDM. Hal ini dapat mempengaruhi penerapan kebijakan jika pengaturan non-default dikonfigurasi. Lihat FAQ berikut untuk detail selengkapnya.
 
Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah BitLocker kebijakan di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 Q: yang edisi Windows dukungan perangkat enkripsi menggunakan kebijakan perlindungan Endpoint?<br>
 A: pengaturan pada kebijakan perlindungan akhir Intune diterapkan menggunakan [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Tidak semua edisi atau versi Windows mendukung BitLocker CSP. <br><br>
      Saat ini, berikut edisi Windows yang didukung: perusahaan, pendidikan, Mobile, Mobile Enterprise, dan profesional (membangun 1809 dan yang lebih baru).
 
Q: jika perangkat sudah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu Re-enkripsi drive dengan pengaturan baru?<br>
A: tidak. Untuk menerapkan pengaturan penyandian baru, kandar harus didekripsi terlebih dahulu.<br><br>
**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga Intune kebijakan dievaluasi, yang memungkinkan pengaturan berbasis kebijakan untuk digunakan di tempat OS asali.
 
Q: jika perangkat dienkripsi sebagai akibat dari penerapan kebijakan Intune, akan didekripsi ketika kebijakan yang dihapus?<br>
A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi kandar yang dikonfigurasi.
 
T: Mengapa kebijakan kepatuhan Intune menunjukkan bahwa perangkat saya tidak memiliki BitLocker diaktifkan, meskipun itu?<br>
A: "BitLocker diaktifkan" pengaturan kebijakan kepatuhan Intune menggunakan klien Windows perangkat kesehatan Attestation (DHA). Klien ini hanya mengukur status perangkat pada saat boot. Jadi, jika perangkat belum reboot sejak enkripsi BitLocker selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.
 
 