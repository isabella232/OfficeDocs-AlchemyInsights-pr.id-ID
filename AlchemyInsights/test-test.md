---
title: Istilah yang hilang SharePoint Penyimpanan Istilah Online
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106429"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Mengaktifkan Enkripsi Bitlocker dengan Intune

Kebijakan Perlindungan Titik Akhir Intune dapat digunakan untuk mengonfigurasi pengaturan enkripsi Boitlocker untuk perangkat Windows seperti yang diuraikan dalam : Windows10 (dan yang lebih baru) untuk melindungi perangkat menggunakan Intune

Anda harus menyadari bahwa banyak perangkat baru yang menjalankan Windows 10 mendukung enkripsi bitlocker otomatis yang dipicu tanpa aplikasi kebijakan MDM. Ini bisa mempengaruhi aplikasi kebijakan jika pengaturan non default dikonfigurasi. Lihat FAQ untuk detail selengkapnya.


TANYA JAWAB UMUM: Edisi produk Windows mendukung enkripsi perangkat menggunakan Kebijakan Proteksi Titik Akhir?
A: Pengaturan dalam Kebijakan Perlindungan Titik Akhir Intune diimplementasikan menggunakan CSP Bitlocker.  Tidak semua edisi maupun build Windows mendukung CSP Bitlocker. Saat ini Windows Editions: Enterprise; Pendidikan, Seluler, Seluler Perusahaan, dan Profesional (dari build 1809 dan seterusnya) didukung.




T: Jika perangkat sudah dienkripsi dengan Bitlocker menggunakan pengaturan default OS untuk metode enkripsi dan kekuatan penentu (XTS-AES-128) akan menerapkan kebijakan dengan pengaturan yang berbeda secara otomatis memicu enkripsi ulang drive dengan pengaturan baru?

J: Tidak. Untuk menerapkan pengaturan penpheran baru, drive harus didekripsi terlebih dahulu.

Catatan Untuk perangkat yang sudah terdaftar dengan Autopilot, enkripsi otomatis yang akan terjadi selama OOBE tidak akan dipicu hingga kebijakan Intune dievaluasi yang memungkinkan pengaturan berbasis kebijakan untuk digunakan di tempat default OS




T Jika perangkat dienkripsi sebagai akibat dari aplikasi kebijakan Intune yang akan didekripsi saat kebijakan tersebut dihapus?

A: Penghapusan kebijakan terkait enkripsi NOT menghasilkan dekripsi drive yang dikonfigurasi.




T: Mengapa kebijakan Kepatuhan intune memperlihatkan bahwa perangkat saya tidak memiliki "Bitlocker Diaktifkan" tetapi ya?

A: Pengaturan "Bitlocker diaktifkan" dalam kebijakan kepatuhan intune menggunakan klien Windows Device Health Attestation (CLIENT). Klien ini hanya mengukur status perangkat pada saat boot. Jadi, jika perangkat belum dinyalakan ulang karena enkripsi bitlocker telah selesai, layanan klienED TIDAK akan melaporkan bitlocker sebagai aktif.