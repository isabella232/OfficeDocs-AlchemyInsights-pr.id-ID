---
title: Batasan email harian telah terlampaui. Alur kerja ditangguhkan.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914654"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Batasan email harian Terlampaui. Alur kerja ditangguhkan.

Kesalahan ini mungkin diterima dalam skenario berikut:

- Anda memiliki alur kerja di SharePoint Online yang menggunakan tipe platform alur kerja SharePoint 2010 atau SharePoint 2013.
- Alur kerja dikonfigurasi untuk mengirim pesan email kustom ke lebih dari 200 pengguna dalam satu waktu, lebih dari 10.000 penerima per hari, atau lebih dari 30 pesan per menit.
- Saat Anda menjalankan alur kerja, pesan email tidak terkirim, dan Anda melihat perilaku berikut ini:
    - Untuk alur kerja menggunakan tipe platform SharePoint 2013, Anda menelusuri ke halaman **Status Alur** Kerja. Pada halaman Status Alur Kerja, **Status Internal** diatur ke **Dimulai,** dan balon informasi tidak **dapat dikirim ke penerima.**

Untuk mengatasi masalah ini, konfigurasi alur kerja Anda untuk mengirim pesan email tanpa [melebihi Exchange Online pengirim .](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Misalnya, gunakan jeda dalam alur kerja, kirim email ke grup Microsoft 365, grup distribusi atau grup keamanan email aktif, atau kirim pesan ke kurang dari 200 penerima dalam satu waktu.


Untuk informasi selengkapnya, lihat artikel [berikut ini](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Topik terkait
- [Membuat Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint dan Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 