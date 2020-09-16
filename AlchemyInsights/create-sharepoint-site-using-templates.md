---
title: Membuat situs di SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732230"
---
# <a name="create-sharepoint-sites-using-templates"></a>Membuat situs SharePoint menggunakan templat

Kemampuan untuk menyimpan situs sebagai Templat tidak didukung dengan situs tim atau komunikasi modern. Untuk informasi selengkapnya tentang menggunakan templat [, lihat menyimpan, mengunduh, dan mengunggah situs SharePoint sebagai Templat](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Berikut adalah beberapa masalah/solusi umum terkait penyimpanan situs atau daftar sebagai Templat di SharePoint online. 

**Tombol Simpan situs/daftar Templat tidak tersedia atau tidak ada**

Administrator perlu memperbolehkan skrip kustom untuk mengaktifkan fitur Templat. Untuk detail langkah, contoh dan pertimbangan Lihat 

- [Memperbolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Perintah Simpan situs sebagai Templat tidak didukung dan bisa menyebabkan masalah pada situs yang menggunakan infrastruktur penerbitan SharePoint Server.

**Templat situs tidak bisa dibuat atau tidak berfungsi dengan benar**

Templat mungkin kehilangan [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak dapat diaktifkan. Jika fitur tidak tersedia untuk diaktifkan dalam kumpulan situs saat ini, Anda tidak bisa menggunakan templat situs untuk membuat situs.

- Periksa untuk melihat apakah ada daftar atau Pustaka yang melebihi [ambang batas batas tampilan daftar](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) item 5000 karena hal ini bisa memblokir pembuatan Templat situs.

- Situs tersebut mungkin menggunakan terlalu banyak sumber daya dan karena itu Templat situs melebihi batas 50 MB.


- Ada masalah menampilkan data dari daftar yang menggunakan kolom pencarian. Untuk informasi selengkapnya, lihat [Daftar yang dihasilkan Templat tidak menampilkan data dari daftar pencarian yang benar di SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Untuk informasi mendetail tentang masalah umum dan solusi, silakan periksa [buat dan gunakan Templat situs](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



