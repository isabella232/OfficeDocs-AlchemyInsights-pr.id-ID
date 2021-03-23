---
title: Koneksi AAD pemberitahuan
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036109"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="17a67-102">Koneksi AAD pemberitahuan</span><span class="sxs-lookup"><span data-stu-id="17a67-102">Notification AAD Connect</span></span>

- <span data-ttu-id="17a67-103">Pastikan Anda memiliki wewenang untuk melakukan operasi.</span><span class="sxs-lookup"><span data-stu-id="17a67-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="17a67-104">Admin global memiliki akses secara default.</span><span class="sxs-lookup"><span data-stu-id="17a67-104">Global Admins have access by default.</span></span> <span data-ttu-id="17a67-105">Selain itu, Anda bisa menggunakan [kontrol akses berbasis peran](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) untuk mendelegasikan izin pendaftaran ke kontributor.</span><span class="sxs-lookup"><span data-stu-id="17a67-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="17a67-106">Pastikan titik akhir yang diperlukan diaktifkan, dan tidak diblokir karena firewall.</span><span class="sxs-lookup"><span data-stu-id="17a67-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="17a67-107">Untuk detailnya, lihat [persyaratan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="17a67-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="17a67-108">Pendaftaran dapat gagal karena komunikasi keluar menjadi sasaran inspeksi SSL oleh lapisan jaringan.</span><span class="sxs-lookup"><span data-stu-id="17a67-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="17a67-109">Pastikan Anda telah memverifikasi pengaturan pemberitahuan untuk kesehatan Azure AD Connect dan Tinjau pengaturan Anda.</span><span class="sxs-lookup"><span data-stu-id="17a67-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="17a67-110">Untuk memahami cara mengonfigurasi pengaturan pemberitahuan untuk pemberitahuan kesehatan Azure AD Connect, lihat [panduan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)ini.</span><span class="sxs-lookup"><span data-stu-id="17a67-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="17a67-111">Untuk mempelajari selengkapnya tentang laporan sinkronisasi kesehatan AAD Connect dan cara mengunduhnya, lihat [laporan tingkat objek sinkronisasi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="17a67-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="17a67-112">Untuk memecahkan masalah pemberitahuan kesehatan AAD Connect ikuti [panduan pemecahan masalah untuk data kesehatan pemberitahuan KESEGARAN AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) dan untuk tanya umum, lihat [pertanyaan umum penginstalan kesehatan AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="17a67-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
