---
title: Alur kerja tidak dimulai
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
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794770"
---
# <a name="workflow-is-not-starting"></a>Alur kerja tidak dimulai

- Alur kerja SharePoint 2010 dan SharePoint 2013 tidak dimulai.

    - Jika alur kerja Anda tidak dimulai, mungkin ada masalah layanan sementara ketika pengguna mungkin mengalami penundaan dengan kemajuan alur kerja. Lihat [dasbor Kesehatan Layanan](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat apakah organisasi Anda terpengaruh.

    - Jika lebih dari 24 jam telah berlalu sejak pertama kali melihat masalah ini, silakan masuk ke tiket dukungan. Dalam banyak kasus, kami sedang mengupayakan solusi. Harap Beri kami setidaknya 24 jam untuk menyelesaikan solusi.

- Alur kerja SharePoint 2010 tertunda saat mulai.

    - Hal ini terjadi jika alur kerja dipicu dalam batch besar. (misalnya, ketika beberapa item ditambahkan sekaligus).

    - Alur kerja tidak dirancang untuk menjalankan real-time, sehingga penundaan adalah perilaku desain.

   -  Jika alur kerja kompleks extensible Object Markup Language (XMOL), kompilasi bisa menjadi lambat. Lihat artikel [ini](https://support.microsoft.com//kb/3043697) .

    - Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan tipe platform alur kerja Microsoft SharePoint 2013.

    - Jika Riwayat alur kerja Anda telah bertambah besar, Anda mungkin ingin menghapus item atau membuat daftar Riwayat baru.

        Informasi selengkapnya: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint online?
- [Buat alur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


