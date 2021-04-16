---
title: Memecahkan masalah pendaftaran perangkat Windows di Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808974"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="6eb6f-102">Memecahkan masalah pendaftaran perangkat Windows di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6eb6f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="6eb6f-103">Tinjau sumber daya yang tercantum di bawah ini untuk mengatasi masalah Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6eb6f-104">Beberapa pesan kesalahan umum dan langkah penyelesaian:</span><span class="sxs-lookup"><span data-stu-id="6eb6f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="6eb6f-105">**Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="6eb6f-106">Unduh ulang paket perangkat lunak Klien PC di Konsol Admin Intune.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="6eb6f-107">Tinjau dokumentasi ini untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="6eb6f-108">**Kode kesalahan 0x801c0003:** Kesalahan dapat terjadi pada skenario berikut:</span><span class="sxs-lookup"><span data-stu-id="6eb6f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="6eb6f-109">Pengguna telah mendaftarkan lebih banyak perangkat daripada batas perangkat.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6eb6f-110">Tinjau dokumen ini [untuk menghapus perangkat](https://docs.microsoft.com/intune/devices-wipe) atau mengubah batas [perangkat](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="6eb6f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="6eb6f-111">"Pengguna dapat menggabungkan perangkat ke Azure AD" diatur ke "tidak ada."</span><span class="sxs-lookup"><span data-stu-id="6eb6f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="6eb6f-112">Atur ke semua atau pilih pengguna.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-112">Set it to all or select users.</span></span> <span data-ttu-id="6eb6f-113">Tinjau [dokumentasi ini](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="6eb6f-114">Perangkat tersebut sudah didaftarkan oleh pengguna lain.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="6eb6f-115">Jika demikian, hapus perangkat dari konsol Azure Intune atau hapus pendaftaran perangkat secara manual sebelum mencoba lagi.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="6eb6f-116">Perangkatnya adalah Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="6eb6f-117">Hanya SKU Windows 10 Pro, Pendidikan, dan Perusahaan yang dapat bergabung dengan Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="6eb6f-118">Sumber daya tambahan untuk membantu mengatasi masalah Anda:</span><span class="sxs-lookup"><span data-stu-id="6eb6f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="6eb6f-119">Gunakan [Portal Pemecahan Masalah Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosis dan mengatasi kegagalan pendaftaran umum.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6eb6f-120">Tinjau [dokumen ini](https://docs.microsoft.com/intune/help-desk-operators) untuk detail selengkapnya.</span><span class="sxs-lookup"><span data-stu-id="6eb6f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="6eb6f-121">Tinjau dokumen ini untuk melihat daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing dokumen: [Panduan pemecahan masalah](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) dan Dokumen pemecahan [masalah.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="6eb6f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="6eb6f-122">[Pelajari cara mendaftarkan perangkat Windows di Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="6eb6f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
