---
title: Persyaratan yang hilang dari penyimpanan istilah SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750454"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan enkripsi BitLocker dengan Intune

Kebijakan proteksi titik akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi Boitlocker untuk perangkat Windows seperti yang diuraikan dalam pengaturan: Windows10 (and later) untuk memproteksi perangkat menggunakan Intune

Anda harus menyadari bahwa banyak perangkat yang lebih baru yang menjalankan Windows 10 mendukung enkripsi BitLocker otomatis yang dipicu tanpa penerapan kebijakan MDM. Hal ini dapat berdampak pada penerapan kebijakan jika pengaturan non default dikonfigurasikan. Lihat Tanya Jawab Umum untuk detail selengkapnya.


Tanya Jawab Umum   p: yang edisi enkripsi perangkat dukungan Windows menggunakan kebijakan perlindungan titik akhir?
 A: pengaturan dalam kebijakan perlindungan titik akhir Intune diimplementasikan menggunakan CSP CSP.Tidak semua edisi maupun Build Windows mendukung BitLocker CSP. 
      Pada saat ini edisi Windows: Enterprise; Pendidikan, seluler, Mobile Enterprise dan Professional (dari Build 1809 seterusnya) didukung.




P: jika perangkat telah dienkripsi dengan BitLocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan penyandian (XTS-AES-128) akan menerapkan kebijakan dengan pengaturan berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?

J: Tidak. Untuk menerapkan pengaturan cipher baru, drive harus didekripsi terlebih dahulu.

Catatan untuk perangkat yang terdaftar dengan autopilot enkripsi otomatis yang akan terjadi selama OOBE tidak dipicu hingga kebijakan Intune dievaluasi yang memungkinkan pengaturan berbasis kebijakan digunakan di tempat default OS




P jika perangkat dienkripsi sebagai hasil dari penerapan kebijakan Intune akan didekripsi saat kebijakan tersebut dihapus?

J: penghapusan Kebijakan terkait enkripsi tidak mengakibatkan dekripsi drive yang dikonfigurasi.




P: Mengapa kebijakan kepatuhan Intune memperlihatkan bahwa perangkat saya tidak memiliki "BitLocker diaktifkan" tapi itu?

A: Pengaturan "BitLocker enabled" dalam kebijakan kepatuhan Intune menggunakan klien Windows Device Health Attestation (DHA). Klien ini hanya mengukur status perangkat pada waktu boot. Jadi jika perangkat belum diboot ulang karena enkripsi BitLocker telah selesai, Layanan klien DHA tidak akan melaporkan BitLocker sebagai aktif.