---
title: Masalah kinerja yang SharePoint atau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093739"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint atau OneDrive Lambat, Tidak Dapat diakses atau Tidak Tersedia untuk Beberapa Pengguna

Jika situs OneDrive atau SharePoint tersedia bagi beberapa pengguna yang sebelumnya memiliki akses, mungkin terdapat masalah layanan sementara. [Periksa dasbor kesehatan layanan](https://portal.office.com/adminportal/home#/servicehealth).

**Menambahkan dan memberikan lisensi kepada pengguna**

Pastikan bahwa Anda [Menetapkan lisensi kepada pengguna di Microsoft 365 untuk bisnis](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tetapkan Izin**

Jika pengguna telah diberi lisensi Sharepoint dan masih menerima pesan yang menolak akses, pastikan mereka memiliki tingkat [izin yang](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tepat ditetapkan.

**Pertimbangkan untuk menggunakan fitur permintaan akses**

Fitur [permintaan akses memungkinkan](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) orang untuk meminta akses ke konten yang saat ini mereka tidak mempunyai izin untuk melihatnya.

**Perbolehkan skrip kustom dapat menyebabkan masalah akses yang ditolak**

There are certain scenarios where the *Allow custom script* feature may be presenting an access denied. Untuk daftar fitur yang terpengaruh, pertimbangan keamanan dan kemampuan untuk menonaktifkan fitur. Silakan kunjungi [Perbolehkan atau cegah skrip kustom.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

