---
title: Penerapan batas penerimaan kotak surat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316043"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Penerapan batas penerimaan kotak surat

Microsoft baru-baru ini mulai memberlakukan ambang batas per kotak surat sebesar 3600 pesan per jam. Untuk informasi selengkapnya, [lihat Exchange Online batasan](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits). Microsoft 365 kotak surat yang menerima lebih dari 3600 pesan dalam satu jam akan dikenai batas untuk 60 menit ke depan. 

Selain itu, pasangan penerima pengirim (SRP) yang memblokir pesan yang diterima oleh kotak surat Microsoft 365 dari pengirim tertentu akan diterapkan. Jika pengirim tunggal mengirim lebih dari 33% dari total ambang batas atau 1200 pesan per rolling hour ke penerima tertentu, batas SRP akan digunakan, dan kotak surat tidak lagi menerima pesan dari pengirim tersebut. Perhatikan bahwa:

- Batas ini adalah aplikasi untuk email yang diterima dari penyewa lain, di tempat, atau pengirim Internet.
- Pengiriman email ke kotak surat diblokir untuk 60 menit ke depan. 
- Pengirim ke kotak surat ini menerima laporan tidak dikirim (5.2.121 atau 5.2.122) yang menyatakan bahwa kotak surat telah melampaui ambang batas pengiriman maksimum. Intra-penyewa (email dalam penyewa yang sama) terus dikirimkan.
- Saat batas SRP diterapkan, kotak surat penerima akan terus menerima pesan dari pengirim lain.

Administrator dapat memantau aktivitas kotak surat saat ini dengan mengakses laporan dan wawasan baru di pusat admin Exchange bernama "Kotak surat yang melebihi batas penerimaan." Wawasan hanya muncul jika penyewa telah menyinggung kotak surat, sementara laporan selalu muncul di dasbor tapi kosong kecuali penyewa telah menyinggung kotak surat.

Untuk informasi selengkapnya tentang batas penerimaan wawasan, lihat [Kotak Surat yang melebihi wawasan batas penerimaan di EAC baru.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Untuk informasi selengkapnya tentang laporan melebihi batas penerimaan, lihat [Kotak Surat yang melebihi batas penerimaan laporan di EAC baru.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)