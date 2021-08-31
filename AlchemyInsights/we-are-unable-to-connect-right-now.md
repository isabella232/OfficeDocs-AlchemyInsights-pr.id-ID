---
title: Masalah Aktivasi - Kami tidak dapat menyambungkan sekarang
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744598"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Memperbaiki pesan Microsoft 365 "Kami tidak dapat menyambungkan saat ini"

Catatan: Jika Anda menggunakan versi Windows yang lebih lama (misalnya Windows 7 SP1, Windows Server 2008 R2), gunakan perbaikan mudah untuk mengaktifkan TLS 1.2 sebagai default. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Untuk informasi selengkapnya, lihat Pembaruan untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP Windows .

Jika Anda menerima pesan ini, cobalah hal berikut:

1. Periksa pengaturan firewall, perangkat lunak antivirus, dan proksi untuk mengonfirmasi bahwa firewall dan proksi tidak memblokir akses Internet Microsoft 365 anda. Lihat [URL dan rentang alamat IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Buka **Mulai**  >  **Jalankan**, lalu ketik **services.msc**. Pastikan semua layanan berikut ini berjalan:
    - Penyetelan Otomatis Perangkat Tersambung Jaringan
    - Layanan Daftar Jaringan
    - Kesadaran Lokasi Jaringan
    - Windows Log Kejadian

Jika salah satu layanan ini tidak berjalan, cobalah memulainya. Jika mengalami masalah saat memulai layanan, jalankan perintah berikut dengan membuka prompt perintah dengan izin yang ditingkatkan:

**sfc /scannow**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi selengkapnya, lihat ["Maaf, kami tidak bisa tersambung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan Office dari Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).