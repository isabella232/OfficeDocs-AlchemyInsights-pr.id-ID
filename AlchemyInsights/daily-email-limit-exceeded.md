---
title: Melebihi batas email harian. Alur kerja ditangguhkan.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053120"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Melebihi batas email harian. Alur kerja ditangguhkan.

Galat ini mungkin diterima dalam skenario berikut:

- Anda memiliki alur kerja di SharePoint online yang menggunakan jenis platform alur kerja SharePoint 2010 atau SharePoint 2013.
- Alur kerja dikonfigurasi untuk mengirim pesan email kustom untuk lebih dari 200 pengguna pada waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.
- Ketika Anda menjalankan alur kerja, pesan email tidak dikirim, dan Anda melihat perilaku berikut ini:
    - Untuk alur kerja menggunakan jenis platform SharePoint 2013, menjelajah ke halaman **status alur kerja** . Pada halaman status alur kerja, **status internal** diatur untuk **memulai**, dan informasi balon menampilkan **tidak dapat mengirim ke penerima**.

Untuk mengatasi masalah ini, konfigurasikan alur kerja Anda untuk mengirim pesan email tanpa melebihi [batas pengirim Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Misalnya, gunakan jeda di alur kerja, mengirim email ke grup 365 Office, grup distribusi atau grup keamanan Surat diaktifkan, atau mengirim pesan ke kurang dari 200 Penerima pada waktu.


Untuk informasi selengkapnya, lihat [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)berikut ini.

## <a name="related-topics"></a>Topik terkait
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan aliran](https://flow.microsoft.com/blog/sharepoint-and-flow/) 