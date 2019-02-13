---
title: Menggunakan alat penyebaran kantor
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898649"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="5902e-102">Menggunakan alat penyebaran kantor (ODT)</span><span class="sxs-lookup"><span data-stu-id="5902e-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5902e-p101">Anda menggunakan alat penyebaran kantor (ODT) untuk menyebarkan versi Office 365 kantor. Kantor penyebaran alat (setup.exe) dijalankan dari baris perintah dan menggunakan file konfigurasi XML untuk menentukan pengaturan apa yang berlaku ketika deploying kantor.</span><span class="sxs-lookup"><span data-stu-id="5902e-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="5902e-105">Download versi terbaru dari Office penyebaran alat dari [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5902e-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="5902e-p102">Gunakan [Alat kustomisasi Office (OCT)](https://config.office.com) untuk memilih preferensi penyebaran dan membuat file konfigurasi XML. Ekspor file konfigurasi dan tempat lokal di folder yang sama di mana setup.exe berada.</span><span class="sxs-lookup"><span data-stu-id="5902e-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="5902e-p103">**Catatan:** Office instalasi masalah yang sering terjadi karena untuk misconfigured atau malformatted file konfigurasi. Untuk menghindari isu-isu tersebut, kami sarankan bahwa Anda menggunakan alat kustomisasi Office untuk membuat file konfigurasi. Anda juga dapat mengimpor file-file konfigurasi yang ada ke alat kustomisasi Office.</span><span class="sxs-lookup"><span data-stu-id="5902e-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="5902e-p104">Dari ditinggikan command prompt, beralih ke lokasi mana setup.exe berada dan menjalankan alat penyebaran kantor dalam download mode dan menentukan file konfigurasi yang baru saja diselamatkan. Dalam contoh ini, konfigurasi file bernama Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="5902e-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="5902e-113">Menjalankan alat penyebaran kantor di mengkonfigurasi mode dan menentukan file konfigurasi.</span><span class="sxs-lookup"><span data-stu-id="5902e-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="5902e-114">**Catatan:** Anda harus menjalankan langkah ini dari komputer klien yang Anda ingin menginstal Office dan Anda harus memiliki izin administrator lokal pada komputer.</span><span class="sxs-lookup"><span data-stu-id="5902e-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="5902e-p105">Untuk mempelajari lebih lanjut tentang menggunakan alat penyebaran kantor untuk skenario penggunaan Office 365 ProPlus Anda, lihat [ikhtisar dari kantor penyebaran alat](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Untuk detail lebih lanjut tentang cara menggunakan alat kustomisasi Office, lihat [Ikhtisar alat kustomisasi Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="5902e-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

