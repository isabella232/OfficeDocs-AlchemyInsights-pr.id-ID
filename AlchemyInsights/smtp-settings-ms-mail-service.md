---
title: Pengaturan SMTP untuk Microsoft 365 email tambahan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813974"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Pengaturan SMTP untuk Microsoft 365 email tambahan

Berikut ini adalah pengaturan SMTP untuk Microsoft 365 email berikut:

**Server**: smtp.office365.com </br>
**Port**: 587 </br>
**Enkripsi**: STARTTLS (Hanya TLS 1.2 versi yang didukung sekarang. Pastikan aplikasi atau perangkat Anda mendukung TLS 1.2) </br>
**Nama** Pengguna : Office 365 Alamat Anda (misalnya alamat example@yourdomain.com) </br>
**Kata Sandi**: Kata Office 365 Sandi Anda </br>
**Autentikasi:** Diperlukan </br>
**Batas Pengiriman:** 10.000 Email sehari </br>

Untuk pengaturan POP dan IMAP, lihat [Pengaturan POP, IMAP, dan SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Untuk mempelajari tentang opsi relai email menggunakan Microsoft 365 langkah-langkahnya, lihat Cara menyiapkan perangkat atau aplikasi [multifungsi](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)untuk mengirimkan email menggunakan Microsoft 365 atau Office 365 .