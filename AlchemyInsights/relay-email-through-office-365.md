---
title: Relay email melalui Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898551"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email

Untuk mempelajari tentang opsi dan langkah-langkahnya, lihat [Cara menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email menggunakan Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Jika Anda memiliki perangkat atau aplikasi yang baru saja berhenti bekerja, masalah paling umum adalah:

- **Autentikasi terkait kesalahan saat menggunakan pengiriman klien SMTP Auth** Baru-baru ini kami membuat beberapa perubahan terkait cara kerja Autentikasi SMTP. Untuk informasi selengkapnya tentang cara mengatasi masalah, lihat bagian autentikasi yang tidak berhasil dari Memperbaiki masalah [dengan printer, pemindai,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)dan aplikasi LOB yang mengirim email menggunakan Microsoft 365 atau Office 365 .
- **Kami hanya menerima versi TLS 1.2 saat membuat koneksi yang aman ke Office 365** Jika menggunakan Koneksi aman (TLS), pastikan perangkat aplikasi Mendukung TLS 1.2. Untuk informasi selengkapnya, lihat [Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Untuk masalah dan solusi lainnya, lihat Memperbaiki masalah [dengan printer, pemindai,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)dan aplikasi LOB yang mengirim email menggunakan Microsoft 365 atau Office 365 .

Untuk melihat perangkat yang terpengaruh, masuk ke [laporan Klien Autentikasi SMTP](https://protection.office.com/mailflow/dashboard).

**Catatan**: Exchange Online tidak mengakomodasi skenario surat massal. Untuk mengirim email komersial massal (misalnya, buletin pelanggan), Anda harus menggunakan penyedia pihak ketiga yang mengkhususkan dalam layanan ini.
