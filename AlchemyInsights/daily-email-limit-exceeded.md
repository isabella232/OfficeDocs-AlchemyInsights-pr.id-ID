---
title: Batas harian email melebihi. Alur kerja ini ditangguhkan.
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
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059642"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Email harian yang melebihi batas. Alur kerja ini ditangguhkan.

Kesalahan ini dapat diterima dalam skenario berikut:

- Anda memiliki alur kerja di SharePoint Online yang menggunakan SharePoint 2010 atau jenis platform SharePoint 2013 alur kerja.
- Alur kerja dikonfigurasi untuk mengirim pesan email kustom ke lebih dari 200 pengguna pada suatu waktu, lebih dari 10.000 Penerima per hari atau lebih dari 30 pesan per menit.
- Ketika Anda menjalankan alur kerja, pesan email tidak dikirim, dan Anda melihat aktivitas berikut:
    - Untuk alur kerja menggunakan jenis platform SharePoint 2013, Anda browse ke halaman **Alur kerja Status** . Pada halaman Status alur kerja, **Internal Status** diatur untuk **memulai**, dan menampilkan informasi balon **gagal mengirim ke penerima**.

Untuk mengatasi masalah ini, konfigurasikan alur kerja Anda untuk mengirim pesan email tanpa melebihi [batas pengirim Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Misalnya, menggunakan jeda dalam alur kerja, kirim email ke Office 365 grup, grup distribusi, atau grup mail diaktifkan keamanan, atau mengirim pesan ke kurang dari 200 Penerima pada suatu waktu.


Untuk informasi lebih lanjut, lihat [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)berikut.

## <a name="related-topics"></a>Topik terkait
- [Menciptakan aliran](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 