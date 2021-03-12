---
title: Mengonfigurasi pengecualian untuk pemindaian ATP Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713897"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="5a39e-102">Mengonfigurasi pengecualian untuk pemindaian ATP Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="5a39e-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="5a39e-103">Secara umum, Anda bisa mengecualikan ekstensi file dan lokasi folder tertentu dari pemindaian Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="5a39e-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="5a39e-104">Anda juga bisa mengonfigurasi pengecualian untuk file yang dibuka oleh proses tertentu.</span><span class="sxs-lookup"><span data-stu-id="5a39e-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="5a39e-105">Untuk informasi selengkapnya, lihat, [mengonfigurasi dan memvalidasi pengecualian berdasarkan ekstensi file dan lokasi folder](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) serta [mengonfigurasi pengecualian untuk file yang dibuka oleh proses](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="5a39e-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="5a39e-106">Untuk mengonfigurasi pengecualian untuk  **Windows server 2016 dan 2019**, lihat [mengonfigurasi pengecualian antivirus Microsoft Defender di Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="5a39e-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="5a39e-107">**Mak**</span><span class="sxs-lookup"><span data-stu-id="5a39e-107">**Mac**</span></span>

<span data-ttu-id="5a39e-108">Untuk detail tentang tipe pengecualian yang didukung dan mengonfigurasi daftar pengecualian untuk Mac, lihat [tipe pengecualian yang didukung](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) dan [cara mengonfigurasi daftar pengecualian](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="5a39e-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="5a39e-109">**Catatan** Anda juga bisa memvalidasi daftar pengecualian menggunakan file uji EICAR.</span><span class="sxs-lookup"><span data-stu-id="5a39e-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="5a39e-110">Untuk informasi selengkapnya, lihat [memvalidasi daftar pengecualian dengan file uji EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="5a39e-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="5a39e-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="5a39e-111">**Linux**</span></span>

<span data-ttu-id="5a39e-112">Untuk detail tentang tipe pengecualian yang didukung dan mengonfigurasi daftar pengecualian untuk Linux, lihat [tipe pengecualian yang didukung](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) serta [konfigurasi dan validasi pengecualian untuk Microsoft Defender ATP untuk Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="5a39e-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="5a39e-113">**Catatan** Anda juga bisa memvalidasi daftar pengecualian menggunakan file uji EICAR.</span><span class="sxs-lookup"><span data-stu-id="5a39e-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="5a39e-114">Untuk informasi selengkapnya, lihat [memvalidasi daftar pengecualian dengan file uji EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="5a39e-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 