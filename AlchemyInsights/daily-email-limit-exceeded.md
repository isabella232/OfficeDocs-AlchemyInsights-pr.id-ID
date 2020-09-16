---
title: Melebihi batas email harian. Alur kerja ditangguhkan.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731566"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Melebihi batas email harian. Alur kerja ditangguhkan.

Kesalahan ini mungkin diterima dalam skenario berikut ini:

- Anda memiliki alur kerja di SharePoint online yang menggunakan tipe platform alur kerja SharePoint 2010 atau SharePoint 2013.
- Alur kerja dikonfigurasikan untuk mengirim pesan email kustom kepada lebih dari 200 pengguna dalam satu waktu, lebih dari 10.000 Penerima per hari, atau lebih dari 30 pesan per menit.
- Saat Anda menjalankan alur kerja, pesan email tidak terkirim, dan Anda melihat perilaku berikut ini:
    - Untuk alur kerja menggunakan tipe platform SharePoint 2013, telusuri ke halaman **status alur kerja** . Pada halaman status alur kerja, **status internal** diatur ke **mulai**, dan balon informasi **tidak dapat dikirim ke penerima**.

Untuk mengatasi masalah ini, konfigurasikan alur kerja Anda untuk mengirim pesan email tanpa melebihi [batas pengirim Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Misalnya, gunakan jeda dalam alur kerja, kirim email ke grup Microsoft 365, grup distribusi atau grup keamanan email aktif, atau kirim pesan ke penerima kurang dari 200 dalam satu waktu.


Untuk informasi selengkapnya, lihat [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)berikut ini.

## <a name="related-topics"></a>Topik terkait
- [Buat alur](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 