---
title: Akses langganan
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807435"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="75962-102">Tidak dapat masuk ke Azure karena masalah browser (Hang browser, tetap berputar, tidak dimuat, dsb.)</span><span class="sxs-lookup"><span data-stu-id="75962-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="75962-103">Anda mungkin terpengaruh oleh gangguan.</span><span class="sxs-lookup"><span data-stu-id="75962-103">You might be impacted by an outage.</span></span> <span data-ttu-id="75962-104">Silakan periksa untuk melihat apakah ada pemutusan yang sedang berlangsung: [status kesehatan Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="75962-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="75962-105">Keluar dari semua sesi Azure aktif.</span><span class="sxs-lookup"><span data-stu-id="75962-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="75962-106">Mulai mode privat atau penyamaran di browser web Anda.</span><span class="sxs-lookup"><span data-stu-id="75962-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="75962-107">Anda juga dapat mencoba untuk me-refresh browser, menggunakan browser lain, menghapus cookie tembolok jika di atas tidak berfungsi.</span><span class="sxs-lookup"><span data-stu-id="75962-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="75962-108">Pelajari selengkapnya: [memecahkan masalah saat masuk](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="75962-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="75962-109">**Tidak dapat mengakses metode berlangganan**</span><span class="sxs-lookup"><span data-stu-id="75962-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="75962-110">Di [portal Azure](https://portal.azure.com/), pastikan bahwa direktori Azure yang benar telah dipilih dari akun di bagian kanan atas.</span><span class="sxs-lookup"><span data-stu-id="75962-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="75962-111">Di [pusat akun Azure](https://account.windowsazure.com/Subscriptions), pastikan jika akun yang digunakan adalah admin akun.</span><span class="sxs-lookup"><span data-stu-id="75962-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="75962-112">Pelajari selengkapnya: [memecahkan masalah langganan tidak ditemukan](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="75962-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="75962-113">**Tidak dapat mengakses Riwayat tagihan**</span><span class="sxs-lookup"><span data-stu-id="75962-113">**Unable to access billing history**</span></span>

<span data-ttu-id="75962-114">Admin akun harus memastikan pengguna yang mengakses informasi tagihan ditambahkan di direktori Azure Active sebagai pengguna tamu: [menambahkan atau menghapus pengguna baru](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="75962-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="75962-115">Pengguna tersebut harus diberi peran admin global: [menetapkan peran kepada pengguna](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="75962-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="75962-116">Posting ini, pengguna bisa diberi akses tagihan menggunakan kebijakan RBAC: [memberi akses ke tagihan](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="75962-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="75962-117">**Dokumen yang direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="75962-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="75962-118">Saya tidak dapat masuk untuk mengelola langganan Azure saya</span><span class="sxs-lookup"><span data-stu-id="75962-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)