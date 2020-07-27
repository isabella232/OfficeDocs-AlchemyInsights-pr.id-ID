---
title: Beberapa pengguna mendapatkan galat Akses ditolak saat menambahkan Add-in di Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423716"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Beberapa pengguna mendapatkan galat Akses ditolak saat menambahkan Add-in di Outlook

Anda dapat menentukan administrator di organisasi yang memiliki izin untuk menginstal dan mengelola add-in untuk Outlook. Anda juga dapat menentukan pengguna mana di organisasi Anda yang memiliki izin untuk menginstal dan mengelola add-in untuk penggunaannya sendiri.

Untuk detailnya, lihat [menentukan administrator dan pengguna yang dapat menginstal dan mengelola add-in untuk Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Untuk memverifikasi bahwa Anda telah berhasil menetapkan izin untuk pengguna, ganti <Role Name> dengan nama peran untuk memverifikasi, dan jalankan perintah berikut ini di Exchange Online PowerShell:

Get-ManagementRoleAssignment-peran " <Role Name> "-geteffectiveusers

Contoh ini menunjukkan cara memverifikasi siapa yang telah Anda tetapkan izin untuk menginstal Add-in dari Office Store untuk organisasi.

Powershell

-Peran "org Marketplace Apps"-GetEffectiveUsers

Dalam hasil, Get-ManagementRoleAssignment, Tinjau entri di kolom pengguna efektif.

Untuk informasi sintaks dan parameter terperinci, lihat [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 