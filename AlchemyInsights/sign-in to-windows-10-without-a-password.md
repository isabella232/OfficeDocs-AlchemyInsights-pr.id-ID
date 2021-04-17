---
title: Masuk ke Windows 10 tanpa menggunakan kata sandi
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830549"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Masuk ke Windows 10 tanpa menggunakan kata sandi

Untuk menghindari harus mengetikkan kata sandi pada startup Windows, kami menyarankan Anda menggunakan salah satu opsi masuk aman Windows Hello, seperti PIN, pengenalan wajah, atau sidik jari, jika tersedia. Jika Anda benar-benar ingin menonaktifkan akses masuk yang aman, lihat instruksi "Masuk secara otomatis ke Windows 10" di bawah ini.

**Mengamankan alternatif Windows Hello dengan kata sandi akun**

Masuk ke **Pengaturan > Akun > opsi Masuk (atau** klik di [sini](ms-settings:signinoptions?activationSource=GetHelp)). Opsi masuk yang tersedia akan dicantumkan. Misalnya:

![Opsi masuk.](media/sign-in-options.png)

Klik atau ketuk salah satu opsi untuk mengonfigurasinya. Saat berikutnya Anda memulai atau membuka kunci Windows, Anda akan bisa menggunakan opsi baru sebagai ganti kata sandi. 

**Masuk ke Windows 10 secara otomatis**

**Catatan**: Masuk otomatis mudah, tetapi menghadirkan risiko keamanan, terutama jika PC Anda dapat diakses oleh beberapa orang. 

1. Klik atau ketuk **tombol** Mulai di Taskbar.

2. Ketik **netplwiz** dan tekan tombol Enter untuk membuka jendela Akun Pengguna.

3. Di **Akun Pengguna,** klik akun yang ingin Anda masuki secara otomatis saat Windows dimulai.

4. Kosongkan kotak centang "Pengguna harus memasukkan nama pengguna dan kata sandi untuk menggunakan komputer ini".

    ![Pengguna harus memasukkan nama pengguna dan opsi kata sandi.](media/users-must-enter-username.png)

5. Klik **OK**. Anda akan diminta untuk memasukkan dan mengonfirmasi kata sandi untuk akun yang dipilih. Klik **OK** untuk menyelesaikannya. Di waktu berikutnya Windows 10 dimulai, Windows 10 akan masuk secara otomatis ke akun yang Anda pilih.
