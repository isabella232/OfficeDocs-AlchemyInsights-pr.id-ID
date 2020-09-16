---
title: Masuk ke Windows 10 tanpa menggunakan kata sandi
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719956"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Masuk ke Windows 10 tanpa menggunakan kata sandi

Untuk menghindari keharusan mengetikkan kata sandi di startup Windows, kami menyarankan agar Anda menggunakan salah satu opsi masuk Windows Hello yang aman, seperti PIN, pengenalan wajah, atau sidik jari, jika tersedia. Jika Anda benar-benar ingin menonaktifkan aman masuk, lihat instruksi "masuk otomatis ke Windows 10" di bawah ini.

**Mengamankan Windows Hello alternatif untuk kata sandi akun**

Masuk ke **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)). Opsi masuk yang tersedia akan dicantumkan. Misalnya:

![Opsi masuk.](media/sign-in-options.png)

Klik atau ketuk salah satu opsi untuk mengonfigurasinya. Saat berikutnya Anda memulai atau membuka kunci Windows, Anda akan dapat menggunakan opsi baru, bukan kata sandi. 

**Masuk secara otomatis ke Windows 10**

**Catatan**: masuk otomatis mudah, namun memperkenalkan risiko keamanan, terutama jika PC Anda dapat diakses oleh beberapa orang. 

1. Klik atau ketuk tombol **mulai** di taskbar.

2. Ketik **netplwiz** dan tekan tombol Enter untuk membuka jendela akun pengguna.

3. Di **akun pengguna**, klik akun yang ingin Anda masuki secara otomatis saat Windows dimulai.

4. Kosongkan kotak centang "pengguna harus memasukkan nama pengguna dan kata sandi untuk menggunakan komputer ini".

    ![Pengguna harus memasukkan opsi nama pengguna dan kata sandi.](media/users-must-enter-username.png)

5. Klik **OK**. Anda akan diminta untuk memasukkan dan mengonfirmasi kata sandi untuk akun yang Anda pilih. Klik **OK** untuk menyelesaikan. Saat berikutnya Windows 10 dimulai, akan otomatis masuk ke akun yang Anda pilih.
