---
title: Alur kerja email tidak sedang dikirim
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049376"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Alur kerja email tidak sedang dikirim untuk SharePoint daftar atau Perpustakaan

1. Email dari alur kerja tidak dikirim ke semua pengguna atau hanya pengguna tertentu, atau Anda melihat galat **pesan email tidak dapat dikirim. Pastikan e-mail memiliki penerima yang valid**.

    Periksa jika pengguna yang ada di **semua orang** izin grup (daftar informasi pengguna) untuk koleksi situs tersebut.  Contoh URL langsung: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0

    - Jika pengguna tidak ada, pastikan pengguna masuk ke halaman. 
    - Jika pengguna eksternal, pastikan bahwa undangan mereka telah diterima.
    - Jika pengguna tidak ada di grup izin, pastikan alamat email sudah benar.
    - Jika alamat email pengguna tidak ditetapkan di sini, kemudian membuat peringatan contoh untuk pengguna yang memaksa sinkronisasi akun pengguna tersebut dari profil pengguna SharePoint untuk koleksi situs ini.
 
2. Email dari alur kerja dikirim ke administrator koleksi situs tetapi tidak untuk pengguna lain dan melihat galat **http terlarang untuk <span>https:</span>/url/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Lihat [Akses ditolak ketika Anda mengirim email ke grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Selain itu, verifikasi bahwa fitur pengumpulan situs **akses terbatas pengguna izin penguncian mode** tidak aktif.


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint online?
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


