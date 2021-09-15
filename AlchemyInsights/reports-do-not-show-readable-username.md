---
title: Laporan di pusat admin Microsoft 365 tidak menampilkan nama pengguna yang dapat dibaca
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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327817"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Laporan di pusat admin Microsoft 365 tidak menampilkan nama pengguna yang dapat dibaca

Laporan di pusat admin Microsoft 365 tidak menampilkan nama pengguna tetapi menampilkan nilai numerik alfa seperti B2BC6C15BB9FCDEA71E5CD302D228CC8.

Perilaku ini diharapkan dan telah dikomunikasikan di Pusat Pesan (MC275344, diterbitkan 3 Agustus 2021). 

Administrator global dapat mengembalikan perubahan ini untuk penyewanya dan menampilkan informasi pengguna yang dapat diidentifikasi jika peraturan privasi organisasinya memperbolehkan. Untuk mengembalikan perubahan untuk penyewa:

1. Di pusat admin, buka **Pengaturan** > **Pengaturan org** > [**Layanan**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ), dan pilih **Laporan**. 
1. Di bawah **Pilih cara menampilkan informasi pengguna**, pilih **Menampilkan informasi pengguna yang dapat diidentifikasi dalam laporan**, lalu jalankan kembali laporan.