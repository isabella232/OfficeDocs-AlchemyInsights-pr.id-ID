---
title: Mengonfigurasi pengecualian untuk ATP Pertahanan Microsoft pemindaian
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543688"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="c61ac-102">Mengonfigurasi pengecualian untuk ATP Pertahanan Microsoft pemindaian</span><span class="sxs-lookup"><span data-stu-id="c61ac-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="c61ac-103">Secara umum, Anda dapat mengecualikan ekstensi file dan lokasi folder tertentu dari ATP Pertahanan Microsoft pemindaian.</span><span class="sxs-lookup"><span data-stu-id="c61ac-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="c61ac-104">Anda juga dapat mengonfigurasi pengecualian untuk file yang dibuka oleh proses tertentu.</span><span class="sxs-lookup"><span data-stu-id="c61ac-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="c61ac-105">Untuk informasi selengkapnya, lihat Mengonfigurasi dan [memvalidasi pengecualian](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) berdasarkan ekstensi file dan lokasi folder dan Mengonfigurasi pengecualian untuk file yang dibuka oleh [proses](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="c61ac-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="c61ac-106">Untuk mengonfigurasi pengecualian untuk **Windows Server 2016 dan 2019,** lihat Mengonfigurasi [Antivirus Pertahanan Microsoft pengecualian di Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="c61ac-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c61ac-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="c61ac-107">**Mac**</span></span>

<span data-ttu-id="c61ac-108">Untuk detail tentang tipe pengecualian yang didukung dan mengonfigurasi daftar pengecualian untuk Mac, lihat [Tipe](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) pengecualian yang didukung dan Cara [mengonfigurasi daftar pengecualian.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="c61ac-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="c61ac-109">**Catatan** Anda juga bisa memvalidasi daftar pengecualian menggunakan file uji EICAR.</span><span class="sxs-lookup"><span data-stu-id="c61ac-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="c61ac-110">Untuk informasi selengkapnya, [lihat Memvalidasi daftar pengecualian dengan file uji EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="c61ac-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="c61ac-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="c61ac-111">**Linux**</span></span>

<span data-ttu-id="c61ac-112">Untuk detail tentang tipe pengecualian yang didukung dan mengonfigurasi daftar [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) pengecualian untuk Linux, lihat Tipe pengecualian yang didukung dan Mengonfigurasi dan memvalidasi pengecualian [untuk ATP Pertahanan Microsoft untuk Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="c61ac-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="c61ac-113">**Catatan** Anda juga bisa memvalidasi daftar pengecualian menggunakan file uji EICAR.</span><span class="sxs-lookup"><span data-stu-id="c61ac-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="c61ac-114">Untuk informasi selengkapnya, [lihat Memvalidasi daftar pengecualian dengan file uji EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="c61ac-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 