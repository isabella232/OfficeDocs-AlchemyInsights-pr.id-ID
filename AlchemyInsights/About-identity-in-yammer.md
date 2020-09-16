---
title: Tentang identitas di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664173"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="c2aa0-102">Tentang identitas di Yammer</span><span class="sxs-lookup"><span data-stu-id="c2aa0-102">About identity in Yammer</span></span>

<span data-ttu-id="c2aa0-103">Disarankan agar semua jaringan melakukan langkah-langkah berikut untuk menghindari masalah terkait identitas:</span><span class="sxs-lookup"><span data-stu-id="c2aa0-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="c2aa0-104">Terapkan identitas 365 Office setelah menetapkan akun Microsoft 365 untuk pengguna di Azure AD guna memastikan bahwa semua pengguna masuk menggunakan akun 365 Microsoft utama Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="c2aa0-105">Untuk informasi selengkapnya, lihat [memaksakan identitas Office 365 untuk pengguna Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="c2aa0-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="c2aa0-106">Menggabungkan beberapa jaringan Yammer.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="c2aa0-107">Warisan konfigurasi Yammer mengizinkan beberapa jaringan Yammer untuk tersambung ke satu penyewa.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="c2aa0-108">Untuk informasi selengkapnya, lihat [migrasi jaringan-menggabungkan beberapa jaringan Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="c2aa0-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="c2aa0-109">Secara opsional, Terapkan lisensi untuk Yammer untuk memblokir pengguna dari Yammer jika mereka tidak memiliki lisensi.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="c2aa0-110">Untuk informasi selengkapnya, lihat [mengelola lisensi pengguna Yammer di Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c2aa0-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="c2aa0-111">Terakhir, audit daftar pengguna untuk jaringan Yammer yang lebih lama dan tangguhkan pengguna pewaris.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="c2aa0-112">Disarankan agar Anda menangguhkan (menonaktifkan) pengguna dan bukan menghapusnya, karena penghapusan tidak dapat dibatalkan.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="c2aa0-113">Untuk informasi selengkapnya, lihat [mengaudit pengguna Yammer di jaringan yang tersambung ke Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) dan [menghapus pengguna](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="c2aa0-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="c2aa0-114">Dengan mengonfigurasi Yammer menggunakan langkah-langkah ini, Anda juga akan siap mengonfigurasi jaringan Yammer Anda untuk mode asli untuk Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c2aa0-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="c2aa0-115">Untuk informasi selengkapnya, lihat [mengonfigurasi jaringan Yammer Anda untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="c2aa0-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>