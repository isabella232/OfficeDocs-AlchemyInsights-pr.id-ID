---
title: Memperbaiki masalah umum dengan Pertahanan Microsoft untuk Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898247"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Memperbaiki masalah umum dengan Pertahanan Microsoft untuk Office 365

Berikut adalah beberapa solusi untuk masalah umum yang bermasalah dengan Pertahanan Microsoft Office 365:

- **Penundaan pesan:**

  Penundaan dalam pengiriman email mungkin disebabkan oleh Brankas Pemindaian pesan Lampiran. Untuk informasi selengkapnya, [lihat Brankas Pengaturan kebijakan Lampiran](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Melaporkan hasil positif atau negatif salah:**

  Untuk informasi selengkapnya, lihat [Melaporkan pesan dan file ke Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Aktifkan Brankas Link Baru**:

  1. Pada portal Pertahanan Microsoft 365 di <https://security.microsoft.com/> , buka Email & Kebijakan **Kolaborasi** \> **& Aturan** \> **Brankas** \> **tautan di** **bagian** Kebijakan.

     Untuk langsung masuk ke Brankas **Tautan,** gunakan <https://security.microsoft.com/safelinksv2> .

  2. Di **Brankas Link** Baru, pilih kebijakan dengan mengklik nama kebijakan.
  3. Di flyout detail yang muncul, lakukan salah satu langkah berikut ini:
     - Untuk menambahkan kebijakan baru, pilih **+ Buat**. Panduan akan diluncurkan untuk membantu Anda menetapkan pengaturan kebijakan.
     - Untuk mengedit kebijakan yang sudah ada, pilih kebijakan dengan mengklik nama kebijakan tersebut. Dalam flyout detail yang muncul, pilih **Edit** di bagian **Pengaturan proteksi.**
  4. Pada halaman **pengaturan Proteksi,** konfigurasi pengaturan berikut ini:
     - Aktifkan **Pilih tindakan untuk URL yang berpotensi berbahaya dan tidak diketahui dalam pesan**.
     - Pilih **Terapkan link aman untuk pesan yang dikirim dalam organisasi**.

  Untuk informasi selengkapnya, [lihat Menyiapkan Brankas Tautan di Pertahanan Microsoft untuk Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
