---
title: Email alur kerja tidak dikirim
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072523"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Email alur kerja tidak dikirim untuk SharePoint daftar atau pustaka baru

1. Email dari alur kerja tidak dikirim ke semua pengguna atau hanya pengguna tertentu, atau Anda melihat kesalahan Pesan email tidak dapat dikirim. Pastikan email memiliki penerima **yang valid.**

    Periksa apakah pengguna berada dalam grup **izin Semua Orang** (daftar informasi pengguna) untuk kumpulan situs tersebut.  Contoh URL langsung: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Jika pengguna tidak ada, pastikan pengguna masuk ke halaman. 
    - Jika pengguna eksternal, pastikan undangan mereka telah diterima.
    - Jika pengguna sudah ada dalam grup izin, pastikan alamat emailnya benar.
    - Jika alamat email pengguna tidak diatur di sini, maka buat sampel pemberitahuan untuk pengguna itu yang memaksa sinkronisasi akun pengguna itu dari Profil Pengguna SharePoint ke kumpulan situs ini.
 
2. Email dari alur kerja dikirim ke administrator kumpulan situs tetapi tidak ke pengguna lain dan melihat kesalahan HTTP Dilarang ke **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Lihat [Access Denied saat Anda mengirim email ke SharePoint grup](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Selain itu, verifikasi bahwa fitur kumpulan situs **mode penguncian izin pengguna** akses terbatas tidak aktif.


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint Online?
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


