---
title: Alur kerja email tidak sedang dikirim
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748992"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Alur kerja email tidak sedang dikirim untuk daftar atau pustaka SharePoint

1. Email dari alur kerja tidak dikirim ke semua pengguna atau pengguna tertentu saja, atau Anda melihat kesalahan **pesan email tidak dapat dikirim. pastikan email memiliki penerima yang valid**.

    Periksa apakah pengguna ada di grup izin **semua orang** (daftar informasi pengguna) untuk kumpulan situs tersebut.  URL langsung sampel: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Jika pengguna tidak ada, pastikan pengguna masuk ke halaman. 
    - Jika merupakan pengguna eksternal, pastikan bahwa undangan mereka telah diterima.
    - Jika pengguna tidak ada di grup izin, pastikan alamat email sudah benar.
    - Jika alamat email pengguna tidak diatur di sini, maka buat pemberitahuan sampel untuk pengguna tersebut yang memaksa sinkronisasi akun pengguna tersebut dari profil pengguna SharePoint ke kumpulan situs ini.
 
2. Email dari alur kerja dikirim ke administrator kumpulan situs tetapi tidak untuk pengguna lain dan melihat kesalahan yang **dilarang <span>https:</span>//\Url/_vti_bin/client.xvc.SP.Utilities.Utility.sendemail**.
 

    Lihat [Akses ditolak saat Anda mengirim email ke grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Selain itu, verifikasi bahwa fitur kumpulan situs **mode penguncian izin akses terbatas pengguna** tidak aktif.


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint online?
- [Buat alur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


