---
title: Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391010"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="0b313-102">Memecahkan masalah dengan mendaftarkan perangkat iOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0b313-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="0b313-103">Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="0b313-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0b313-104">Beberapa pesan kesalahan umum dan langkah-langkah resolusi:</span><span class="sxs-lookup"><span data-stu-id="0b313-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="0b313-105">**Perangkat Cap mencapai** Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat.</span><span class="sxs-lookup"><span data-stu-id="0b313-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0b313-106">Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0b313-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="0b313-107">**Layanan ini tidak didukung. Tidak ada kebijakan pendaftaran:** Apple mendorong pemberitahuan Layanan (APNS) perlu dikonfigurasi atau diperbaharui.</span><span class="sxs-lookup"><span data-stu-id="0b313-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="0b313-108">Meninjau [dokumen ini](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) untuk petunjuk tentang cara untuk melakukan itu.</span><span class="sxs-lookup"><span data-stu-id="0b313-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="0b313-109">**Pengguna lisensi jenis valid atau nama pengguna tidak dikenal:** Kebutuhan pengguna akan diberikan izin Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="0b313-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="0b313-110">Meninjau dokumen-dokumen ini untuk menetapkan lisensi melalui: [Kantor Admin Center](https://docs.microsoft.com/intune/licenses-assign) atau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="0b313-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="0b313-111">Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="0b313-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0b313-112">Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="0b313-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0b313-113">Meninjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk rincian lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="0b313-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0b313-114">Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0b313-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="0b313-115">[Belajar bagaimana untuk mendaftar perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="0b313-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

