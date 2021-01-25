---
title: Masalah dalam mengembangkan aplikasi dengan api
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974621"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="51d52-102">Masalah dalam mengembangkan aplikasi dengan api</span><span class="sxs-lookup"><span data-stu-id="51d52-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="51d52-103">Untuk mulai menggunakan API grafik Azure Active Directory, lihat [panduan mulai cepat AZURE AD GRAPH api](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , atau Tampilkan [dokumentasi referensi api Azure AD graph interaktif](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="51d52-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="51d52-104">**Akhir dukungan untuk Azure Active Directory Authentication Library (ADAL) dan Azure AD graph API (Graf AAD)**</span><span class="sxs-lookup"><span data-stu-id="51d52-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="51d52-105">**Mulai 30 juni 2020**, kami tidak akan lagi menambahkan fitur baru untuk ADAL dan Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="51d52-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="51d52-106">Kami akan terus menyediakan dukungan teknis dan pembaruan keamanan tetapi tidak lagi menyediakan pembaruan fitur.</span><span class="sxs-lookup"><span data-stu-id="51d52-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="51d52-107">**Mulai 30 juni 2022**, kami akan mengakhiri dukungan untuk ADAL dan Azure AD graph dan tidak akan lagi menyediakan dukungan teknis atau pembaruan keamanan.</span><span class="sxs-lookup"><span data-stu-id="51d52-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="51d52-108">Aplikasi yang menggunakan ADAL pada versi OS yang sudah ada akan terus berfungsi setelah waktu ini tetapi tidak akan mendapatkan dukungan teknis atau pembaruan keamanan apa pun.</span><span class="sxs-lookup"><span data-stu-id="51d52-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="51d52-109">Aplikasi menggunakan grafik Azure AD setelah waktu ini mungkin tidak lagi menerima respons dari titik akhir Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="51d52-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="51d52-110">**Migrasi ADAL**</span><span class="sxs-lookup"><span data-stu-id="51d52-110">**ADAL Migration**</span></span>

<span data-ttu-id="51d52-111">Sebaiknya Perbarui ke [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), yang memiliki fitur dan pembaruan keamanan terbaru.</span><span class="sxs-lookup"><span data-stu-id="51d52-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="51d52-112">Jika Anda menggunakan Microsoft Apps, Ketahuilah bahwa Microsoft sedang dalam proses migrasi aplikasinya ke MSAL dengan tenggat waktu dukungan akhir, memastikan mereka akan mendapatkan manfaat dari peningkatan keamanan dan fitur yang sedang berlangsung.</span><span class="sxs-lookup"><span data-stu-id="51d52-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="51d52-113">[Baca FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="51d52-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="51d52-114">[Pelajari tentang cara melakukan migrasi aplikasi secara per platform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="51d52-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="51d52-115">Jika Anda memerlukan bantuan untuk memahami aplikasi mana yang menggunakan ADAL, kami menyarankan agar Anda meninjau semua kode sumber aplikasi Anda, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun.</span><span class="sxs-lookup"><span data-stu-id="51d52-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="51d52-116">Dukungan Microsoft juga bisa memberi Anda daftar semua aplikasi non-Microsoft ADAL di penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="51d52-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="51d52-117">**Migrasi Graf AAD**</span><span class="sxs-lookup"><span data-stu-id="51d52-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="51d52-118">Untuk aplikasi yang menggunakan Azure AD graph, ikuti panduan kami untuk melakukan migrasi [aplikasi AZURE AD graph ke Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="51d52-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="51d52-119">[Daftar Periksa migrasi kami menyediakan titik mulai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="51d52-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="51d52-120">Portal pendaftaran aplikasi Azure memperlihatkan aplikasi mana yang menggunakan grafik AAD.</span><span class="sxs-lookup"><span data-stu-id="51d52-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="51d52-121">Kami menyarankan agar Anda meninjau semua kode sumber aplikasi, dan jika ada, hubungi penyedia ISVs atau aplikasi apa pun.</span><span class="sxs-lookup"><span data-stu-id="51d52-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="51d52-122">Dukungan Microsoft juga bisa memberi Anda daftar semua penggunaan grafik AAD dalam penyewa Anda.</span><span class="sxs-lookup"><span data-stu-id="51d52-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="51d52-123">Agar aplikasi Anda dapat mengakses data di Microsoft graph, pengguna atau administrator harus memberinya izin yang benar melalui proses persetujuan.</span><span class="sxs-lookup"><span data-stu-id="51d52-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="51d52-124">[Referensi izin Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) mencantumkan izin yang terkait dengan setiap kumpulan utama api Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="51d52-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="51d52-125">Ini juga memberikan panduan tentang cara menggunakan izin.</span><span class="sxs-lookup"><span data-stu-id="51d52-125">It also provides guidance about how to use the permissions.</span></span>
