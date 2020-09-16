---
title: Pemberitahuan peringatan SharePoint tidak terkirim
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751246"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Pemberitahuan peringatan SharePoint tidak terkirim

Silakan periksa folder sampah dalam email, karena terkadang pemberitahuan mungkin ada di sana.

Tentukan apakah **semua pemberitahuan tidak terkirim** atau **pemberitahuan individu** dari file atau pustaka tertentu tidak terkirim.

- **Pemberitahuan individual tidak terkirim**: Jika pemberitahuan individu dari file atau pustaka tertentu tidak terkirim, Anda bisa mencoba untuk menghapus dan membuatnya kembali. Lihat [mengelola, menampilkan, atau menghapus pemberitahuan SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) untuk membuat ulang pemberitahuan.
- **Semua pemberitahuan tidak terkirim**: jika semua pemberitahuan dari beberapa file atau pustaka tidak terkirim, kunjungi [dasbor Kesehatan Layanan](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) untuk memeriksa setiap saran/insiden yang mungkin terjadi dengan SharePoint atau Exchange. Masalah ini mungkin dengan kapabilitas pemberitahuan SharePoint atau keterlambatan dalam email melalui Exchange. Akan sangat penting untuk diingat Apakah email lain sedang dikirim, dan jika tidak, masalah cenderung dengan penundaan Exchange.

Tanya jawab umum tentang pemberitahuan:

- Tidak dimungkinkan untuk mengirim pemberitahuan ke grup distribusi, hanya grup keamanan dan O365 yang didukung.
- Anda tidak dapat mengustomisasi Templat email pemberitahuan; Anda perlu menggunakan alur kerja Microsoft FLOW atau SharePoint Designer untuk mencapainya.

## <a name="related-topics"></a>Topik terkait

Ingin mencoba Microsoft Flow di SharePoint online?

- [Buat alur](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint dan Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
