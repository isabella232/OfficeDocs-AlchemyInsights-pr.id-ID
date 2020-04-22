---
title: Alur kerja tidak dimulai
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766100"
---
# <a name="workflow-is-not-starting"></a>Alur kerja tidak dimulai

- SharePoint 2010 dan SharePoint 2013 alur kerja tidak dimulai.

    - Jika alur kerja Anda tidak dimulai, mungkin ada masalah layanan sementara di mana pengguna mungkin mengalami penundaan terputus-putus dengan kemajuan alur kerja. Periksa [dasbor Kesehatan Layanan](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.

    - Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket dukungan. Dalam banyak kasus, kami telah bekerja pada solusi. Tolong beri kami setidaknya 24 jam untuk menyelesaikan solusi.

- SharePoint 2010 alur kerja tertunda pada mulai.

    - Hal ini terjadi jika alur kerja dipicu dalam batch besar. (misalnya, ketika beberapa item ditambahkan sekaligus).

    - Alur kerja tidak dirancang untuk berjalan secara real-time, sehingga penundaan adalah perilaku dengan desain.

   -  Jika alur kerja kompleks extensible objek Markup Language (XMOL), kompilasi dapat lambat. Periksa artikel [ini](https://support.microsoft.com//kb/3043697) .

    - Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan jenis platform Microsoft SharePoint 2013 alur kerja.

    - Jika Riwayat alur kerja Anda tumbuh besar, Anda mungkin ingin membersihkan item atau membuat daftar Riwayat baru.

        Informasi lebih lanjut: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint online?
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


