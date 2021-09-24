---
title: Menambahkan sub domain
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506485"
---
# <a name="adding-a-sub-domain"></a>Menambahkan sub domain

Sub domain bisa ditambahkan ke penyewa yang sama atau berbeda dari domain induk. Dalam kedua kasus tersebut, Anda harus mengelola pengaturan DNS sendiri di situs web pendaftar. Jika Anda telah mengizinkan Microsoft mengelola pengaturan DNS dengan catatan NS, atau jika Anda membeli domain dari Microsoft, Anda tidak dapat menambahkan subdomain tanpa mengubah ini terlebih dahulu.

Tambahkan domain induk terlebih dahulu lalu tambahkan sub domain. Jika subdomain berada dalam penyewa yang sama, verifikasi tambahan tidak diperlukan. Jika menambahkan sub domain ke penyewa terpisah, catatan TXT DNS diperlukan untuk verifikasi kepemilikan sebelum menambahkan domain dan catatan DNS tambahan untuk layanan yang dipilih.

- Untuk menambahkan domain atau subdomain, ikuti [panduan Tambahkan Domain](https://admin.microsoft.com/Adminportal#/Domains/Wizard), atau tambahkan domain atau subdomain secara manual dengan masuk ke Pengaturan   >  **Menambahkan**  >  **Domain Domain.**

Jika perlu:

- Untuk mengubah siapa yang mengelola pengaturan DNS Anda untuk domain yang sudah ada, masuk ke **Pengaturan** Domain , pilih kotak centang di samping domain, lalu  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)pilih **Kelola DNS**. Dalam panduan, pilih **Tambahkan catatan DNS Anda sendiri** dan selesaikan panduan.
- Untuk menambahkan sub domain ke domain yang dibeli Microsoft, terlebih dahulu transfer domain ke pendaftar lain, lalu buat perubahan di atas untuk mengelola catatan DNS Anda sendiri. Untuk instruksinya, [lihat Mentransfer domain dari Microsoft ke host lain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Jika Anda menerima pesan kesalahan bahwa domain Anda sudah digunakan oleh anggota atau orang lain di organisasi Anda, pertama-mata Anda harus mengambil alih akun tidak tertata ini sebelum menggunakan domain. Untuk instruksinya, [lihat Mengambil alih direktori tidak tertahan sebagai administrator di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
