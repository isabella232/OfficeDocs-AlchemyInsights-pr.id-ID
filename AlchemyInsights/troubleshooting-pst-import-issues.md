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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972422"
---
# <a name="troubleshooting-pst-import-issues"></a>Memecahkan masalah impor PST

- Jika mengimpor di dalam klien Outlook sendiri, lihat Memperbaiki masalah [pengi impor file .pst Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Jika menggunakan Layanan Impor dan terhenti, perhatikan bahwa setiap file PST yang Diunggah ke lokasi Azure Storage tidak boleh lebih besar dari 20GB. File PST yang berukuran lebih besar dari 20GB dapat memengaruhi kinerja proses impor PST. Untuk informasi selengkapnya memecahkan masalah pekerjaan terjebak, [lihat Masalah yang memengaruhi pekerjaan impor PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Jika Anda ingin memverifikasi status pekerjaan Impor tertentu, gunakan [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Untuk detail lengkap tentang layanan impor, [lihat Gambaran umum pengi impor file PST organisasi Anda.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
