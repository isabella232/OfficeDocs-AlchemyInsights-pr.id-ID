---
title: Laporan dalam pusat admin Microsoft 365 tidak memperlihatkan nama pengguna yang dapat dibaca
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316190"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Laporan dalam pusat admin Microsoft 365 tidak memperlihatkan nama pengguna yang dapat dibaca

Laporan di pusat admin Microsoft 365 tidak memperlihatkan nama pengguna tetapi memperlihatkan nilai numerik alfa seperti B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ini adalah perilaku yang diharapkan dan telah dikomunikasikan di Pusat Pesan (MC275344, yang diterbitkan 3 Agustus 2021). 

Administrator global dapat mengembalikan perubahan ini untuk penyewa mereka dan memperlihatkan informasi pengguna yang dapat diidentifikasi jika praktik privasi organisasi mereka memperbolehkan. Untuk mengembalikan perubahan bagi penyewa:

1. Di pusat admin, masuk ke **Pengaturan**  >  **Layanan pengaturan**  >  [**Organisasi**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services), lalu pilih **Laporan.** 
1. Di **bawah Pilih cara menampilkan informasi pengguna**, pilih **Perlihatkan informasi pengguna yang dapat diidentifikasi** dalam laporan , lalu jalankan ulang laporan.