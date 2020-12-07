---
title: Dukungan Microsoft Edge untuk Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583581"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Dukungan Microsoft Edge untuk Microsoft Defender Application Guard

Didesain untuk Windows 10 dan Microsoft Edge, aplikasi Guard menggunakan pendekatan isolasi perangkat keras yang memungkinkan pengguna menavigasi situs tidak tepercaya dari dalam wadah yang terisolasi dan Hyper-V yang diaktifkan, dipisahkan dari sistem operasi host.

Admin perusahaan menentukan daftar situs web tepercaya, sumber daya awan, dan jaringan internal. Saat pengguna mengunjungi situs yang tidak ada di daftar, Microsoft Edge akan membuka situs tersebut dalam wadah. Ini berarti bahwa jika situs ternyata berbahaya, PC host akan tetap terlindung dan penyerang tidak bisa masuk ke data perusahaan.

Penginstalan ekstensi dalam wadah didukung sebagai Microsoft Edge versi 81, dan dapat dikontrol melalui kebijakan. Alamat updateURL yang akan digunakan dalam kebijakan ExtensionInstallForcelist harus ditambahkan sebagai sumber daya netral dalam kebijakan isolasi jaringan yang digunakan oleh penjaga aplikasi.

Untuk informasi selengkapnya, lihat [dukungan Microsoft Edge untuk Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
