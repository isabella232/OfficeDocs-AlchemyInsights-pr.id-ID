---
title: Intune inventaris perangkat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439656"
---
# <a name="intune-device-inventory"></a>Intune inventaris perangkat

Bilah perangkat memberikan wawasan administrator ke perangkat di bawah manajemen di Intune pada setiap perangkat. Informasi yang ditampilkan meliputi: perangkat keras, aplikasi yang ditemukan, status kepatuhan perangkat, dan status konfigurasi perangkat.

Data inventaris untuk perangkat keras dan aplikasi yang ditemukan dikumpulkan pada siklus tujuh hari. Aplikasi dan elemen spesifik perangkat keras yang dilaporkan berbeda tergantung pada sistem operasi perangkat dan apakah perangkat tersebut dimiliki secara pribadi atau perusahaan.

Untuk informasi selengkapnya, lihat [Lihat rincian perangkat di Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

Q: saya tidak menerima daftar lengkap persediaan aplikasi yang hadir pada perangkat Windows Intune-terdaftar. Mengapa tidak?

A: saat ini, hanya aplikasi modern yang terdaftar untuk PC Windows 10 yang diidentifikasi sebagai perangkat korporat. Intune tidak mengumpulkan informasi tentang aplikasi Win32 diinstal pada perangkat ini.

T: Mengapa nomor telepon tidak dikumpulkan dari semua perangkat?

A: telepon dikategorikan sebagai perangkat korporat di Intune tidak diidentifikasi dengan nomor telepon penuh ketika, misalnya, Anda menjalankan laporan inventaris perangkat seluler. Membawa-Anda-sendiri-nomor telepon perangkat selalu ditutupi sebagian dengan tanda bintang (* * * *), dan hanya menampilkan empat digit terakhir.