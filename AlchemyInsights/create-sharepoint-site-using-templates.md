---
title: Membuat situs di SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057969"
---
# <a name="create-sharepoint-sites-using-templates"></a>Membuat SharePoint situs menggunakan templat

Kemampuan untuk menyimpan situs sebagai templat tidak didukung pada Situs Tim atau Komunikasi modern. Untuk informasi selengkapnya tentang cara menggunakan templat, lihat [Menyimpan, mengunduh, dan mengunggah situs SharePoint sebagai templat](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Berikut adalah beberapa masalah/solusi umum terkait Menyimpan Situs atau Daftar sebagai templat di Sharepoint Online. 

**Tombol Simpan templat situs/daftar tidak tersedia atau hilang**

Administrator perlu Mengizinkan Skrip Kustom untuk mengaktifkan fitur templat. Untuk langkah detail, contoh dan pertimbangan lihat 

- [Mengizinkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Perintah Simpan situs sebagai templat tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan Infrastruktur Penerbitan Server SharePoint.

**Templat situs tidak bisa dibuat atau tidak berfungsi dengan benar**

Templat tersebut mungkin tidak memiliki [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak dapat diaktifkan. Jika fitur tidak tersedia untuk diaktifkan di kumpulan situs saat ini, Anda tidak dapat menggunakan templat situs untuk membuat situs.

- Periksa apakah ada daftar atau pustaka yang melampaui [Ambang Batas Tampilan Daftar](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) sebesar 5000 item karena ini dapat memblokir pembuatan templat situs.

- Situs ini mungkin menggunakan sumber daya terlalu banyak sehingga templat situs melampaui batas 50 MB.


- Ada masalah ketika menampilkan data dari daftar yang menggunakan kolom pencarian. Untuk informasi selengkapnya, lihat [Daftar yang dihasilkan templat tidak menampilkan data dari daftar pencarian yang benar di SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Untuk informasi yang lebih mendetail tentang masalah dan solusi umum, silakan centang [Buat dan gunakan templat situs.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



