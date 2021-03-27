---
title: Konsep autentikasi tingkat lanjut berlaku untuk Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398587"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Konsep autentikasi tingkat lanjut berlaku untuk Microsoft Edge

Berikut adalah konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge:

**Autentikasi Proaktif**

Saat Anda mengaktifkan kebijakan [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge akan mencoba mengautentikasi pengguna yang masuk secara proaktif melalui layanan Microsoft. Pada interval reguler, layanan online akan menggunakan layanan untuk memeriksa manifes diperbarui yang berisi konfigurasi yang mengatur Autentikasi Proaktif.

Manfaat: Autentikasi Proaktif memungkinkan autentikasi untuk layanan kunci, seperti Halaman Tab Baru Office. Selain itu, jika Bing digunakan sebagai mesin pencarian, Autentikasi Proaktif meningkatkan kinerja bilah alamat dan membantu menghasilkan hasil pencarian yang dipersonalisasi sesuai kebutuhan bisnis Anda.

**CredUI Windows Hello untuk Autentikasi NTLM**

Jika masuk tunggal (SSO) tidak tersedia saat situs web mencoba untuk masuk kepada pengguna melalui mekanisme NTLM atau Negotiate, fitur ini akan memungkinkan pengguna untuk berbagi kredensial OS dengan situs web dan untuk memenuhi tantangan autentikasi dengan menggunakan Windows Hello Cred UI. Aliran masuk ini hanya akan muncul di Windows 10 dan hanya untuk pengguna yang tidak mendapatkan SSO selama NTLM atau tantangan Negosiasi.

**Menggunakan kata sandi yang disimpan untuk masuk secara otomatis**

Pengguna yang menyimpan kata sandi di Microsoft Edge dapat mengaktifkan akses masuk otomatis ke situs web tempat mereka menyimpan kredensial. Pengguna dapat mengaktifkan atau menonaktifkan fitur edge://settings/passwords, dan Anda dapat mengonfigurasinya dalam kebijakan [pengelola kata](https://go.microsoft.com/fwlink/?linkid=2134622) sandi.
