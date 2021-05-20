---
title: Masalah penginstalan Pertahanan Microsoft di Mac atau Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539683"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="a664e-102">Masalah penginstalan Pertahanan Microsoft di Mac atau Linux</span><span class="sxs-lookup"><span data-stu-id="a664e-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="a664e-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="a664e-103">**Mac**</span></span>

- <span data-ttu-id="a664e-104">Pastikan bahwa persyaratan sistem terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Mac.</span><span class="sxs-lookup"><span data-stu-id="a664e-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="a664e-105">Untuk informasi selengkapnya, [lihat Cara menginstal ATP Pertahanan Microsoft untuk Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="a664e-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="a664e-106">Tinjau informasi dalam file: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="a664e-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="a664e-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="a664e-107">**Linux**</span></span>

- <span data-ttu-id="a664e-108">Pastikan bahwa persyaratan sistem telah terpenuhi sebelum menginstal ATP Pertahanan Microsoft untuk Linux.</span><span class="sxs-lookup"><span data-stu-id="a664e-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="a664e-109">Untuk informasi selengkapnya, [lihat Cara menginstal MDATP untuk Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="a664e-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="a664e-110">Untuk memverifikasi bahwa layanan MDATP sedang berjalan, [lihat Penginstalan gagal.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="a664e-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="a664e-111">Untuk memecahkan dan mengatasi masalah jika layanan tidak berjalan, lihat [Langkah-langkah untuk memecahkan masalah jika layanan mdatp tidak berjalan.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="a664e-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="a664e-112">Untuk langkah-langkah untuk memeriksa konfigurasi klien, yang memverifikasi kesehatan produk, dan untuk menjalankan uji deteksi pada file teks EICAR, lihat [Konfigurasi klien](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="a664e-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="a664e-113">**Catatan** Untuk daftar sistem file yang didukung untuk aktivitas akses, lihat ATP Pertahanan Microsoft [untuk Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="a664e-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>