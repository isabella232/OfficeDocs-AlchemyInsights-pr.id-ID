---
title: Dukungan Microsoft Edge untuk Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583581"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="7f653-102">Dukungan Microsoft Edge untuk Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="7f653-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="7f653-103">Didesain untuk Windows 10 dan Microsoft Edge, aplikasi Guard menggunakan pendekatan isolasi perangkat keras yang memungkinkan pengguna menavigasi situs tidak tepercaya dari dalam wadah yang terisolasi dan Hyper-V yang diaktifkan, dipisahkan dari sistem operasi host.</span><span class="sxs-lookup"><span data-stu-id="7f653-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="7f653-104">Admin perusahaan menentukan daftar situs web tepercaya, sumber daya awan, dan jaringan internal.</span><span class="sxs-lookup"><span data-stu-id="7f653-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="7f653-105">Saat pengguna mengunjungi situs yang tidak ada di daftar, Microsoft Edge akan membuka situs tersebut dalam wadah.</span><span class="sxs-lookup"><span data-stu-id="7f653-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="7f653-106">Ini berarti bahwa jika situs ternyata berbahaya, PC host akan tetap terlindung dan penyerang tidak bisa masuk ke data perusahaan.</span><span class="sxs-lookup"><span data-stu-id="7f653-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="7f653-107">Penginstalan ekstensi dalam wadah didukung sebagai Microsoft Edge versi 81, dan dapat dikontrol melalui kebijakan.</span><span class="sxs-lookup"><span data-stu-id="7f653-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="7f653-108">Alamat updateURL yang akan digunakan dalam kebijakan ExtensionInstallForcelist harus ditambahkan sebagai sumber daya netral dalam kebijakan isolasi jaringan yang digunakan oleh penjaga aplikasi.</span><span class="sxs-lookup"><span data-stu-id="7f653-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="7f653-109">Untuk informasi selengkapnya, lihat [dukungan Microsoft Edge untuk Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="7f653-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
