---
title: Perangkat dalam status tertunda
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678483"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="4e225-102">Perangkat dalam status tertunda</span><span class="sxs-lookup"><span data-stu-id="4e225-102">Device in pending state</span></span>

<span data-ttu-id="4e225-103">**Tuntutan**</span><span class="sxs-lookup"><span data-stu-id="4e225-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="4e225-104">Jika Anda menyetel pendaftaran perangkat untuk pertama kalinya, pastikan bahwa Anda telah meninjau [pengenalan ke manajemen perangkat di Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) yang akan memandu Anda tentang cara mendapatkan perangkat di bawah kontrol Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4e225-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="4e225-105">Jika Anda mendaftarkan perangkat ke Azure AD secara langsung dan mendaftarkan mereka ke dalam Intune, Anda perlu memastikan bahwa Anda telah [mengonfigurasi Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) dan meminta [lisensi](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tersebut terlebih dahulu.</span><span class="sxs-lookup"><span data-stu-id="4e225-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="4e225-106">Pastikan Anda memiliki wewenang untuk melakukan operasi di Azure AD dan AD di tempat.</span><span class="sxs-lookup"><span data-stu-id="4e225-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="4e225-107">Hanya administrator global di Azure AD yang dapat mengelola pengaturan untuk pendaftaran perangkat.</span><span class="sxs-lookup"><span data-stu-id="4e225-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="4e225-108">Selain itu, jika Anda menyetel pendaftaran otomatis di direktori aktif di tempat, Anda harus menjadi administrator direktori aktif dan AD FS (jika ada).</span><span class="sxs-lookup"><span data-stu-id="4e225-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="4e225-109">Proses registrasi gabungan Azure AD Pendaftaran memerlukan perangkat untuk berada di jaringan perusahaan.</span><span class="sxs-lookup"><span data-stu-id="4e225-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="4e225-110">Ini juga berfungsi melalui VPN namun ada beberapa hal yang perlu diperhatikan.</span><span class="sxs-lookup"><span data-stu-id="4e225-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="4e225-111">Kami telah mendengar Pelanggan yang memerlukan bantuan dengan pemecahan masalah hibrid Azure AD bergabung dalam proses pendaftaran di bawah kondisi kerja jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="4e225-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="4e225-112">**Lingkungan autentikasi awan (menggunakan sinkronisasi hash kata sandi Azure atau autentikasi kirim langsung)**</span><span class="sxs-lookup"><span data-stu-id="4e225-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="4e225-113">Alur pendaftaran ini juga dikenal sebagai "gabungan sinkronisasi".</span><span class="sxs-lookup"><span data-stu-id="4e225-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="4e225-114">Berikut ini adalah rincian apa yang terjadi selama proses pendaftaran:</span><span class="sxs-lookup"><span data-stu-id="4e225-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="4e225-115">Windows 10 menemukan catatan koneksi Layanan (SCP) ketika pengguna masuk ke perangkat.</span><span class="sxs-lookup"><span data-stu-id="4e225-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="4e225-116">Perangkat tersebut pertama kali mencoba untuk mengambil informasi penyewa dari SCP sisi klien dalam registri [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="4e225-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="4e225-117">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="4e225-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="4e225-118">Jika gagal, perangkat berkomunikasi dengan direktori aktif di tempat untuk mendapatkan informasi penyewa dari SCP.</span><span class="sxs-lookup"><span data-stu-id="4e225-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="4e225-119">Untuk memverifikasi SCP, rujuk [dokumen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)ini.</span><span class="sxs-lookup"><span data-stu-id="4e225-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="4e225-120">Kami merekomendasikan untuk mengaktifkan SCP di direktori aktif dan hanya menggunakan SCP sisi klien untuk validasi awal.</span><span class="sxs-lookup"><span data-stu-id="4e225-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="4e225-121">Windows 10 mencoba untuk berkomunikasi dengan Azure AD di bawah konteks sistem untuk mengautentikasi dirinya.</span><span class="sxs-lookup"><span data-stu-id="4e225-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="4e225-122">Anda dapat memverifikasi apakah perangkat dapat mengakses sumber daya Microsoft di bawah akun sistem dengan menggunakan [skrip konektivitas registrasi perangkat uji](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="4e225-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="4e225-123">Windows 10 menghasilkan sertifikat yang ditandatangani sendiri dan menyimpannya di bawah objek komputer di direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="4e225-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="4e225-124">Ini memerlukan garis pandang ke pengontrol domain.</span><span class="sxs-lookup"><span data-stu-id="4e225-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="4e225-125">Objek perangkat yang memiliki sertifikat disinkronkan ke Azure AD melalui Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4e225-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="4e225-126">Siklus sinkronisasi adalah setiap 30 menit secara default, namun tergantung pada konfigurasi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4e225-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="4e225-127">Untuk informasi selengkapnya, lihat [dokumen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)ini.</span><span class="sxs-lookup"><span data-stu-id="4e225-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="4e225-128">Pada tahap ini, Anda akan bisa melihat perangkat subjek dalam status "**tertunda**" di bawah bilah perangkat Azure portal.</span><span class="sxs-lookup"><span data-stu-id="4e225-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="4e225-129">Di pengguna berikutnya masuk ke Windows 10, pendaftaran akan diselesaikan.</span><span class="sxs-lookup"><span data-stu-id="4e225-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4e225-130">Jika Anda berada di VPN dan logoff/login mengakhiri konektivitas domain, Anda bisa memicu pendaftaran secara manual.</span><span class="sxs-lookup"><span data-stu-id="4e225-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="4e225-131">Untuk melakukan itu:</span><span class="sxs-lookup"><span data-stu-id="4e225-131">To do that:</span></span>
    >
    > <span data-ttu-id="4e225-132">Masalah `dsregcmd /join` secara lokal pada prompt admin atau jarak jauh melalui PSExec ke PC Anda.</span><span class="sxs-lookup"><span data-stu-id="4e225-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="4e225-133">Misalnya: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="4e225-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="4e225-134">Untuk masalah umum dengan pendaftaran perangkat Azure Active Directory, lihat [FAQ perangkat](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="4e225-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
