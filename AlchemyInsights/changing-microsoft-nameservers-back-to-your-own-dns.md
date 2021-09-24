---
title: Mengubah dari nameserver Microsoft kembali untuk mengelola catatan DNS Anda sendiri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506606"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Mengubah dari nameserver Microsoft kembali untuk mengelola catatan DNS Anda sendiri

Anda sebelumnya telah mengubah catatan NS agar mengarahkan ke Microsoft (ns1.bdm.microsoftonline.com) tetapi sekarang telah memutuskan untuk mengelola catatan DNS Anda sendiri:

Di situs web pendaftar domain, ubah server nama kembali ke pendaftar Anda atau pengaturan sebelumnya. Jika Anda belum terbiasa dengan DNS, hubungi dukungan di pencatat domain. Perlu diketahui bahwa perubahan nameserver dapat memakan waktu hingga 48 jam untuk dis propagate. 

1. Di portal Microsoft 365 admin, masuk **Pengaturan** Domain , pilih kotak centang di samping  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)domain, dan pilih **Kelola DNS.** 

2. Dalam panduan, pilih **Tambahkan catatan DNS Anda sendiri** dan selesaikan panduan. Ini akan mengubah cara DNS Anda dikelola, lalu memungkinkan Anda menambahkan catatan DNS kustom yang diperlukan untuk mendukung layanan pilihan Anda.

Atau, Jika Anda mengubah catatan server nama Anda ke Microsoft dan memiliki situs web, Anda bisa menambahkan catatan DNS untuk situs web, bukan mengubah server nama kembali. Untuk informasi selengkapnya, lihat [Memperbarui catatan DNS agar situs web Anda tetap menggunakan penyedia hosting Anda saat ini.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


