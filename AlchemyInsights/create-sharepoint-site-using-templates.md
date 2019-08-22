---
title: Membuat situs di SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515001"
---
# <a name="create-sharepoint-sites-using-templates"></a>Buat situs SharePoint menggunakan template

Template situs SharePoint adalah prebuilt definisi yang dirancang di sekitar kebutuhan bisnis tertentu. Untuk selengkapnya, lihat [menggunakan template untuk membuat berbagai jenis situs SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Berikut adalah beberapa masalah/solusi umum mengenai menyimpan situs atau daftar sebagai template dalam Sharepoint Online. 

**Menyimpan daftar situs/template tombol ini tidak tersedia atau hilang**

Administrator akan perlu untuk membolehkan Custom Script untuk mengaktifkan fitur template. Untuk langkah-langkah rinci contoh dan pertimbangan Lihat 

- [Membolehkan atau mencegah script kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Situs Simpan sebagai perintah template tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan SharePoint Server Publishing infrastruktur.

**Situs template tidak dapat dibuat atau tidak berfungsi dengan benar**

Template mungkin hilang [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak akan diaktifkan. Jika fitur ini tidak tersedia untuk mengaktifkan dalam koleksi situs saat ini, Anda tidak dapat menggunakan situs template untuk membuat situs.

- Periksa untuk melihat jika atau daftar perpustakaan melebihi [Ambang batas daftar View](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 item seperti ini dapat menghalangi pembentukan situs template.

- Situs mungkin menggunakan terlalu banyak sumber daya dan karena itu situs template melebihi batas 50 MB.


- Ada masalah yang menampilkan data dari daftar yang menggunakan kolom pencarian. Untuk informasi lebih lanjut, lihat [Daftar Template yang dihasilkan tidak menampilkan data dari daftar SharePoint Online benar lookup](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Untuk informasi lebih rinci tentang umum masalah dan solusi, silahkan cek [membuat dan menggunakan situs template](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



