---
title: Masalah dengan AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482069"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fde56-102">Masalah dengan AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="fde56-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fde56-103">Pastikan Anda memiliki wewenang untuk melakukan operasi.</span><span class="sxs-lookup"><span data-stu-id="fde56-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fde56-104">Admin global memiliki akses secara default.</span><span class="sxs-lookup"><span data-stu-id="fde56-104">Global Admins have access by default.</span></span> <span data-ttu-id="fde56-105">Selain itu, Anda bisa menggunakan [kontrol akses berbasis peran](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) untuk mendelegasikan izin pendaftaran ke kontributor.</span><span class="sxs-lookup"><span data-stu-id="fde56-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fde56-106">Pastikan titik akhir yang diperlukan diaktifkan, dan tidak diblokir karena firewall.</span><span class="sxs-lookup"><span data-stu-id="fde56-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fde56-107">Untuk detailnya, lihat [persyaratan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="fde56-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fde56-108">Pendaftaran dapat gagal karena komunikasi keluar menjadi sasaran inspeksi SSL oleh lapisan jaringan.</span><span class="sxs-lookup"><span data-stu-id="fde56-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fde56-109">Pastikan Anda telah memverifikasi pengaturan pemberitahuan untuk kesehatan Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fde56-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fde56-110">Tinjau pengaturan Anda.</span><span class="sxs-lookup"><span data-stu-id="fde56-110">Please review your setting.</span></span> <span data-ttu-id="fde56-111">[Panduan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) ini dapat membantu Anda memahami cara mengonfigurasi pengaturan pemberitahuan untuk pemberitahuan kesehatan Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fde56-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fde56-112">Untuk mempelajari selengkapnya tentang laporan sinkronisasi kesehatan AAD Connect dan cara mengunduhnya, lihat [laporan tingkat objek sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="fde56-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fde56-113">Untuk memecahkan masalah pemberitahuan kesehatan AAD Connect, ikuti [panduan pemecahan masalah untuk menyambungkan pemberitahuan kesegaran data kesehatan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) dan tanya jawab umum, lihat [pertanyaan umum tentang penginstalan kesehatan AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="fde56-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
