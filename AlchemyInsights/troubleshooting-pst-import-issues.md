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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="4e789-102">Memecahkan masalah impor PST</span><span class="sxs-lookup"><span data-stu-id="4e789-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="4e789-103">Jika Anda mengimpor di klien Outlook sendiri, silakan lihat [Memperbaiki masalah mengimpor file .pst Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="4e789-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="4e789-104">Jika Anda menggunakan Layanan Impor dan mengalami kesulitan, harap diingat bahwa setiap file PST yang diunggah ke lokasi Penyimpanan Azure tidak boleh melebihi 20 GB.</span><span class="sxs-lookup"><span data-stu-id="4e789-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="4e789-105">File PST yang lebih besar dari 20 GB dapat memengaruhi kinerja proses impor PST.</span><span class="sxs-lookup"><span data-stu-id="4e789-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="4e789-106">Jika Anda ingin memverifikasi status pekerjaan impor tertentu, Anda dapat menggunakan [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="4e789-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="4e789-107">Untuk detail selengkapnya tentang layanan impor, silakan lihat [Gambaran umum tentang mengimpor file PST organisasi](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4e789-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
