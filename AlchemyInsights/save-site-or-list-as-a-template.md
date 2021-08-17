---
title: Menyimpan situs atau daftar sebagai templat
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109207"
---
# <a name="save-site-or-list-as-a-template"></a>Menyimpan situs atau daftar sebagai templat

SharePoint templat situs adalah definisi bawaan yang dirancang untuk kebutuhan bisnis tertentu. Untuk informasi selengkapnya, lihat [Menggunakan templat untuk membuat jenis situs SharePoint berbeda.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Berikut ini beberapa masalah/solusi umum terkait Menyimpan Situs atau Daftar sebagai templat di SharePoint Online.

**Tombol Simpan templat situs/daftar tidak tersedia atau hilang.** 

- Administrator perlu Mengizinkan Skrip Kustom untuk mengaktifkan fitur templat. Untuk langkah detail, contoh dan pertimbangan, lihat [Perbolehkan atau mencegah skrip kustom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Perintah Simpan situs sebagai templat tidak didukung dan dapat menyebabkan masalah pada situs yang menggunakan Infrastruktur Penerbitan Server SharePoint.


**Templat situs tidak bisa dibuat atau tidak berfungsi dengan benar**

- Templat tersebut mungkin tidak memiliki [fitur](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) dan tidak dapat diaktifkan. Jika fitur tidak tersedia untuk diaktifkan di kumpulan situs saat ini, Anda tidak dapat menggunakan templat situs untuk membuat situs.


- Periksa apakah ada daftar atau pustaka yang melampaui [Ambang Batas Tampilan Daftar](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) sebesar 5000 item karena ini dapat memblokir pembuatan templat situs.


- Situs tersebut mungkin menggunakan terlalu banyak sumber daya dan karenanya templat situs melebihi batas 50 megabyte (MB).


- Ada masalah ketika menampilkan data dari daftar yang menggunakan kolom pencarian. Untuk informasi selengkapnya, [lihat Daftar yang dihasilkan templat tidak menampilkan data dari daftar pencarian yang benar dalam SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Untuk informasi lebih detail tentang masalah dan solusi umum, silakan lihat referensi, [Membuat dan menggunakan templat situs.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

