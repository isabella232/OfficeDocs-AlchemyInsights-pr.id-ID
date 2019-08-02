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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059607"
---
# <a name="workflow-email-is-not-being-sent"></a>Alur kerja email tidak dikirim

1. Email dari alur kerja tidak dikirim ke semua pengguna atau hanya pengguna tertentu, atau Anda melihat kesalahan **pesan e-mail tidak dapat dikirim. Pastikan e-mail memiliki Penerima berlaku**.

Periksa jika pengguna yang ada di grup izin **Semua orang** (daftar informasi pengguna) untuk koleksi situs itu.  Contoh URL langsung: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Jika pengguna tidak ada, pastikan pengguna masuk ke halaman. 
- Jika pengguna eksternal, pastikan bahwa undangan telah diterima.
- Jika pengguna ada di kelompok izin, pastikan alamat email benar.
- Jika alamat email pengguna yang tidak diatur di sini, kemudian membuat lansiran sampel untuk pengguna yang yang pasukan sync account pengguna tersebut dari profil pengguna SharePoint untuk koleksi situs ini.
 
2. Email dari alur kerja akan dikirim ke administrator koleksi situs tapi tidak untuk pengguna lain dan melihat kesalahan **HTTP terlarang untuk <spam> <spam> ** <spam> <spam>.
 

Lihat [Akses ditolak ketika email yang dikirim ke grup](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Juga, pastikan **akses terbatas pengguna izin kuncian modus** situs koleksi fitur tidak aktif.

## <a name="related-topics"></a>Topik terkait
- [Menciptakan aliran](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


