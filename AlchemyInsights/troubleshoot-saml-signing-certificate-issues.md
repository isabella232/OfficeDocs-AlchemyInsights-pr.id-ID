---
title: Memecahkan masalah sertifikat penandatanganan SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693424"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Memecahkan masalah sertifikat penandatanganan SAML

Untuk mengatasi masalah sertifikat penandatanganan SAML, lakukan langkah-langkah berikut ini:

1. Saat Anda menambahkan aplikasi Enterprise yang mendukung SSO, Azure akan menghasilkan sertifikat yang disebut [sertifikat penandatanganan SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Sertifikat ini memiliki tanggal kedaluwarsa 3 tahun. Untuk mengubah tanggal kedaluwarsa sertifikat Anda, lihat [Mengustomisasi tanggal kedaluwarsa sertifikat Federasi Anda dan memindahkannya ke sertifikat baru](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure akan menggunakan sertifikat ini untuk menandatangani token SAML yang diminta oleh aplikasi dan mengirimkannya ke aplikasi untuk SSO yang berhasil. Agar ini selesai, Unduh sertifikat dari Azure portal dan kirimkan ke vendor aplikasi untuk menyelesaikan proses SSO.

Setelah proses ini selesai, aplikasi Anda akan mempercayai sertifikat ini dan semua token SAML yang ditandatangani oleh sertifikat ini akan diterima oleh aplikasi.

3. Jika sertifikat ini kedaluwarsa, buat sertifikat baru, perbarui ke vendor aplikasi, lalu lakukan yang aktif di sisi Azure. Untuk informasi selengkapnya, lihat [memperpanjang sertifikat yang akan segera kedaluwarsa](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Jika sertifikat kedaluwarsa, pengguna tidak akan diblokir.

4. [Tambahkan alamat email untuk pemberitahuan](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) yang akan diterima sebelum sertifikat saat ini kedaluwarsa.

> [!NOTE]
> Langkah-4 adalah yang opsional.

5. Mengubah opsi penandatanganan sertifikat SAML aplikasi dan algoritme penandatanganan sertifikat. Untuk informasi selengkapnya, lihat [mengubah opsi penandatanganan sertifikat dan algoritma penandatanganan](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

