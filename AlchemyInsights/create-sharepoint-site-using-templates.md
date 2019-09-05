---
title: Membuat situs di SharePoint online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755311"
---
# <a name="create-sharepoint-sites-using-templates"></a>Membuat situs SharePoint menggunakan template

Template situs SharePoint adalah definisi prebuilt yang dirancang di sekitar kebutuhan bisnis tertentu. Untuk informasi lebih lanjut, lihat [menggunakan template untuk membuat berbagai jenis situs SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Berikut adalah beberapa masalah/solusi umum mengenai menyimpan situs atau daftar sebagai template di SharePoint online. 

**Simpan situs/daftar template tombol tidak tersedia atau hilang**

Administrator akan perlu Izinkan skrip kustom untuk mengaktifkan fitur template. Untuk langkah rinci, contoh dan pertimbangan Lihat 

- [Membolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Simpan situs sebagai template perintah tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan infrastruktur penerbitan SharePoint Server.

**Template situs tidak dapat dibuat atau tidak berfungsi dengan benar**

Template mungkin hilang [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak akan mengaktifkan. Jika fitur ini tidak tersedia untuk mengaktifkan dalam koleksi situs saat ini, Anda tidak dapat menggunakan template situs untuk membuat situs.

- Periksa untuk melihat apakah ada daftar atau Perpustakaan melebihi [ambang batas tampilan daftar](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 item karena hal ini dapat memblokir pembuatan template situs.

- Situs mungkin menggunakan terlalu banyak sumber daya dan oleh karena itu situs template melebihi batas MB 50.


- Ada masalah menampilkan data dari daftar yang menggunakan kolom pencarian. Untuk informasi selengkapnya, lihat [Daftar dihasilkan template tidak menampilkan data dari daftar pencarian yang benar di SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Untuk informasi lebih rinci tentang masalah umum dan solusi, silakan periksa [membuat dan menggunakan situs template](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



