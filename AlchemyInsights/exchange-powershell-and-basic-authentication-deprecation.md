---
title: Menukar PowerShell dan menghentikan autentikasi dasar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015692"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Menukar PowerShell dan menghentikan autentikasi dasar

Untuk informasi terbaru tentang cara menghubungkan Exchange Online PowerShell tanpa menggunakan Autentikasi Dasar, [klik di sini](https://aka.ms/psbasicauth).

Harap diperhatikan bahwa Autentikasi Dasar masih perlu diaktifkan pada komputer klien.
Modul PowerShell V2 baru menggunakan Autentikasi Modern untuk membuat koneksi guna memungkinkan semua Cmdlet V2 berbasis REST. Selain cmdlet V2, modul ini juga memungkinkan akses ke Cmdlet PowerShell Jarak Jauh (RPS) versi lebih lama yang perlu membuat sesi PowerShell Jarak Jauh. Membuat sesi RPS pada komputer Windows memerlukan Autentikasi Dasar WinRM yang diaktifkan di komputer klien meskipun modul menggunakan mekanisme Autentikasi Modern untuk mengautentikasi ke layanan. Alur Autentikasi Dasar WinRM digunakan untuk mengangkut token Autentikasi Modern. Jika Autentikasi Dasar WinRM dinonaktifkan di komputer klien, cmdlet V2 baru akan terus berfungsi (tetapi cmdlet RPS yang lebih lama tidak akan berfungsi).
