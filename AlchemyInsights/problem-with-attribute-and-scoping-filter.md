---
title: Masalah dengan atribut dan cakupan filter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481893"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Masalah dengan atribut dan cakupan filter

**Masalah dengan nilai UPN yang berkonflik**

Hari kerja untuk penyediaan pengguna untuk Workday untuk provisioning pengguna AD memperlihatkan pesan kesalahan **Hybridsynchronizationactivedirectoryuserprincipalnamenotunique**. Operasi gagal karena nilai UPN yang disediakan untuk penambahan/modifikasi bukan merupakan Forest Unique. Detail kesalahan: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Nilai **userPrincipalName** yang akan diatur oleh konektor workday saat membuat akun pengguna AD sudah ada di domain AD target. Ini menyiratkan bahwa (1) pengguna sudah ada dan pemeriksaan ID yang cocok gagal untuk pengguna atau (2) aturan pembuatan UPN yang menghasilkan nilai berkonflik.

Berikut adalah langkah-langkah resolusi yang disarankan:

Jika pengguna sudah ada dan ID pencocokan yang sesuai gagal untuk menautkan akun Workday ke akun direktori aktif, periksa apakah atribut ID yang cocok (biasanya **idkaryawan**) dalam hari kerja dan iklan memiliki kecocokan yang sama persis. Jika mereka tidak memiliki kecocokan, itu adalah masalah data yang perlu diperbaiki. Misalnya, jika Idkaryawan dalam hari kerja adalah 001052 dan di 1052 AD, maka mesin provisioning akan gagal untuk menautkan kedua akun dan akan mencoba membuat pengguna yang sudah ada. Solusi dalam kasus ini adalah mengubah nilai **idkaryawan** di AD untuk menyertakan angka nol terdepan untuk membuatnya 001052.
Jika ekspresi yang menghasilkan UPN tidak menghasilkan nilai unik, pertimbangkan menggunakan fungsi de-duplikasi **Selectuniquevalue** untuk menghasilkan nilai unik setiap kali.

**Hari kerja untuk penyediaan pengguna AD tidak mengatur nilai atribut manajer untuk akun pengguna AD**

Hari kerja ke pekerjaan penyediaan pengguna AD tidak mengatur nilai atribut **manajer** untuk akun pengguna AD. Ada dua kemungkinan skenario saat perilaku ini terlihat:

1. Manajer di Workday tidak dapat diselesaikan ke akun pengguna AD terkait karena manajer tidak berada dalam lingkup.
2. Dalam skenario **beberapa domain AD** , manajer dalam hari kerja tidak ada di domain yang sama dengan pengguna.

Cobalah langkah-langkah ini untuk mengatasi masalah tersebut:

1. Jika Anda telah menetapkan filter lingkup, pertama-tama Periksa apakah manajer berada dalam lingkup dan itu memenuhi klausul pelingkupan. Jika Manajer tidak memenuhi cakupan pelingkupan, Ubah filter sehingga manajer juga berada dalam lingkup operasi penyediaan.
2. Jika Anda memiliki beberapa domain, maka konektor memiliki batasan yang diketahui ketidakmampuan untuk mengatasi referensi manajer domain silang.

Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













