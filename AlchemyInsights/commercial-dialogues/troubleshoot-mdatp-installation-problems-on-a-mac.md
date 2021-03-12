---
title: Memecahkan masalah penginstalan MDATP pada Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746301"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="28dbb-102">Memecahkan masalah penginstalan MDATP pada Mac</span><span class="sxs-lookup"><span data-stu-id="28dbb-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="28dbb-103">Jika penginstalan manual gagal, halaman **ringkasan** panduan penginstalan memperlihatkan kesalahan berikut:</span><span class="sxs-lookup"><span data-stu-id="28dbb-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="28dbb-104">"Terjadi galat selama penginstalan.</span><span class="sxs-lookup"><span data-stu-id="28dbb-104">"An error occurred during installation.</span></span> <span data-ttu-id="28dbb-105">Penginstal mengalami kesalahan yang menyebabkan penginstalan gagal.</span><span class="sxs-lookup"><span data-stu-id="28dbb-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="28dbb-106">Hubungi produsen perangkat lunak untuk mendapatkan bantuan. "</span><span class="sxs-lookup"><span data-stu-id="28dbb-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="28dbb-107">Untuk penggunaan MDM, halaman juga memperlihatkan kegagalan penginstalan umum.</span><span class="sxs-lookup"><span data-stu-id="28dbb-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="28dbb-108">Meskipun kami tidak menampilkan kesalahan yang tepat kepada pengguna akhir, kami menyimpan file log dengan kemajuan instalasi, di **/Library/logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="28dbb-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="28dbb-109">Setiap sesi instalasi menambahkan file log ini.</span><span class="sxs-lookup"><span data-stu-id="28dbb-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="28dbb-110">Untuk menampilkan hanya sesi instalasi terakhir, gunakan `sed` .</span><span class="sxs-lookup"><span data-stu-id="28dbb-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="28dbb-111">Untuk mempelajari selengkapnya, lihat [memecahkan masalah instalasi untuk Microsoft Defender ATP untuk Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="28dbb-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
