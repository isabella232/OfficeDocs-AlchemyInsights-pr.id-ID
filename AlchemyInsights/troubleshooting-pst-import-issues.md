---
title: Memecahkan masalah impor PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059818"
---
# <a name="troubleshooting-pst-import-issues"></a>Memecahkan masalah impor PST

- Jika Anda mengimpor dalam klien Outlook itu sendiri, lihat [Memperbaiki masalah pengi impor file .pst Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Jika menggunakan Layanan Impor dan terhenti, perhatikan bahwa setiap file PST yang Anda unggah ke lokasi Penyimpanan Azure tidak boleh lebih besar dari 20GB. File PST yang berukuran lebih besar dari 20GB dapat memengaruhi kinerja proses impor PST. Untuk informasi selengkapnya memecahkan masalah pekerjaan terjebak, [lihat Masalah yang memengaruhi pekerjaan impor PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Jika Anda ingin memverifikasi status pekerjaan Impor tertentu, gunakan [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Untuk detail lengkap tentang layanan impor, [lihat Gambaran umum pengi impor file PST organisasi Anda.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
