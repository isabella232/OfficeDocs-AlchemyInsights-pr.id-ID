---
title: Memecahkan masalah gabungan Hybrid Microsoft Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401910"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="06892-102">Memecahkan masalah gabungan Hybrid Microsoft Azure AD</span><span class="sxs-lookup"><span data-stu-id="06892-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="06892-103">Sangat Disarankan untuk Memastikan bahwa perangkat dapat mengakses titik akhir Pendaftaran Perangkat di bawah akun sistem dengan menggunakan [skrip Konektivitas Pendaftaran Perangkat Uji](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="06892-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="06892-104">Jika Anda menyiapkan pendaftaran perangkat untuk pertama kalinya, pastikan untuk meninjau [Pengenalan manajemen perangkat di Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) untuk mempelajari cara mendapatkan perangkat di bawah kontrol Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06892-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="06892-105">Jika Anda mendaftarkan perangkat ke Microsoft Azure AD secara langsung dan mendaftarkannya ke Intune, pastikan Anda telah [mengonfigurasi Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) dan memiliki [lisensinya](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="06892-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="06892-106">Pastikan Anda telah mendapatkan izin untuk melakukan operasi di Microsoft Azure AD dan AD lokal.</span><span class="sxs-lookup"><span data-stu-id="06892-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="06892-107">Hanya administrator global di Microsoft Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat.</span><span class="sxs-lookup"><span data-stu-id="06892-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="06892-108">Selain itu, jika Anda menyiapkan pendaftaran otomatis di Active Directory lokal, Anda perlu menjadi administrator Active Directory dan AD FS (jika berlaku).</span><span class="sxs-lookup"><span data-stu-id="06892-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="06892-109">Untuk detail selengkapnya tentang mengatasi potensi masalah dengan gabungan Hibrid, lihat[Mengatasi Masalah Gabungan Hibrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) dan untuk menyiapkan hibrid Azure AD yang tergabung serta Mengelola Perangkat menggunakan portal Microsoft Azure AD, lihat[Menyiapkan perangkat gabungan hibrid Microsoft Azure AD (bergabung dengan domain lokal)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) dan [Mengelola perangkat menggunakan portal Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="06892-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="06892-110">Untuk mengatasi masalah umum dengan gabungan Hibrid Azure Active Directory (AD), lihat [FAQ gabungan Hibrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="06892-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
