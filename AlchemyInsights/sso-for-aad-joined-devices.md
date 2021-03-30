---
title: Single-Sign aktif untuk perangkat yang tergabung di Azure Active Directory
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405048"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="91ed6-102">Akses tunggal untuk Perangkat Bergabung Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="91ed6-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="91ed6-103">Jika memiliki lingkungan Direktori Aktif (AD) lokal dan ingin menggabungkan komputer gabungan domain AD ke Azure AD, Anda dapat melakukannya dengan melakukan gabungan hibrid Azure AD.</span><span class="sxs-lookup"><span data-stu-id="91ed6-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="91ed6-104">[Cara Untuk: Merencanakan penerapan gabungan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) hibrid akan memberi Anda langkah-langkah terkait untuk menerapkan gabungan Azure AD hibrid di lingkungan Anda.</span><span class="sxs-lookup"><span data-stu-id="91ed6-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="91ed6-105">Mengonfigurasi perangkat yang bergabung di Azure AD untuk Perangkat Single-Sign Aktif menggunakan Windows Hello untuk Bisnis</span><span class="sxs-lookup"><span data-stu-id="91ed6-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="91ed6-106">**Masalah Token Refresh Utama (PRT, Primary Refresh Token)** Token Refresh Utama (PRT) adalah artifak kunci autentikasi Azure AD di Windows 10, Windows Server 2016 dan versi yang lebih baru, perangkat iOS, dan Android.</span><span class="sxs-lookup"><span data-stu-id="91ed6-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="91ed6-107">Cara ini adalah JSON Web Token (JWT) yang diterbitkan secara khusus untuk oelar token pihak pertama Microsoft untuk mengaktifkan akses masuk tunggal (SSO) di seluruh aplikasi yang digunakan di perangkat tersebut.</span><span class="sxs-lookup"><span data-stu-id="91ed6-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="91ed6-108">[Dalam Apa itu Token Refresh Utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), kami akan menyediakan detail tentang bagaimana PRT diterbitkan, digunakan, dan dilindungi di perangkat Windows 10.</span><span class="sxs-lookup"><span data-stu-id="91ed6-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="91ed6-109">**WamDefaultSet: YES dan AzureADPrt: YES** Bidang-bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD ketika masuk ke perangkat.</span><span class="sxs-lookup"><span data-stu-id="91ed6-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="91ed6-110">Jika nilai bukan **,** hal ini mungkin disebabkan:</span><span class="sxs-lookup"><span data-stu-id="91ed6-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="91ed6-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span><span class="sxs-lookup"><span data-stu-id="91ed6-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="91ed6-112">ID Masuk Alternatif</span><span class="sxs-lookup"><span data-stu-id="91ed6-112">Alternate Login ID</span></span>
- <span data-ttu-id="91ed6-113">Proksi HTTP tidak ditemukan</span><span class="sxs-lookup"><span data-stu-id="91ed6-113">HTTP Proxy not found</span></span>

<span data-ttu-id="91ed6-114">Memecahkan masalah perangkat yang menggunakan perintah dsregcmd - [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="91ed6-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
