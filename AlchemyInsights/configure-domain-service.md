---
title: Mengonfigurasi layanan domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885220"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="e854f-102">Tidak dapat mengaktifkan AAD-DS atau Deployment gagal</span><span class="sxs-lookup"><span data-stu-id="e854f-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="e854f-103">Untuk mengatasi masalah layanan domain Azure AD (AAD-DS) yang tidak diaktifkan atau gagal untuk disebarkan, lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="e854f-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="e854f-104">Jika Anda menggunakan jaringan virtual yang sudah ada, periksa NSG Anda untuk aturan yang diperlukan untuk menyinkronkan Port dalam AAD-DS di portal https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="e854f-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="e854f-105">Periksa untuk melihat apakah pesan kesalahan Anda dijawab dalam panduan pemecahan masalah yang tersedia di  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="e854f-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="e854f-106">Cobalah menyebarkan layanan domain Azure AD di jaringan virtual baru.</span><span class="sxs-lookup"><span data-stu-id="e854f-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="e854f-107">Ikuti panduan memulai tentang cara menggunakan AAD-DS: [membuat dan mengonfigurasi layanan domain AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="e854f-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="e854f-108">Jika Anda mengalami masalah dalam menyebarkan layanan domain Azure AD, lihat [memecahkan masalah layanan domain AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) untuk mengatasi kesalahan umum untuk membantu Anda menyelesaikan pekerjaan.</span><span class="sxs-lookup"><span data-stu-id="e854f-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="e854f-109">**Tidak dapat menonaktifkan AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="e854f-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="e854f-110">AAD-DS tidak dapat dihentikan sebentar.</span><span class="sxs-lookup"><span data-stu-id="e854f-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="e854f-111">Jika ingin berhenti menggunakan domain terkelola, Anda harus dihapus.</span><span class="sxs-lookup"><span data-stu-id="e854f-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="e854f-112">Untuk menghapus domain terkelola Anda, lihat [menghapus layanan domain AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="e854f-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



