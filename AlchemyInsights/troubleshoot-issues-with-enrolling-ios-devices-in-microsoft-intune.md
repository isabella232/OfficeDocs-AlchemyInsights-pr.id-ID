---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708965"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="19ca3-102">Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="19ca3-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="19ca3-103">Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="19ca3-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="19ca3-104">Beberapa langkah pemecahan masalah dan pesan kesalahan umum:</span><span class="sxs-lookup"><span data-stu-id="19ca3-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="19ca3-105">**Kapitalisasi perangkat tercapai** Pengguna memiliki lebih banyak perangkat yang terdaftar dibandingkan batas perangkat.</span><span class="sxs-lookup"><span data-stu-id="19ca3-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="19ca3-106">Tinjau dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="19ca3-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="19ca3-107">**Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Layanan pemberitahuan push Apple (APN) perlu dikonfigurasikan atau diperbarui.</span><span class="sxs-lookup"><span data-stu-id="19ca3-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="19ca3-108">Tinjau [dokumen ini](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) untuk mendapatkan instruksi tentang cara melakukannya.</span><span class="sxs-lookup"><span data-stu-id="19ca3-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="19ca3-109">**Lisensi pengguna tipe tidak valid atau nama pengguna tidak dikenali:** Pengguna harus diberi lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="19ca3-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="19ca3-110">Tinjau dokumen ini untuk menetapkan lisensi melalui: [Pusat admin Office](https://docs.microsoft.com/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="19ca3-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="19ca3-111">Sumber daya tambahan untuk membantu mengatasi masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="19ca3-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="19ca3-112">Gunakan [portal pemecahan masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="19ca3-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="19ca3-113">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="19ca3-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="19ca3-114">Tinjau dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan pemecahan](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) masalah dan dokumen [pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="19ca3-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="19ca3-115">[Pelajari cara mendaftarkan perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="19ca3-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

