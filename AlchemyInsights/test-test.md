---
title: Persyaratan yang hilang dari SharePoint online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053516"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi BitLocker dengan Intune

Intune Endpoint Protection Policy dapat digunakan untuk mengonfigurasi pengaturan enkripsi Boitlocker untuk perangkat Windows seperti yang dijelaskan dalam pengaturan: Windows10 (dan yang lebih baru) untuk melindungi perangkat menggunakan Intune

Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 dukungan otomatis BitLocker enkripsi yang dipicu tanpa penerapan kebijakan MDM. Hal ini dapat mempengaruhi penerapan kebijakan jika pengaturan non default dikonfigurasi. Lihat FAQ untuk lebih jelasnya.


FAQ  Q: yang edisi Windows dukungan perangkat enkripsi menggunakan kebijakan perlindungan Endpoint?
 A: tataan di Intune Endpoint Protection kebijakan diterapkan menggunakan BitLocker CSP.Tidak semua edisi atau Build Windows mendukung BitLocker CSP. 
      Pada saat ini edisi Windows: Enterprise; Pendidikan, Mobile, Mobile Enterprise dan profesional (dari membangun 1809 dan seterusnya) yang didukung.




Q: jika perangkat sudah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan cipher (XTS-AES-128) akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu Re-enkripsi drive dengan pengaturan baru?

A: tidak. Untuk menerapkan pengaturan penyandian baru, kandar harus didekripsi terlebih dahulu.

Catatan untuk perangkat yang terdaftar dengan autopilot enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga Intune kebijakan dievaluasi yang memungkinkan pengaturan berbasis kebijakan untuk digunakan di tempat default OS




Q jika perangkat dienkripsi sebagai akibat dari penerapan kebijakan Intune akan didekripsi ketika kebijakan yang dihapus?

A: penghapusan Kebijakan enkripsi terkait tidak mengakibatkan dekripsi kandar yang dikonfigurasi.




T: Mengapa Intune kebijakan kepatuhan menunjukkan bahwa perangkat saya tidak memiliki "BitLocker diaktifkan" tapi itu?

A: "BitLocker diaktifkan" pengaturan di Intune kepatuhan kebijakan menggunakan klien Windows perangkat kesehatan Attestation (DHA). Klien ini hanya mengukur status perangkat pada saat boot. Jadi, jika perangkat belum reboot sejak enkripsi BitLocker selesai layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.