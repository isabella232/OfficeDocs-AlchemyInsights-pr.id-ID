---
title: Tidak dapat mengaktifkan Office
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
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327849"
---
# <a name="unable-to-activate-office"></a>Tidak dapat mengaktifkan Office

**Catatan**: Jika Anda menggunakan versi Windows yang lebih lama (Misalnya, Windows 7), pastikan bahwa TLS 1.2 diaktifkan sebagai default. Untuk informasi selengkapnya, lihat Memperbarui untuk mengaktifkan [TLS 1.1 dan TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)sebagai protokol aman default di WinHTTP Windows .

- Periksa apakah status langganan Anda sudah kedaluwarsa.
- Pastikan Anda memiliki langganan yang mengizinkan lisensi klien, seperti Office 365 Bisnis atau Bisnis Premium, dan [pastikan pengguna memiliki lisensi yang ditetapkan](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Pastikan pengguna masuk ke Office menggunakan akun yang sama dengan lisensi yang ditetapkan.
- Periksa [halaman Kondisi Layanan Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) untuk melihat apakah ada masalah umum pada layanan.
- Periksa firewall, perangkat lunak antivirus, dan pengaturan proksi Anda untuk memastikan agar akses aplikasi Microsoft 365 ke internet tidak terblokir. Lihat [Rentang URL dan alamat IP Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL dan rentang alamat IP Office 365").

**Tips** Di komputer Windows, kami dapat mendiagnosis dan otomatis memperbaiki beberapa masalah masuk Office yang umum untuk Anda. Unduh dan jalankan  **[Asisten Dukungan dan Pemulihan Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** untuk menggunakan alat otomatis kami.

Gunakan tindakan pemecahan masalah berikut:

- Buka aplikasi Office, lalu [keluar](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) dari akun pengguna yang ada. [Hapus](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) dan [tetapkan kembali](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) lisensi Office, kemudian [masuk ke Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) menggunakan akun pengguna yang terpengaruh.
- Jalankan [Pemecah Masalah Aktivasi](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Atur ulang status aktivasi Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Atur ulang status aktivasi Office")
- [Lakukan Perbaikan Online Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Untuk solusi pemecahan masalah lainnya, lihat:  

- [Produk Tanpa Lisensi dan kesalahan aktivasi di Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Kesalahan "Maaf, kami tidak dapat terhubung ke akun Anda. Coba lagi nanti" saat Anda mengaktifkan Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)