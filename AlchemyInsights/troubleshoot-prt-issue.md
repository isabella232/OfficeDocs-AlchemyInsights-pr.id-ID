---
title: Memecahkan masalah PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573718"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="53a96-102">Memecahkan masalah PRT</span><span class="sxs-lookup"><span data-stu-id="53a96-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="53a96-103">Untuk perangkat apa pun yang diselesaikan dengan benar, harus terdaftar dan di negara bagian yang baik dan dapat memperoleh token refresh utama (PRT).</span><span class="sxs-lookup"><span data-stu-id="53a96-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="53a96-104">Proses registrasi gabungan Azure AD Pendaftaran memerlukan perangkat untuk berada di jaringan perusahaan.</span><span class="sxs-lookup"><span data-stu-id="53a96-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="53a96-105">Ini juga berfungsi melalui VPN namun ada beberapa hal yang perlu diperhatikan.</span><span class="sxs-lookup"><span data-stu-id="53a96-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="53a96-106">Kami telah mendengar Pelanggan yang memerlukan bantuan dengan pemecahan masalah hibrid proses pendaftaran gabungan Azure AD di bawah kondisi kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="53a96-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="53a96-107">Berikut ini adalah rincian apa yang terjadi ' di bawah kap ' selama proses registrasi.</span><span class="sxs-lookup"><span data-stu-id="53a96-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="53a96-108">**Lingkungan autentikasi awan (menggunakan sinkronisasi hash kata sandi Azure atau autentikasi kirim langsung)**</span><span class="sxs-lookup"><span data-stu-id="53a96-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="53a96-109">Alur pendaftaran ini juga dikenal sebagai "gabungan sinkronisasi".</span><span class="sxs-lookup"><span data-stu-id="53a96-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="53a96-110">Windows 10 menemukan catatan SCP saat pengguna masuk ke perangkat.</span><span class="sxs-lookup"><span data-stu-id="53a96-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="53a96-111">Perangkat tersebut pertama kali mencoba untuk mengambil informasi penyewa dari SCP sisi klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="53a96-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="53a96-112">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)ini.</span><span class="sxs-lookup"><span data-stu-id="53a96-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="53a96-113">Jika gagal, perangkat berkomunikasi dengan Active Directory lokal (AD) untuk mendapatkan informasi penyewa dari titik koneksi Layanan (SCP).</span><span class="sxs-lookup"><span data-stu-id="53a96-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="53a96-114">Untuk memverifikasi SCP, silakan lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)ini.</span><span class="sxs-lookup"><span data-stu-id="53a96-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="53a96-115">Kami merekomendasikan untuk mengaktifkan SCP dalam iklan dan hanya menggunakan SCP sisi klien untuk validasi awal.</span><span class="sxs-lookup"><span data-stu-id="53a96-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="53a96-116">Windows 10 mencoba untuk berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya.</span><span class="sxs-lookup"><span data-stu-id="53a96-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="53a96-117">Anda dapat memverifikasi apakah perangkat dapat mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan skrip konektivitas registrasi perangkat uji.</span><span class="sxs-lookup"><span data-stu-id="53a96-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="53a96-118">Windows 10 menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di AD di tempat.</span><span class="sxs-lookup"><span data-stu-id="53a96-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="53a96-119">Ini memerlukan garis pandang ke pengontrol domain.</span><span class="sxs-lookup"><span data-stu-id="53a96-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="53a96-120">Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="53a96-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="53a96-121">Siklus sinkronisasi adalah setiap 30 menit secara default, namun tergantung pada konfigurasi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="53a96-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="53a96-122">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)ini.</span><span class="sxs-lookup"><span data-stu-id="53a96-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="53a96-123">Pada tahap ini, Anda akan bisa melihat perangkat subjek dalam status "tertunda" di bawah bilah perangkat Azure portal.</span><span class="sxs-lookup"><span data-stu-id="53a96-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="53a96-124">Di pengguna berikutnya masuk ke Windows 10, pendaftaran akan diselesaikan.</span><span class="sxs-lookup"><span data-stu-id="53a96-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="53a96-125">Jika Anda menggunakan VPN dan logoff-proses masuk mengakhiri konektivitas domain, Anda bisa memicu pendaftaran secara manual:</span><span class="sxs-lookup"><span data-stu-id="53a96-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="53a96-126">Menerbitkan dsregcmd/Join secara lokal pada prompt admin atau jarak jauh melalui PSExec ke PC Anda.</span><span class="sxs-lookup"><span data-stu-id="53a96-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="53a96-127">Sebagai contoh, PsExec-s \\ win10client01 CMD, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="53a96-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="53a96-128">Untuk detail selengkapnya tentang masalah gabungan hibrid, lihat [memecahkan masalah perangkat](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="53a96-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
