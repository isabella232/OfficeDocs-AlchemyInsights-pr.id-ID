---
title: Mengubah pengaturan pembatasan EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075900"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="c88a7-102">Mengubah pengaturan pembatasan EWS</span><span class="sxs-lookup"><span data-stu-id="c88a7-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="c88a7-103">Jalankan uji otomatis kami yang akan memungkinkan Anda mengubah kebijakan pembatasan EWS selama durasi migrasi.</span><span class="sxs-lookup"><span data-stu-id="c88a7-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="c88a7-104">Perlu diperhatikan bahwa meskipun proses ini telah dijalankan, impor EWS masih akan dibatasi hingga 150 mb per 5 menit per kotak surat; untuk mencapai kecepatan throughput migrasi yang lebih tinggi, silakan migrasikan lebih banyak pengguna secara bersamaan.</span><span class="sxs-lookup"><span data-stu-id="c88a7-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="c88a7-105">Ingat bahwa perubahan kebijakan pembatasan EWS tidak berpengaruh pada jenis migrasi berikut (menggunakan alat Microsoft): Hibrid, Langsung/Bertahap (RPC/HTTP), Protokol Akses Pesan Internet, G Suite, Folder Publik, atau Layanan Impor PST.</span><span class="sxs-lookup"><span data-stu-id="c88a7-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>