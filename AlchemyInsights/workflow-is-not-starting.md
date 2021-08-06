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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907741"
---
# <a name="workflow-is-not-starting"></a>Alur kerja tidak dimulai

- SharePoint 2010 SharePoint 2013 tidak dimulai.

    - Jika alur kerja Anda tidak dimulai, mungkin terdapat masalah layanan sementara ketika pengguna mungkin mengalami penundaan sebentar-sebentar dengan kemajuan alur kerja. Periksa Dasbor [Kesehatan Layanan untuk](https://admin.microsoft.com/AdminPortal/Home/servicehealth) melihat apakah organisasi Anda terkena dampak.

    - Jika sudah lebih dari 24 jam sejak masalah ini muncul pertama kali, silakan log tiket dukungan. Dalam banyak kasus, kami sudah mencari solusinya. Harap beri kami setidaknya 24 jam untuk menyelesaikan solusi.

- SharePoint kerja 2010 tertunda saat dimulai.

    - Hal ini terjadi jika alur kerja dipicu dalam kumpulan yang besar. (misalnya, ketika beberapa item ditambahkan sekaligus).

    - Alur kerja tidak dirancang untuk berjalan secara real-time, jadi penundaan adalah perilaku berdasarkan desain.

   -  Jika Alur Kerja kompleks Extensible Object Markup Language (X HTML), kompilasi bisa lambat. Periksa [artikel](https://support.microsoft.com//kb/3043697) ini.

    - Anda harus menyederhanakan alur kerja atau mendesain ulang alur kerja menggunakan tipe platform Alur Kerja Microsoft SharePoint 2013.

    - Jika riwayat alur kerja Anda bertambah besar, Anda mungkin ingin membersihkan item atau membuat daftar riwayat baru.

        Informasi Selengkapnya : [Membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint Online?
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
