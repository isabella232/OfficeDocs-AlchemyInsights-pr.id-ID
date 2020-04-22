---
title: Menggunakan alat penyebaran Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726251"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="286ba-102">Menggunakan alat penyebaran Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="286ba-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="286ba-103">Anda menggunakan alat penyebaran Office (ODT) untuk menyebarkan Office 365 versi Office.</span><span class="sxs-lookup"><span data-stu-id="286ba-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="286ba-104">Alat penyebaran Office (setup. exe) dijalankan dari baris perintah dan menggunakan konfigurasi XML file untuk menentukan apa pengaturan untuk menerapkan saat menyebarkan Office.</span><span class="sxs-lookup"><span data-stu-id="286ba-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="286ba-105">Download versi terbaru dari alat penyebaran Office dari [Microsoft download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="286ba-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="286ba-106">Gunakan [alat kustomisasi Office (Oct)](https://config.office.com) untuk memilih preferensi penyebaran dan membuat file XML konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="286ba-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="286ba-107">Ekspor file konfigurasi dan tempatkan secara lokal pada folder yang sama di mana setup. exe berada.</span><span class="sxs-lookup"><span data-stu-id="286ba-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="286ba-108">**Catatan:** Masalah penginstalan Office biasanya terjadi karena berkas konfigurasi yang salah dikonfigurasi atau terformat.</span><span class="sxs-lookup"><span data-stu-id="286ba-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="286ba-109">Untuk menghindari masalah tersebut, kami sarankan Anda menggunakan alat kustomisasi Office untuk membuat berkas konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="286ba-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="286ba-110">Anda juga dapat mengimpor berkas konfigurasi yang ada ke alat kustomisasi Office.</span><span class="sxs-lookup"><span data-stu-id="286ba-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="286ba-111">Dari wantian perintah yang ditinggikan, beralih ke lokasi di mana setup. exe berada dan menjalankan alat penyebaran Office dalam mode download dan menentukan file konfigurasi yang baru saja Anda simpan.</span><span class="sxs-lookup"><span data-stu-id="286ba-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="286ba-112">Dalam contoh ini, berkas konfigurasi bernama Configuration. xml:</span><span class="sxs-lookup"><span data-stu-id="286ba-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="286ba-113">Jalankan alat penyebaran Office dalam mode konfigurasi dan menentukan berkas konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="286ba-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="286ba-114">**Catatan:** Anda harus menjalankan langkah ini dari komputer klien di mana Anda ingin menginstal Office dan Anda harus memiliki izin administrator lokal di komputer.</span><span class="sxs-lookup"><span data-stu-id="286ba-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="286ba-115">Untuk mempelajari selengkapnya tentang cara menggunakan alat penyebaran Office untuk Microsoft 365 aplikasi untuk skenario penyebaran perusahaan, lihat [Ikhtisar alat penyebaran Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="286ba-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="286ba-116">Untuk rincian lebih lanjut tentang cara menggunakan alat kustomisasi Office, lihat [Ikhtisar alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="286ba-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
