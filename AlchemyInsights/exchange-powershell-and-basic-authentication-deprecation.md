---
title: Menukar PowerShell dan menghentikan autentikasi dasar
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069247"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Menukar PowerShell dan menghentikan autentikasi dasar

Untuk informasi terbaru tentang cara menghubungkan Exchange Online PowerShell tanpa menggunakan Autentikasi Dasar, [klik di sini](https://aka.ms/exops-docs). Modul PowerShell V2 tidak menggunakan autentikasi dasar.

Harap diperhatikan bahwa Autentikasi Dasar masih perlu diaktifkan pada komputer klien.
Modul PowerShell V2 baru menggunakan Autentikasi Modern untuk membuat koneksi guna memungkinkan semua Cmdlet V2 berbasis REST. Selain cmdlet V2, modul ini juga memungkinkan akses ke Cmdlet PowerShell Jarak Jauh (RPS) versi lebih lama yang perlu membuat sesi PowerShell Jarak Jauh. Membuat sesi RPS pada komputer Windows memerlukan Autentikasi Dasar WinRM yang diaktifkan di komputer klien meskipun modul menggunakan mekanisme Autentikasi Modern untuk mengautentikasi ke layanan. Alur Autentikasi Dasar WinRM digunakan untuk mengangkut token Autentikasi Modern. Jika Autentikasi Dasar WinRM dinonaktifkan di komputer klien, cmdlet V2 baru akan terus berfungsi (tetapi cmdlet RPS yang lebih lama tidak akan berfungsi).
