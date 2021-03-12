---
title: Mengonfigurasi dan memvalidasi pengecualian untuk MDATP pada mesin Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746021"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="87025-102">Mengonfigurasi dan memvalidasi pengecualian untuk MDATP pada mesin Linux</span><span class="sxs-lookup"><span data-stu-id="87025-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="87025-103">Anda bisa mengecualikan file, folder, proses, dan file tertentu yang dibuka dari pemindaian MDATP.</span><span class="sxs-lookup"><span data-stu-id="87025-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="87025-104">Pengecualian membantu mencegah deteksi perangkat lunak dan file yang salah atau dikustomisasi ke organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="87025-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="87025-105">Pengecualian juga membantu mengurangi masalah kinerja yang disebabkan oleh MDATP.</span><span class="sxs-lookup"><span data-stu-id="87025-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="87025-106">Untuk mempelajari selengkapnya, lihat [mengonfigurasi dan memvalidasi pengecualian untuk MDATP untuk Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="87025-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="87025-107">Pengecualian yang diuraikan dalam artikel ini tidak berlaku untuk kapabilitas lain dari MDATP untuk Linux, termasuk deteksi titik akhir dan respons (EDR).</span><span class="sxs-lookup"><span data-stu-id="87025-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="87025-108">File yang Anda kecualikan dengan menggunakan metode yang diuraikan dalam artikel ini masih dapat memicu peringatan EDR dan kapabilitas deteksi lainnya.</span><span class="sxs-lookup"><span data-stu-id="87025-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
