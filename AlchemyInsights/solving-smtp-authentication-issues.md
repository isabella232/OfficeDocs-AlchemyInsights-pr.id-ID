---
title: Mengaktifkan autentikasi SMTP dan pemecahan masalah
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077654"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="b4958-102">Mengaktifkan autentikasi SMTP dan pemecahan masalah</span><span class="sxs-lookup"><span data-stu-id="b4958-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="b4958-103">Jika ingin mengaktifkan autentikasi SMTP untuk kotak surat atau mendapatkan kesalahan "Client not authenticated", "Authentication unsuccessful", atau "SmtpClientAuthentication" dengan kode 5.7.57 atau 5.7.3 atau 5.7.139 ketika mencoba melakukan relai email dengan mengautentikasi perangkat atau aplikasi dengan Microsoft 365, lakukan tiga tindakan ini untuk mengatasi masalah tersebut:</span><span class="sxs-lookup"><span data-stu-id="b4958-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="b4958-104">Nonaktifkan [default keamanan Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) dengan mengaktifkan keamanan default **ke** **Tidak.**</span><span class="sxs-lookup"><span data-stu-id="b4958-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="b4958-105">a.</span><span class="sxs-lookup"><span data-stu-id="b4958-105">a.</span></span> <span data-ttu-id="b4958-106">Masuk ke portal Azure sebagai administrator Keamanan, administrator Akses Kondisional, atau administrator global.</span><span class="sxs-lookup"><span data-stu-id="b4958-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="b4958-107">b.</span><span class="sxs-lookup"><span data-stu-id="b4958-107">b.</span></span> <span data-ttu-id="b4958-108">Telusuri ke Azure Active Directory > **Properti.**</span><span class="sxs-lookup"><span data-stu-id="b4958-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="b4958-109">c.</span><span class="sxs-lookup"><span data-stu-id="b4958-109">c.</span></span> <span data-ttu-id="b4958-110">Pilih **Kelola default keamanan.**</span><span class="sxs-lookup"><span data-stu-id="b4958-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="b4958-111">d.</span><span class="sxs-lookup"><span data-stu-id="b4958-111">d.</span></span> <span data-ttu-id="b4958-112">Atur **Aktifkan default keamanan ke** **Tidak.**</span><span class="sxs-lookup"><span data-stu-id="b4958-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="b4958-113">e.</span><span class="sxs-lookup"><span data-stu-id="b4958-113">e.</span></span> <span data-ttu-id="b4958-114">Pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="b4958-114">Select **Save**.</span></span>

2. <span data-ttu-id="b4958-115">[Mengaktifkan pengiriman SMTP Klien](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) pada kotak surat berlisensi.</span><span class="sxs-lookup"><span data-stu-id="b4958-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="b4958-116">a.</span><span class="sxs-lookup"><span data-stu-id="b4958-116">a.</span></span> <span data-ttu-id="b4958-117">Dari pusat admin Microsoft 365, masuk ke **Pengguna Aktif**, lalu pilih pengguna.</span><span class="sxs-lookup"><span data-stu-id="b4958-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="b4958-118">b.</span><span class="sxs-lookup"><span data-stu-id="b4958-118">b.</span></span> <span data-ttu-id="b4958-119">Masuk ke tab Email, dan di **bawah Aplikasi email**, pilih Kelola aplikasi **email**.</span><span class="sxs-lookup"><span data-stu-id="b4958-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="b4958-120">d.</span><span class="sxs-lookup"><span data-stu-id="b4958-120">d.</span></span> <span data-ttu-id="b4958-121">Pastikan SMTP **Terautentikasi** dicentang (diaktifkan).</span><span class="sxs-lookup"><span data-stu-id="b4958-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="b4958-122">e.</span><span class="sxs-lookup"><span data-stu-id="b4958-122">e.</span></span> <span data-ttu-id="b4958-123">Pilih **Simpan perubahan.**</span><span class="sxs-lookup"><span data-stu-id="b4958-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="b4958-124">[Menonaktifkan Multi-Factor Authentication (MFA) pada](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) kotak surat berlisensi.</span><span class="sxs-lookup"><span data-stu-id="b4958-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="b4958-125">a.</span><span class="sxs-lookup"><span data-stu-id="b4958-125">a.</span></span> <span data-ttu-id="b4958-126">Masuk ke pusat admin Microsoft 365, dan di menu navigasi kiri, pilih **Pengguna**  >  **Aktif pengguna**.</span><span class="sxs-lookup"><span data-stu-id="b4958-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="b4958-127">b.</span><span class="sxs-lookup"><span data-stu-id="b4958-127">b.</span></span> <span data-ttu-id="b4958-128">Pilih **Multi-factor authentication**.</span><span class="sxs-lookup"><span data-stu-id="b4958-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="b4958-129">c.</span><span class="sxs-lookup"><span data-stu-id="b4958-129">c.</span></span> <span data-ttu-id="b4958-130">Pilih pengguna dan nonaktifkan **Multi-Factor auth**.</span><span class="sxs-lookup"><span data-stu-id="b4958-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
