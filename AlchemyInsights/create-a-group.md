---
title: Membuat grup
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816359"
---
# <a name="create-a-group"></a>Membuat grup

Topik ini menjelaskan pembuatan grup.

**Izin untuk Membuat Grup**

Pastikan Anda memiliki wewenang untuk membuat grup baru. Administrator global dapat menonaktifkan pembuatan grup di portal Azure atau Panel Akses. Anda mungkin memerlukan administrator untuk membuat grup baru untuk Anda, atau memberi Anda izin yang tepat.

**Mengelola izin pembuatan Grup**

1. Administrator global dapat mengelola izin pembuatan grup (untuk alasan terkait keamanan) atau grup Office 365 yang dibuat di portal Azure atau Panel Access, dengan memilih "Pengguna dapat membuat grup keamanan di portal Azure" atau "Pengguna dapat membuat grup Office 365 di portal Azure" di opsi Semua grup Umum  >  **(Pengaturan).**
2. Anda juga dapat membatasi pembuatan grup untuk memilih grup pengguna jika memiliki lisensi Azure Active Directory P1 Premium.

**Menonaktifkan pemberitahuan selamat datang untuk anggota grup Office 365 baru**

Pemberitahuan selamat datang yang dikirimkan kepada pengguna yang ditambahkan ke grup Office 365 bisa dinonaktifkan dengan menyetel **UnifiedGroupWelcomeMessageEnabled** ke False di Powershell. Pelajari tentang pengaturan ini di [sini](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

