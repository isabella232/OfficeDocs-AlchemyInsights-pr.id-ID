---
title: Memecahkan masalah masuk tunggal untuk perangkat yang bergabung dengan Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036172"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="52874-102">Memecahkan masalah masuk tunggal untuk perangkat yang bergabung dengan Azure AD</span><span class="sxs-lookup"><span data-stu-id="52874-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="52874-103">Jika Anda memiliki lingkungan direktori aktif (AD) di tempat dan Anda ingin bergabung dengan komputer yang tergabung dalam domain-domain ke Azure AD, Anda bisa mencapainya dengan melakukan gabungan Azure AD Exchange.</span><span class="sxs-lookup"><span data-stu-id="52874-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="52874-104">[Cara: merencanakan penerapan hibrid Azure Active Directory gabungan](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) memberi Anda langkah terkait untuk menerapkan gabungan Azure AD di lingkungan Anda.</span><span class="sxs-lookup"><span data-stu-id="52874-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="52874-105">Untuk informasi selengkapnya, lihat [mengonfigurasi perangkat yang bergabung dengan AZURE AD untuk Single-Sign di tempat untuk menggunakan Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="52874-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="52874-106">**Masalah token refresh utama (PRT)**</span><span class="sxs-lookup"><span data-stu-id="52874-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="52874-107">Token refresh utama (PRT) adalah artefak kunci Azure AD Authentication pada Windows 10, Windows Server 2016 dan versi yang lebih baru, iOS, dan perangkat Android.</span><span class="sxs-lookup"><span data-stu-id="52874-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="52874-108">Ini adalah JSON web Token (JWT) yang diterbitkan secara khusus untuk pialang Microsoft pihak pertama untuk mengaktifkan masuk tunggal (SSO) di seluruh aplikasi yang digunakan pada perangkat tersebut.</span><span class="sxs-lookup"><span data-stu-id="52874-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="52874-109">Untuk detail tentang cara PRT dikeluarkan, digunakan, dan diproteksi pada perangkat Windows 10, lihat [apa itu token refresh utama?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="52874-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="52874-110">**WamDefaultSet: Ya dan AzureADPrt: Ya**</span><span class="sxs-lookup"><span data-stu-id="52874-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="52874-111">Bidang ini menunjukkan apakah pengguna telah berhasil diautentikasi ke Azure AD saat masuk ke perangkat.</span><span class="sxs-lookup"><span data-stu-id="52874-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="52874-112">Jika nilai **tidak**, itu mungkin karena:</span><span class="sxs-lookup"><span data-stu-id="52874-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="52874-113">Kunci penyimpanan yang buruk dalam TPM yang terkait dengan perangkat saat pendaftaran (periksa tombol uji saat menjalankan peningkatan)</span><span class="sxs-lookup"><span data-stu-id="52874-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="52874-114">ID masuk alternatif</span><span class="sxs-lookup"><span data-stu-id="52874-114">Alternate Login ID</span></span>
- <span data-ttu-id="52874-115">Proksi HTTP tidak ditemukan</span><span class="sxs-lookup"><span data-stu-id="52874-115">HTTP Proxy not found</span></span>

<span data-ttu-id="52874-116">Untuk memecahkan masalah perangkat menggunakan perintah dsregcmd, lihat [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="52874-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
