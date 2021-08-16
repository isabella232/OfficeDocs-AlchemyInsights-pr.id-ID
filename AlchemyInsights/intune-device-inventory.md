---
title: Inventaris Perangkat Intune
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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014075"
---
# <a name="intune-device-inventory"></a>Inventaris Perangkat Intune

Blade Perangkat memberikan wawasan administrator ke perangkat dalam manajemen di Intune setiap perangkat. Informasi yang diperlihatkan meliputi: Perangkat Keras, aplikasi yang ditemukan, status Kepatuhan Perangkat, dan status Konfigurasi Perangkat.

Data inventaris untuk perangkat keras dan aplikasi yang ditemukan dikumpulkan dalam siklus tujuh hari. Aplikasi dan elemen tertentu dari perangkat keras yang dilaporkan berbeda bergantung pada sistem operasi perangkat dan apakah perangkat tersebut dimiliki secara pribadi atau milik perusahaan.

Untuk informasi selengkapnya, lihat [Lihat detail perangkat di Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

T: Saya tidak menerima daftar inventaris lengkap aplikasi yang ada di perangkat Windows Intune. Mengapa tidak?

A: Saat ini, hanya aplikasi modern yang tercantum Windows 10 PC yang diidentifikasi sebagai perangkat perusahaan. Intune tidak mengumpulkan informasi tentang aplikasi Win32 yang diinstal di perangkat ini.

P: Mengapa nomor telepon tidak dikumpulkan dari semua perangkat?

A: Telepon yang dikategorikan sebagai perangkat perusahaan di Intune tidak diidentifikasi dengan nomor telepon lengkapnya ketika, misalnya, Anda menjalankan laporan inventaris perangkat seluler. Nomor telepon bawa-anda-sendiri selalu diseminggikan sebagian dengan tanda bintang (****), dan hanya memperlihatkan empat digit terakhir.