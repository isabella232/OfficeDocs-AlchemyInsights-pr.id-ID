---
title: Memecahkan masalah impor PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991240"
---
# <a name="troubleshooting-pst-import-issues"></a>Memecahkan masalah impor PST

- Jika Anda mengimpor di klien Outlook sendiri, silakan lihat [Memperbaiki masalah mengimpor file .pst Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Jika Anda menggunakan Layanan Impor dan mengalami kesulitan, harap diingat bahwa setiap file PST yang diunggah ke lokasi Penyimpanan Azure tidak boleh melebihi 20 GB. File PST yang lebih besar dari 20 GB dapat memengaruhi kinerja proses impor PST.

- Jika Anda ingin memverifikasi status pekerjaan impor tertentu, Anda dapat menggunakan [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Untuk detail selengkapnya tentang layanan impor, silakan lihat [Gambaran umum tentang mengimpor file PST organisasi](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
