---
title: Konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573522"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge

Berikut ini adalah konsep autentikasi tingkat lanjut yang berlaku untuk Microsoft Edge:

**Autentikasi proaktif**

Saat Anda mengaktifkan kebijakan [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge akan mencoba mengautentikasi pengguna yang masuk secara proaktif melalui layanan Microsoft. Secara berkala, akan menggunakan layanan online untuk memeriksa manifest yang berisi konfigurasi yang mengatur autentikasi proaktif.

Manfaat: autentikasi proaktif memungkinkan autentikasi ke layanan utama, seperti halaman tab baru Office. Selain itu, jika Bing digunakan sebagai mesin pencari, autentikasi proaktif meningkatkan kinerja bilah alamat dan membantu menghasilkan hasil pencarian yang dipersonalisasi dengan kebutuhan bisnis Anda.

**Windows Hello CredUI untuk autentikasi NTLM**

Jika masuk tunggal (SSO) tidak tersedia ketika sebuah situs web mencoba untuk masuk ke pengguna melalui mekanisme NTLM atau Negotiate, fitur ini akan memungkinkan pengguna untuk berbagi kredensial OS dengan situs web dan untuk memenuhi tantangan autentikasi dengan menggunakan Windows Halo Cred UI. Alur masuk ini hanya akan muncul di Windows 10 dan hanya untuk pengguna yang tidak mendapatkan SSO selama tantangan NTLM atau negosiasi.

**Gunakan kata sandi yang disimpan untuk masuk secara otomatis**

Pengguna yang menyimpan kata sandi di Microsoft Edge dapat mengaktifkan masuk otomatis ke situs web tempat kredensial disimpan. Pengguna bisa mengaktifkan atau menonaktifkan fitur ini di edge://settings/passwords, dan Anda bisa mengonfigurasinya di kebijakan [manajer kata sandi](https://go.microsoft.com/fwlink/?linkid=2134622) .
