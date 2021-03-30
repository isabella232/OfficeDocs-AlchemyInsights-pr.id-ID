---
title: Memecahkan masalah bergabung di Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405128"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="7ce89-102">Memecahkan masalah bergabung di Azure AD</span><span class="sxs-lookup"><span data-stu-id="7ce89-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="7ce89-103">Jika Anda menyiapkan pendaftaran perangkat untuk kali pertama, pastikan Anda telah meninjau Pengenalan pada manajemen perangkat di [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) yang akan memandu Anda tentang cara mendapatkan Perangkat di bawah kontrol ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ce89-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="7ce89-104">Jika mendaftarkan perangkat ke Azure AD secara langsung dan mendaftarkan perangkat ke Intune, Pastikan Anda telah mengonfigurasi [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) dan lisensinya tersedia terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="7ce89-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="7ce89-105">Pastikan Anda memiliki wewenang untuk melakukan operasi di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ce89-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="7ce89-106">Hanya administrator global di Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat.</span><span class="sxs-lookup"><span data-stu-id="7ce89-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="7ce89-107">Untuk melakukan implementasi bergabung di Azure AD, lihat [Merencanakan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="7ce89-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="7ce89-108">Untuk detail selengkapnya tentang mengatasi masalah umum dengan Azure AD bergabung, lihat [FAQ Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) dan untuk perangkat pro Windows 10, lihat Tidak dapat bergabung ke komputer Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) ke Azure AD - Perlu memutakhirkan ke - Microsoft Community</span><span class="sxs-lookup"><span data-stu-id="7ce89-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
