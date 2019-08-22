---
title: Alur kerja email tidak dikirim
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530879"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Alur kerja email tidak dikirim untuk daftar SharePoint atau Perpustakaan

1. Email dari alur kerja tidak dikirim ke semua pengguna atau hanya pengguna tertentu, atau Anda melihat kesalahan **pesan e-mail tidak dapat dikirim. Pastikan e-mail memiliki Penerima berlaku**.

    Periksa jika pengguna yang ada di grup izin **Semua orang** (daftar informasi pengguna) untuk koleksi situs itu.  Contoh URL langsung: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Jika pengguna tidak ada, pastikan pengguna masuk ke halaman. 
    - Jika pengguna eksternal, pastikan bahwa undangan telah diterima.
    - Jika pengguna ada di kelompok izin, pastikan alamat email benar.
    - Jika alamat email pengguna yang tidak diatur di sini, kemudian membuat lansiran sampel untuk pengguna yang yang pasukan sync account pengguna tersebut dari profil pengguna SharePoint untuk koleksi situs ini.
 
2. Email dari alur kerja akan dikirim ke administrator koleksi situs tapi tidak untuk pengguna lain dan melihat kesalahan **HTTP terlarang untuk <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Lihat [Akses ditolak ketika Anda mengirim email ke grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Juga, pastikan **akses terbatas pengguna izin kuncian modus** situs koleksi fitur tidak aktif.


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint Online?
- [Menciptakan aliran](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


