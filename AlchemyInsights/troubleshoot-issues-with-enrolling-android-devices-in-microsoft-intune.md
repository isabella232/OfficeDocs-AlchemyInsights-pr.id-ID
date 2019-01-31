---
title: Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655886"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="838bd-102">Memecahkan masalah dengan mendaftarkan perangkat Android di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="838bd-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="838bd-103">Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="838bd-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="838bd-104">Beberapa masalah umum dan langkah-langkah resolusi:</span><span class="sxs-lookup"><span data-stu-id="838bd-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="838bd-p101">**Perangkat tidak dienkripsi kesalahan dalam Portal perusahaan:** Versi Android, khususnya diawali v7.0, memerlukan passcode startup untuk memastikan bahwa perangkat Anda dienkripsi penuh. Solusi umum akan mengaktifkan startup pin atau sepenuhnya mengenkripsi perangkat. Meninjau [dokumen ini](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="838bd-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="838bd-p102">**Perangkat gagal untuk check-in Layanan Intune atau menampilkan sebagai "Tidak sehat" di konsol admin Intune:** Beberapa 4.4 Samsung dan 5.5 perangkat tidak dapat memeriksa ke layanan. Ada 3 kemungkinan solusi untuk masalah ini:</span><span class="sxs-lookup"><span data-stu-id="838bd-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="838bd-110">Secara manual membuka app Intune perusahaan Portal, yang akan secara otomatis memulai sinkronisasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="838bd-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="838bd-111">Memperbarui perangkat untuk Android 6.0 atau lebih tinggi.</span><span class="sxs-lookup"><span data-stu-id="838bd-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="838bd-p103">Menonaktifkan Samsung Smart Manager dari mengelola Intune Portal perusahaan. Meninjau [dokumen ini](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) untuk rincian lebih lanjut pada masalah ini dan resolusi.</span><span class="sxs-lookup"><span data-stu-id="838bd-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="838bd-p104">**Pengguna lisensi jenis tidak valid** atau **kesalahan pengguna nama tidak dikenali:** kebutuhan pengguna akan diberikan izin Intune atau EMS. Meninjau dokumen-dokumen ini untuk menetapkan lisensi melalui: portal kantor Admin Center atau Azure.</span><span class="sxs-lookup"><span data-stu-id="838bd-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="838bd-116">Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="838bd-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="838bd-p105">Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk rincian lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="838bd-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="838bd-119">Meninjau [dokumen ini](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing.</span><span class="sxs-lookup"><span data-stu-id="838bd-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="838bd-120">[Belajar bagaimana untuk mendaftar perangkat Android di Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="838bd-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

