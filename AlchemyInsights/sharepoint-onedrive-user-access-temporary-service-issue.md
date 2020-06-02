---
title: Masalah kinerja-SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511151"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive lambat, tidak dapat diakses atau tidak tersedia untuk banyak pengguna

Jika OneDrive atau situs SharePoint tidak tersedia untuk beberapa pengguna yang sebelumnya memiliki akses, mungkin ada masalah layanan sementara. [Periksa dasbor Kesehatan Layanan](https://portal.office.com/adminportal/home#/servicehealth).

**Menambahkan dan melisensikan pengguna**

Pastikan bahwa Anda [menetapkan lisensi untuk pengguna di Microsoft 365 untuk bisnis](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Menetapkan izin**

Jika pengguna telah ditetapkan lisensi SharePoint dan masih menerima pesan Akses ditolak, pastikan mereka memiliki [tingkat izin yang sesuai](https://docs.microsoft.com/sharepoint/understanding-permission-levels) yang ditetapkan.

**Pertimbangkan untuk menggunakan fitur permintaan akses**

[Fitur permintaan akses](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) memungkinkan orang untuk meminta akses ke konten yang saat ini tidak diizinkan untuk dilihat.

**Memungkinkan skrip kustom dapat menyebabkan masalah Akses ditolak**

Ada skenario tertentu mana fitur *memungkinkan kustom skrip* mungkin menyajikan Akses ditolak. Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur. Silakan kunjungi [Izinkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

