---
title: Masalah membuka atau men-download file di heboh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148332"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Masalah membuka atau men-download file di heboh

Klasik heboh mendukung beberapa pilihan untuk file upload ke pesan dan kelompok. Tergantung pada konfigurasi jaringan, file default ke penyimpanan di SharePoint.

Pemilih file di heboh baru belum mendukung semua pilihan yang tersedia dalam klasik heboh. Pembaruan berikutnya akan menambahkan fitur tambahan. Untuk informasi lebih lanjut, lihat [melampirkan file atau gambar ke posting percakapan heboh](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Tidak dapat membuka atau mengunduh berkas**  

Berkas yang mungkin meng-upload ke Yammer tetapi juga dapat menghubungkan ke berkas di SharePoint online. Untuk memecahkan masalah, pertama-tama Anda harus menentukan lokasi berkas. Jika file telah diunggah ke heboh, itu akan memiliki URL *. yammer.com. Pastikan URL dan alamat IP yang diperlukan tidak diblokir. Untuk informasi lebih lanjut, lihat posting blog [menggunakan alamat IP keras kode untuk heboh tidak dianjurkan](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Periksa apakah pengguna yang juga admin global dapat men-download file. Jika file bersifat pribadi, Anda mungkin harus menggunakan mode konten pribadi. Untuk informasi lebih lanjut, lihat kemudian [memantau konten pribadi di heboh](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Heboh tingkat jaringan tamu dan file dalam SharePoint online**  

[Tingkat jaringan tamu di heboh](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) tidak menggunakan AZURE AD B2B dan internal untuk layanan heboh, sehingga mereka tidak dapat mengakses file heboh disimpan di SharePoint. Membuat eksternal AAD B2B pengguna yang dapat mengakses perpustakaan dokumen di SharePoint online dengan menggunakan identitas tersebut. Untuk informasi tentang masa depan Azure AD B2B dukungan tamu di Yammer, lihat [dukungan tamu Business-to-Business (B2B) di Yammer pratinjau-persyaratan pelanggan dan FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).