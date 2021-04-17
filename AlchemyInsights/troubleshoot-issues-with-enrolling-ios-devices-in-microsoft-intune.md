---
title: Memecahkan masalah pendaftaran perangkat iOS di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823466"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1d454-102">Memecahkan masalah pendaftaran perangkat iOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1d454-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1d454-103">Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="1d454-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1d454-104">Beberapa pesan kesalahan umum dan langkah penyelesaian:</span><span class="sxs-lookup"><span data-stu-id="1d454-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1d454-105">**Jumlah Perangkat Tercapai** Pengguna telah mendaftarkan lebih banyak perangkat daripada batas perangkat.</span><span class="sxs-lookup"><span data-stu-id="1d454-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1d454-106">Tinjau dokumen ini [untuk menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau mengubah batas [perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="1d454-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1d454-107">**Layanan ini tidak didukung. Tidak Ada Kebijakan Pendaftaran:** Apple Push Notification Service (APNS) harus dikonfigurasi atau diperbarui.</span><span class="sxs-lookup"><span data-stu-id="1d454-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="1d454-108">Tinjau [dokumen](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ini untuk mendapatkan instruksi tentang cara melakukannya.</span><span class="sxs-lookup"><span data-stu-id="1d454-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1d454-109">**Tipe Lisensi Pengguna Tidak Valid atau Nama Pengguna Tidak Dikenali:** Pengguna harus diberi lisensi Intune atau EMS.</span><span class="sxs-lookup"><span data-stu-id="1d454-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1d454-110">Tinjau dokumen ini untuk menetapkan lisensi melalui: [Pusat Admin Office](https://docs.microsoft.com/intune/licenses-assign) atau portal [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="1d454-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1d454-111">Sumber daya tambahan untuk membantu mengatasi masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="1d454-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1d454-112">Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="1d454-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1d454-113">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="1d454-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1d454-114">Tinjau dokumen ini untuk melihat daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing dokumen: [Panduan pemecahan masalah](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) dan Dokumen pemecahan [masalah.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="1d454-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1d454-115">[Pelajari cara mendaftarkan perangkat iOS di Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="1d454-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

