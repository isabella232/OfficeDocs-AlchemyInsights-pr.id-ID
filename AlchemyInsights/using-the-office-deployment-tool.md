---
title: Menggunakan alat penyebaran Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085835"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="aa604-102">Menggunakan Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="aa604-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="aa604-103">Anda menggunakan Office Deployment Tool (ODT) untuk menggunakan Office versi 365 Office.</span><span class="sxs-lookup"><span data-stu-id="aa604-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="aa604-104">Office Deployment Tool (setupodt.exe) dijalankan dari baris perintah dan menggunakan file XML konfigurasi untuk menentukan pengaturan apa yang diterapkan saat menyebarkan Office.</span><span class="sxs-lookup"><span data-stu-id="aa604-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="aa604-105">Unduh versi terbaru Office Deployment tool dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="aa604-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="aa604-106">Gunakan [alat kustomisasi Office (Oct)](https://config.office.com) untuk memilih preferensi penggunaan dan membuat file XML konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="aa604-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="aa604-107">Ekspor file konfigurasi dan tempatkan secara lokal di folder yang sama tempat setupodt.exe berada.</span><span class="sxs-lookup"><span data-stu-id="aa604-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="aa604-108">**Catatan:** Masalah penginstalan Office umumnya terjadi karena file konfigurasi yang salah dikonfigurasi atau tidak diformat.</span><span class="sxs-lookup"><span data-stu-id="aa604-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="aa604-109">Untuk menghindari masalah tersebut, kami menyarankan agar Anda menggunakan alat kustomisasi Office untuk membuat file konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="aa604-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="aa604-110">Anda juga dapat mengimpor file konfigurasi yang sudah ada ke alat kustomisasi Office.</span><span class="sxs-lookup"><span data-stu-id="aa604-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="aa604-111">Dari wantian perintah yang ditinggikan, alihkan ke lokasi tempat setupodt.exe berada dan jalankan alat penyebaran Office dalam mode Unduh dan tentukan file konfigurasi yang baru saja Anda simpan.</span><span class="sxs-lookup"><span data-stu-id="aa604-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="aa604-112">Dalam contoh ini, file konfigurasi bernama Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="aa604-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="aa604-113">4. Jalankan alat penyebaran Office dalam mode konfigurasi dan tentukan file konfigurasinya.</span><span class="sxs-lookup"><span data-stu-id="aa604-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="aa604-114">**Catatan:** Anda harus menjalankan langkah ini dari komputer klien yang ingin Anda instal Office dan Anda harus memiliki izin administrator lokal di komputer tersebut.</span><span class="sxs-lookup"><span data-stu-id="aa604-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="aa604-115">Untuk mempelajari selengkapnya tentang menggunakan Office Deployment Tool untuk aplikasi Microsoft 365 Anda untuk skenario penggunaan perusahaan, lihat [gambaran umum tentang alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="aa604-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="aa604-116">Untuk detail selengkapnya tentang cara menggunakan alat kustomisasi Office, lihat [gambaran umum alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="aa604-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
