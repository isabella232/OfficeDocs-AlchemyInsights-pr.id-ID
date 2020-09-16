---
title: Intune perangkat inventaris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667881"
---
# <a name="intune-device-inventory"></a>Intune perangkat inventaris

Bilah perangkat menyediakan wawasan administrator ke perangkat di bawah manajemen di Intune pada basis per perangkat. Informasi yang diperlihatkan meliputi: perangkat keras, aplikasi yang ditemukan, status kepatuhan perangkat, dan status konfigurasi perangkat.

Inventaris data untuk perangkat keras dan ditemukan aplikasi dikumpulkan dalam siklus tujuh hari. Aplikasi dan elemen perangkat keras tertentu yang dilaporkan berbeda tergantung pada sistem operasi perangkat dan apakah perangkat tersebut bersifat pribadi atau milik perusahaan.

Untuk informasi selengkapnya, lihat [melihat detail perangkat di Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

T: saya tidak menerima daftar inventaris lengkap tentang aplikasi yang ada di perangkat Windows yang didaftarkan Intune. Mengapa tidak?

J: saat ini, hanya aplikasi modern yang dicantumkan untuk PC Windows 10 yang diidentifikasi sebagai perangkat korporat. Intune tidak mengumpulkan informasi tentang aplikasi Win32 yang terinstal di perangkat ini.

P: Mengapa nomor telepon tidak dikumpulkan dari semua perangkat?

A: telepon yang dikategorikan sebagai perangkat korporat di Intune tidak diidentifikasi dengan nomor telepon lengkap mereka saat, misalnya, Anda menjalankan laporan inventaris perangkat seluler. Bawalah-Anda-sendiri-nomor telepon perangkat selalu ditutupi dengan tanda bintang (* * * *), dan hanya memperlihatkan empat digit terakhir.