---
title: Pemberitahuan di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097201"
---
# <a name="notifications-in-yammer"></a>Pemberitahuan di Yammer

Untuk memberi tahu Anda kegiatan baru dalam percakapan yang relevan, [Yammer mengirimkan pemberitahuan](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) melalui email atau, jika Anda menggunakan Yammer di perangkat seluler, melalui pemberitahuan push. Secara default, Yammer mengirimkan pemberitahuan untuk berbagai jenis kegiatan di jaringan Anda. Pengaturan email dapat diperbarui pengguna melalui situs web Yammer, sementara pemberitahuan push dikonfigurasi melalui aplikasi seluler. 

Yammer telah menambahkan dukungan untuk [email interaktif di Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Beberapa email (salinan pesan) akan menjadi interaktif dalam Outlook di web. Pada pembaruan mendatang, fitur ini akan dibawa ke versi Outlook lain.

**Tipe pemberitahuan di Yammer**

- Email (Pembaruan dari grup, seseorang mengundang Anda ke grup, Anda menerima pesan di kotak masuk, dll.)
- Pemberitahuan push (Dikirimkan ke perangkat seluler saat Anda disebutkan, menerima pesan di kotak masuk, dll.)
- Popup desktop (Jika Anda menginstal aplikasi Yammer Desktop, aplikasi akan menampilkan pemberitahuan kepada pengguna, yang disebut pemberitahuan “toast”.)
- Pemberitahuan bel (Di dalam situs web Yammer, pengguna akan melihat pemberitahuan untuk berbagai kejadian. Pemberitahuan ini mungkin tidak selalu memiliki email atau pemberitahuan push terkait.)

[Informasi lebih mendetail tentang pemberitahuan](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) tersedia.

**Mengelola pemberitahuan**

Pengguna harus mengelola pemberitahuannya sendiri. Informasi tentang [Cara mengaktifkan dan menonaktifkan email dan pemberitahuan seluler Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) tersedia. 

Administrator tidak mungkin menonaktifkan semua pemberitahuan, atau mengontrol pemberitahuan, atas nama pengguna. Admin dapat [mengontrol logo yang disertakan dalam email dan perlu tidaknya pengguna mengonfirmasi pesan](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) yang diposting melalui email.

**Pemberitahuan email dikirim ke banyak pengguna di organisasi Anda**

Kadang-kadang, satu email pemberitahuan akan dikirim oleh Yammer dan diterima oleh lebih banyak pengguna di organisasi daripada yang diperkirakan. Hal ini terjadi ketika daftar distribusi, atau tipe alamat email nonindividu lain, ditambahkan ke Yammer. Yammer tidak selalu mengetahui apakah alamat email milik satu pengguna atau alamat email yang akan menyebabkan satu email dikirimkan ke banyak penerima. Saat masalah ini terjadi, Anda harus mengambil tindakan untuk [menyuspensi (menonaktifkan) pengguna tidak valid dengan alamat email tersebut](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) di Yammer. 

Untuk mengurangi kemungkinan terjadinya masalah ini, Anda sebaiknya:

1. [Memberlakukan identitas Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) untuk Yammer.
2. Memblokir pengirim eksternal untuk mengirim email ke organisasi Anda atau membatasi pengirim berdasarkan daftar yang disetujui.

Jika masalah ini terjadi:

1. Identifikasi penerima email, yang harus sesuai dengan pengguna di Yammer. Misalnya, all-in-sales@fabrikam.com adalah daftar distribusi untuk semua orang penjualan. Daftar distribusi ini akan dapat diidentifikasi dari email Yammer yang diterima pengguna.
2. Gunakan [fitur menonaktifkan (suspensi) di Admin Jaringan](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) untuk menyuspensi pengguna yang memiliki alamat email all-in-sales@fabrikam.com. Suspensi dapat dibatalkan, jadi lebih aman daripada penghapusan. Penghapusan pengguna akan terjadi secara otomatis setelah 90 hari.
3. Jika diperlukan, tinjau [Ekspor Pengguna](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) untuk mengidentifikasi alamat email nonpengguna lain yang harus disuspensi.
