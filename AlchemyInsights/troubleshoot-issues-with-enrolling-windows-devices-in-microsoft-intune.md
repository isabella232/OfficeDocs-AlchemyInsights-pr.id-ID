---
title: Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474759"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e7273-102">Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e7273-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e7273-103">Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="e7273-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e7273-104">Beberapa pesan kesalahan umum dan langkah-langkah resolusi:</span><span class="sxs-lookup"><span data-stu-id="e7273-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e7273-p101">**Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa. Download ulang paket perangkat lunak PC Client di Konsol Admin Intune. Meninjau dokumentasi ini untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7273-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="e7273-108">**Kode kesalahan 0x801c0003:** Kesalahan dapat terjadi dalam skenario berikut:</span><span class="sxs-lookup"><span data-stu-id="e7273-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="e7273-p102">Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat. Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/en-us/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e7273-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="e7273-p103">"Pengguna dapat bergabung perangkat Azure iklan" diatur ke "tidak". Set ke semua atau pilih pengguna. Meninjau [dokumentasi ini](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7273-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="e7273-p104">Perangkat sudah terdaftar oleh pengguna lain. Jika itu adalah kasus, menghapus perangkat dari konsol Azure Intune atau secara manual unenroll perangkat sebelum mencoba lagi.</span><span class="sxs-lookup"><span data-stu-id="e7273-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="e7273-p105">Perangkat ini Windows 10 Home. Hanya Windows 10 Pro, pendidikan dan Enterprise SKU dapat bergabung Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7273-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="e7273-118">Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="e7273-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e7273-p106">Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/en-us/intune/help-desk-operators) untuk rincian lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7273-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e7273-121">Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e7273-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="e7273-122">[Belajar bagaimana untuk mendaftar perangkat Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="e7273-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

