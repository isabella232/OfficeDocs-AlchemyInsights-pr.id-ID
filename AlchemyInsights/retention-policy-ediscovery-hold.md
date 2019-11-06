---
title: 2609-retensi-atau-eDiscovery-tahan
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994072"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis

Anda atau pengguna Anda mungkin tidak dapat menghapus item di SharePoint online atau OneDrive untuk bisnis karena kebijakan retensi, retensi label atau penahanan eDiscovery diterapkan ke situs SharePoint OneDrive atau item tertentu. Ini termasuk tidak dapat menghapus dokumen, versi dokumen, folder, pustaka dokumen, daftar, aplikasi, situs, atau koleksi situs. Berikut adalah beberapa contoh dari pesan galat yang mungkin Anda terima jika Anda mencoba untuk menghapus item yang dipertahankan:

- "Situs ini tidak dapat dihapus karena disertakan dalam kebijakan penyimpanan atau penahanan eDiscovery"
- "Situs ini memiliki kebijakan kepatuhan yang ditetapkan untuk memblokir penghapusan"
- "Kebijakan kepatuhan saat ini memblokir penghapusan situs ini"
- "Koleksi situs ini tidak dihapus karena berisi situs yang disertakan dalam kebijakan penyimpanan atau penahanan eDiscovery"
- "Anda harus menghapus semua item dalam folder ini sebelum Anda menghapus folder"
- "Versi item ini tidak dapat dihapus karena kebijakan ditahan atau retensi"
- "Item tidak dapat dihapus saat ditahan"
- "Label yang diterapkan untuk item ini mencegah dari sedang diedit atau dihapus"
- "Daftar tidak dihapus saat ditahan atau kebijakan retensi"
- "Daftar tidak dapat dihapus jika diblokir atau kebijakan retensi diterapkan untuk itu"

Untuk menghapus item dalam salah satu dari skenario ini, kebijakan retensi, label retensi, atau penahanan eDiscovery harus dihapus (atau situs harus dikecualikan dari kebijakan penyimpanan). Anda perlu menonaktifkan atau mengecualikan masing-masing memegang yang menyebabkan masalah ini. Setelah kebijakan retensi atau tahan dihapus, mungkin diperlukan waktu hingga 24 jam agar perubahan diterapkan. 

Untuk informasi tentang tentang fitur penyimpanan dan tahan yang berbeda yang dapat diterapkan ke situs SharePoint dan akun OneDrive, lihat salah satu topik berikut.

- [Ikhtisar kebijakan retensi](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Ikhtisar label Penyimpanan](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Mengelola pembekuan dalam eDiscovery tingkat lanjut](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery memegang](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Kebijakan penutupan dan penghapusan situs warisan](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
