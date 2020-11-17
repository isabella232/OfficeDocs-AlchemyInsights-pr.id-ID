---
title: Peran manajemen identitas istimewa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088881"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="b5200-102">Peran manajemen identitas istimewa (PIM)</span><span class="sxs-lookup"><span data-stu-id="b5200-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="b5200-103">**Izin tidak diberikan setelah mengaktifkan peran**</span><span class="sxs-lookup"><span data-stu-id="b5200-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="b5200-104">Saat Anda mengaktifkan peran di Azure AD Privileged Management (PIM), aktivasi mungkin tidak langsung dialihkan ke semua portal yang memerlukan peran istimewa.</span><span class="sxs-lookup"><span data-stu-id="b5200-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="b5200-105">Terkadang, meskipun perubahan disebarkan, caching web di portal mungkin mengakibatkan perubahan tidak berpengaruh dengan segera.</span><span class="sxs-lookup"><span data-stu-id="b5200-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="b5200-106">Jika aktivasi tertunda, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="b5200-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="b5200-107">Keluar dari Azure portal lalu masuk kembali.</span><span class="sxs-lookup"><span data-stu-id="b5200-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="b5200-108">Saat Anda mengaktifkan peran Azure AD atau peran sumber daya Azure, Anda akan melihat tahapan aktivasi Anda.</span><span class="sxs-lookup"><span data-stu-id="b5200-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="b5200-109">Setelah semua tahapan selesai, Anda akan melihat link ' keluar '.</span><span class="sxs-lookup"><span data-stu-id="b5200-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="b5200-110">Anda dapat menggunakan tautan ini untuk keluar. Ini akan menyelesaikan sebagian besar kasus untuk penundaan aktivasi.</span><span class="sxs-lookup"><span data-stu-id="b5200-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="b5200-111">Di PIM, verifikasi bahwa Anda tercantum sebagai anggota peran.</span><span class="sxs-lookup"><span data-stu-id="b5200-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="b5200-112">Jika Anda mengaktifkan peran administrator Exchange, pastikan Anda keluar dan masuk kembali.</span><span class="sxs-lookup"><span data-stu-id="b5200-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="b5200-113">Jika masalah masih terjadi, buka tiket dukungan dan Naikkan ini sebagai masalah.</span><span class="sxs-lookup"><span data-stu-id="b5200-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="b5200-114">Jika Anda menggunakan peran administrator Exchange Anda untuk mengakses pusat keamanan dan kepatuhan, lihat langkah berikutnya.</span><span class="sxs-lookup"><span data-stu-id="b5200-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="b5200-115">Jika Anda mengaktifkan peran untuk mengakses pusat keamanan dan kepatuhan atau jika Anda mengaktifkan peran administrator SharePoint, Anda akan mengalami beberapa penundaan aktivasi dari beberapa menit hingga beberapa jam.</span><span class="sxs-lookup"><span data-stu-id="b5200-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="b5200-116">Ini adalah masalah umum dan kami sedang bekerja sama dengan tim ini untuk mengatasi masalah ini sesegera mungkin.</span><span class="sxs-lookup"><span data-stu-id="b5200-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="b5200-117">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="b5200-117">For more information, see:</span></span>

- [<span data-ttu-id="b5200-118">Mengaktifkan peran Azure AD di PIM</span><span class="sxs-lookup"><span data-stu-id="b5200-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="b5200-119">Mengaktifkan peran sumber daya Azure saya di PIM</span><span class="sxs-lookup"><span data-stu-id="b5200-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="b5200-120">**Izin tidak dihapus setelah menonaktifkan peran atau aktivasi peran kedaluwarsa**</span><span class="sxs-lookup"><span data-stu-id="b5200-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="b5200-121">Saat Anda menonaktifkan peran dalam manajemen identitas Azure AD Privilege atau ketika periode aktivasi peran berakhir, mungkin ada penundaan ketika Anda masih memiliki akses.</span><span class="sxs-lookup"><span data-stu-id="b5200-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="b5200-122">Jika penonaktifan ditunda, ikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="b5200-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="b5200-123">Jika Anda menonaktifkan peran administrator Exchange atau periode aktivasi peran kedaluwarsa, dan Anda melihat penundaan yang signifikan sebelum izin dihapus, buka tiket dukungan dan beri tahu teknisi dukungan Anda untuk membantu Anda mengirimkan tiket dengan tim manajemen akses istimewa (PAM) di dalam kantor tentang masalah ini.</span><span class="sxs-lookup"><span data-stu-id="b5200-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="b5200-124">Jika periode aktivasi telah kedaluwarsa, tapi Anda masih memiliki sesi browser terbuka, tutup browser Anda.</span><span class="sxs-lookup"><span data-stu-id="b5200-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="b5200-125">Anda dapat terus menggunakan peran hingga Anda menutup sesi tersebut.</span><span class="sxs-lookup"><span data-stu-id="b5200-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="b5200-126">Ini adalah masalah umum dan kami melihat potensi perbaikan untuk secara aktif mencabut setiap sesi setelah aktivasi kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="b5200-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="b5200-127">Jika delay berbeda dengan dua skenario ini, silakan buka tiket dukungan.</span><span class="sxs-lookup"><span data-stu-id="b5200-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
