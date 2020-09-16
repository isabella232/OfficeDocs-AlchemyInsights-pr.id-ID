---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771247"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses, atau tidak tersedia untuk beberapa pengguna

Jika OneDrive atau situs SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki Access, mungkin ada masalah layanan sementara. [Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).

**Menambahkan dan melisensikan pengguna**

Pastikan Anda [menetapkan lisensi kepada pengguna di Microsoft 365 for Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tetapkan izin**

Jika pengguna telah diberi lisensi SharePoint dan masih menerima pesan Akses ditolak, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/sharepoint/understanding-permission-levels) yang ditetapkan.

**Pertimbangkan menggunakan fitur permintaan Access**

[Fitur permintaan Access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang saat ini tidak memiliki izin untuk dilihat.

**Memperbolehkan skrip kustom mungkin menyebabkan masalah Akses ditolak**

Ada beberapa skenario di mana fitur *Izinkan skrip kustom* mungkin menyajikan Akses ditolak. Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur. Silakan kunjungi [Izinkan atau Cegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

