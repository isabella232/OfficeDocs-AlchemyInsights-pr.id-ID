---
title: Masalah dalam mengembangkan aplikasi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974472"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="19004-102">Masalah dalam mengembangkan aplikasi</span><span class="sxs-lookup"><span data-stu-id="19004-102">Issues developing applications</span></span>

<span data-ttu-id="19004-103">Untuk memecahkan masalah paling umum ketika membuat aplikasi Azure Active Directory (AD), lihat artikel berikut ini:</span><span class="sxs-lookup"><span data-stu-id="19004-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="19004-104">Saya mengalami masalah saat masuk ke aplikasi menggunakan browser Chrome saja</span><span class="sxs-lookup"><span data-stu-id="19004-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="19004-105">Saya tidak tahu cara mengubah default seumur hidup token untuk aplikasi saya</span><span class="sxs-lookup"><span data-stu-id="19004-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="19004-106">Saya bingung tentang cara kerja persetujuan aplikasi</span><span class="sxs-lookup"><span data-stu-id="19004-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="19004-107">Saya tidak tahu cara memberikan izin ke aplikasi saya</span><span class="sxs-lookup"><span data-stu-id="19004-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="19004-108">Saya tidak memahami perbedaan antara izin delegasi dan aplikasi</span><span class="sxs-lookup"><span data-stu-id="19004-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="19004-109">\***Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan AZURE AD GRAPH api (GRAF AAD)** _</span><span class="sxs-lookup"><span data-stu-id="19004-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="19004-110">Mulai tanggal 30 Juni 2020, kami tidak akan lagi menambahkan fitur baru ke pustaka autentikasi direktori aktif Azure (ADAL) dan Azure AD graph API (Graf AAD).</span><span class="sxs-lookup"><span data-stu-id="19004-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="19004-111">Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan tetapi tidak lagi menyediakan pembaruan fitur.</span><span class="sxs-lookup"><span data-stu-id="19004-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="19004-112">Mulai 30 Juni 2022, kami akan mengakhiri dukungan untuk Graf ADAL dan AAD dan tidak lagi menyediakan dukungan teknis atau pembaruan keamanan.</span><span class="sxs-lookup"><span data-stu-id="19004-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="19004-113">Sebagai akibat dari kondisi ini, berikut ini adalah implikasi:</span><span class="sxs-lookup"><span data-stu-id="19004-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="19004-114">Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.</span><span class="sxs-lookup"><span data-stu-id="19004-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="19004-115">Aplikasi menggunakan grafik AAD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Graf AAD</span><span class="sxs-lookup"><span data-stu-id="19004-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="19004-116">_ *Migrasi ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="19004-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="19004-117">Jika Anda menggunakan aplikasi Microsoft, sebaiknya Perbarui ke Microsoft Authentication Library (MSAL), yang memiliki fitur dan pembaruan keamanan terbaru.</span><span class="sxs-lookup"><span data-stu-id="19004-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="19004-118">Rekomendasi ini adalah dalam konteks Microsoft memulai proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir.</span><span class="sxs-lookup"><span data-stu-id="19004-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="19004-119">Migrasi dengan Microsoft dari aplikasinya ke MSAL memastikan bahwa aplikasi tersebut mendapatkan manfaat dari penyempurnaan fitur dan keamanan yang sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="19004-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="19004-120">Membaca FAQ ADAL</span><span class="sxs-lookup"><span data-stu-id="19004-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="19004-121">Pelajari tentang cara melakukan migrasi aplikasi secara per platform</span><span class="sxs-lookup"><span data-stu-id="19004-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="19004-122">Jika Anda memerlukan bantuan dalam memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda dan, jika ada, menjangkau ke vendor perangkat lunak independen (ISVs) atau penyedia aplikasi.</span><span class="sxs-lookup"><span data-stu-id="19004-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="19004-123">Dukungan Microsoft juga bisa memberi Anda daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="19004-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="19004-124">**Migrasi Graf AAD**</span><span class="sxs-lookup"><span data-stu-id="19004-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="19004-125">Untuk aplikasi yang menggunakan grafik AAD, ikuti panduan kami untuk melakukan migrasi aplikasi Graf AAD ke Microsoft graph:</span><span class="sxs-lookup"><span data-stu-id="19004-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="19004-126">[Daftar Periksa migrasi kami menyediakan titik mulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="19004-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="19004-127">Portal pendaftaran aplikasi Azure memperlihatkan aplikasi mana yang menggunakan grafik AAD.</span><span class="sxs-lookup"><span data-stu-id="19004-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="19004-128">Kami menyarankan agar Anda meninjau semua kode sumber aplikasi dan, jika ada, menjangkau ke vendor perangkat lunak independen (ISVs) atau penyedia aplikasi.</span><span class="sxs-lookup"><span data-stu-id="19004-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="19004-129">Dukungan Microsoft juga bisa memberi Anda informasi tentang penggunaan grafik AAD dalam penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="19004-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







