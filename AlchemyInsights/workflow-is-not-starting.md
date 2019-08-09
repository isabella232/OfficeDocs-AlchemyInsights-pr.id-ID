---
title: Alur kerja tidak memulai
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270783"
---
# <a name="workflow-is-not-starting"></a>Alur kerja tidak memulai

- SharePoint 2010 dan SharePoint 2013 alur kerja tidak mulai.

    - Jika alur kerja Anda tidak memulai, mungkin ada masalah sementara layanan mana pengguna mungkin mengalami penundaan intermiten dengan kemajuan alur kerja. Periksa [Layanan kesehatan Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk melihat jika organisasi Anda dipengaruhi.

    - Jika lebih dari 24 jam telah berlalu sejak Anda pertama kali melihat masalah ini, silakan log tiket support. Dalam banyak kasus, kami sudah bekerja pada sebuah solusi. Mohon berikan setidaknya 24 jam untuk menyelesaikan solusi.

- SharePoint 2010 Workflow tertunda pada awal.

    - Hal ini terjadi jika alur kerja dipicu dalam kumpulan besar. (sebagai contoh, ketika beberapa item ditambahkan sekaligus).

    - Alur kerja tidak dirancang untuk menjalankan real-time, sehingga penundaan adalah perilaku oleh desain.

   -  Jika alur kerja adalah kompleks Extensible Object Markup Language (XMOL), kompilasi bisa lambat. Check [this](https://support.microsoft.com/en-us/kb/3043697) artikel.

    - Anda harus menyederhanakan alur kerja atau mendesain ulang menggunakan jenis platform Microsoft SharePoint 2013 alur kerja.

    - Jika Riwayat alur kerja telah tumbuh besar, Anda mungkin ingin membersihkan item atau membuat daftar sejarah baru.

        Informasi lebih lanjut: [membersihkan riwayat alur kerja](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Topik terkait
Ingin mencoba Microsoft Flow di SharePoint Online?
- [Menciptakan aliran](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


