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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731242"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi BitLocker dengan Intune

 Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi BitLocker untuk perangkat Windows. Untuk informasi selengkapnya, lihat [pengaturan Windows 10 (dan yang lebih baru) untuk memproteksi perangkat menggunakan Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Anda harus mengetahui bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis, yang dipicu tanpa penerapan kebijakan MDM. Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non-default dikonfigurasikan. Lihat Tanya Jawab Umum berikut untuk detail selengkapnya.
 
Untuk informasi tentang pemecahan masalah BitLocker, lihat [memecahkan masalah kebijakan BitLocker di Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**FAQ**

 P: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?<br>
 A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan [CSP CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Tidak semua edisi atau Build Windows mendukung BitLocker CSP. <br><br>
      Saat ini, edisi Windows berikut ini didukung: Enterprise, Education, Mobile, Mobile Enterprise, dan Professional (Build 1809 dan yang lebih baru).
 
P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128), akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?<br>
J: Tidak. Untuk menerapkan pengaturan penyandian baru, drive harus didekripsi terlebih dahulu.<br><br>
**Catatan:** Untuk perangkat yang terdaftar dengan autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi, yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS.
 
P: jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune, Apakah perangkat akan didekripsi saat kebijakan tersebut dihapus?<br>
A: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.
 
P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki BitLocker yang diaktifkan, meskipun itu?<br>
A: Pengaturan "BitLocker enabled" dalam kebijakan Intune Compliance menggunakan klien Windows Device Health Attestation (DHA). Klien ini hanya mengukur status perangkat pada waktu boot. Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.
 
 