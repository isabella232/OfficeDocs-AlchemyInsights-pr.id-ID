---
title: Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353540"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e7257-102">Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e7257-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e7257-103">Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="e7257-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e7257-104">Beberapa pesan kesalahan umum dan langkah-langkah resolusi:</span><span class="sxs-lookup"><span data-stu-id="e7257-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e7257-105">**Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="e7257-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="e7257-106">Download ulang paket perangkat lunak PC Client di Konsol Admin Intune.</span><span class="sxs-lookup"><span data-stu-id="e7257-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="e7257-107">Meninjau dokumentasi ini untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7257-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="e7257-108">**Kode kesalahan 0x801c0003:** Kesalahan dapat terjadi dalam skenario berikut:</span><span class="sxs-lookup"><span data-stu-id="e7257-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="e7257-109">Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat.</span><span class="sxs-lookup"><span data-stu-id="e7257-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e7257-110">Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e7257-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="e7257-111">"Pengguna dapat bergabung perangkat Azure iklan" diatur ke "tidak".</span><span class="sxs-lookup"><span data-stu-id="e7257-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="e7257-112">Set ke semua atau pilih pengguna.</span><span class="sxs-lookup"><span data-stu-id="e7257-112">Set it to all or select users.</span></span> <span data-ttu-id="e7257-113">Meninjau [dokumentasi ini](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7257-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="e7257-114">Perangkat sudah terdaftar oleh pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="e7257-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="e7257-115">Jika itu adalah kasus, menghapus perangkat dari konsol Azure Intune atau secara manual unenroll perangkat sebelum mencoba lagi.</span><span class="sxs-lookup"><span data-stu-id="e7257-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="e7257-116">Perangkat ini Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="e7257-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="e7257-117">Hanya Windows 10 Pro, pendidikan dan Enterprise SKU dapat bergabung Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7257-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="e7257-118">Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="e7257-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e7257-119">Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="e7257-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e7257-120">Meninjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk rincian lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="e7257-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="e7257-121">Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e7257-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="e7257-122">[Belajar bagaimana untuk mendaftar perangkat Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="e7257-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
