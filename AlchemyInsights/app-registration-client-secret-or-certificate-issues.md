---
title: Masalah rahasia klien pendaftaran aplikasi atau Sertifikat
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951496"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Masalah rahasia klien pendaftaran aplikasi atau Sertifikat

Rahasia klien aplikasi kedaluwarsa?

Terlepas dari bagaimana aplikasi terdaftar dibuat, baik melalui proses pendaftaran standar di portal Registrasi Aplikasi atau jika Prinsipal Layanan dibuat di penyewa Anda dengan menggunakan persetujuan aplikasi, Rahasia Klien baru harus dibuat sebelum kedaluwarsanya Aplikasi saat ini dan diperbarui dalam kode aplikasi yang terkait. Periode validitas maksimum adalah 2 tahun. Sebagai pengingat, nilai rahasia harus direkam karena tidak akan terlihat lagi setelah meninggalkan halaman Pendaftaran aplikasi di portal. Untuk informasi selengkapnya, [lihat Mulai cepat: Mendaftarkan aplikasi di platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) dan Praktik terbaik untuk [platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Untuk mempelajari selengkapnya, [lihat Membuat & layanan Azure AD di portal - platform identitas Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
