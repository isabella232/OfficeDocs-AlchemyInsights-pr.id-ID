---
title: Mengubah pengaturan pembatasan EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818039"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="8a027-102">Mengubah pengaturan pembatasan EWS</span><span class="sxs-lookup"><span data-stu-id="8a027-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="8a027-103">Jalankan uji otomatis kami yang akan memungkinkan Anda mengubah kebijakan pembatasan EWS selama durasi migrasi.</span><span class="sxs-lookup"><span data-stu-id="8a027-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="8a027-104">Perlu diperhatikan bahwa meskipun proses ini telah dijalankan, impor EWS masih akan dibatasi hingga 150 mb per 5 menit per kotak surat; untuk mencapai kecepatan throughput migrasi yang lebih tinggi, silakan migrasikan lebih banyak pengguna secara bersamaan.</span><span class="sxs-lookup"><span data-stu-id="8a027-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="8a027-105">Ingat bahwa perubahan kebijakan pembatasan EWS tidak berpengaruh pada jenis migrasi berikut (menggunakan alat Microsoft): Hibrid, Langsung/Bertahap (RPC/HTTP), Protokol Akses Pesan Internet, G Suite, Folder Publik, atau Layanan Impor PST.</span><span class="sxs-lookup"><span data-stu-id="8a027-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>