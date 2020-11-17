---
title: Membuat grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088906"
---
# <a name="create-a-group"></a>Membuat grup

Topik ini menguraikan pembuatan grup.

**Izin untuk membuat grup**

Pastikan Anda memiliki wewenang untuk membuat grup baru. Administrator global dapat menonaktifkan pembuatan grup di portal Azure atau panel akses. Anda mungkin memerlukan administrator untuk membuat grup baru untuk Anda, atau untuk memberi izin yang sesuai.

**Mengelola izin pembuatan grup**

1. Administrator global dapat mengelola izin pembuatan grup (untuk alasan keamanan yang terkait) atau grup 365 Office yang dibuat di portal Azure atau panel akses, dengan memilih "pengguna dapat membuat grup keamanan di portal Azure" atau "pengguna dapat membuat grup Office 365 di portal Azure" di **semua grup**  >  **Umum (pengaturan)**.
2. Anda juga bisa membatasi pembuatan grup untuk memilih grup pengguna jika Anda memiliki lisensi Premium Azure Active Directory P1.

**Menonaktifkan pemberitahuan Selamat datang untuk anggota grup Office 365 baru**

Pemberitahuan sambutan yang dikirimkan kepada pengguna yang ditambahkan ke grup Office 365 dapat dinonaktifkan dengan mengatur **Unifiedgroupwelcomemessagediaktifkan** ke false di PowerShell. Pelajari tentang pengaturan ini [di sini](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

