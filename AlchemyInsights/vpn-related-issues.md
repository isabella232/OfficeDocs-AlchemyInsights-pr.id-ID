---
title: Masalah terkait VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555235"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="51b01-102">Masalah terkait VPN</span><span class="sxs-lookup"><span data-stu-id="51b01-102">VPN related issues</span></span>

<span data-ttu-id="51b01-103">Keberhasilan pelaksanaan konektivitas VPN untuk MDM klien tergantung pada profil disebarkan yang benar mencerminkan persyaratan infrastruktur VPN.</span><span class="sxs-lookup"><span data-stu-id="51b01-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="51b01-104">Untuk pengaturan yang sesuai untuk platform klien yang sedang Anda selidiki, lihat:</span><span class="sxs-lookup"><span data-stu-id="51b01-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="51b01-105">Windows 10 dan Windows Holographic pengaturan perangkat untuk menambahkan sambungan VPN menggunakan Intune</span><span class="sxs-lookup"><span data-stu-id="51b01-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="51b01-106">Menambahkan pengaturan VPN pada perangkat iOS dan iPadOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="51b01-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="51b01-107">Pengaturan perangkat Android untuk mengkonfigurasi VPN di Intune</span><span class="sxs-lookup"><span data-stu-id="51b01-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="51b01-108">Menambahkan pengaturan VPN pada perangkat macOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="51b01-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="51b01-109">Jika profil VPN Anda menggunakan otentikasi berbasis sertifikat, pastikan bahwa sertifikat akar dan klien otentikasi sertifikat profil tertaut ke profil VPN disebarkan berhasil.</span><span class="sxs-lookup"><span data-stu-id="51b01-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="51b01-110">**Masalah umum**</span><span class="sxs-lookup"><span data-stu-id="51b01-110">**Common Issues**</span></span>

<span data-ttu-id="51b01-111">**Saya menerapkan profil VPN ke perangkat. Intune menunjukkan bahwa itu berhasil, tetapi perangkat tidak terhubung ke VPN.**</span><span class="sxs-lookup"><span data-stu-id="51b01-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="51b01-112">Status berhasil berarti bahwa Intune telah berhasil menyebarkan profil sebagai dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="51b01-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="51b01-113">Namun, konfigurasi ini mungkin tidak cocok dengan persyaratan jaringan dan/atau autentikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="51b01-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="51b01-114">Tinjau log dalam infrastruktur dan otentikasi Layanan (di VPN server dan NPS/radius server) untuk rincian lebih lanjut tentang percobaan sambungan.</span><span class="sxs-lookup"><span data-stu-id="51b01-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="51b01-115">Anda mungkin harus bekerja sama dengan tim infrastruktur jaringan, atau vendor VPN pihak ketiga, untuk mengumpulkan dan meninjau log.</span><span class="sxs-lookup"><span data-stu-id="51b01-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="51b01-116">**Saat saya mengonfigurasi VPN khusus untuk iOS, fitur VPN per aplikasi tidak tersedia.**</span><span class="sxs-lookup"><span data-stu-id="51b01-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="51b01-117">VPN per aplikasi untuk perangkat iOS di Intune saat ini tersedia untuk daftar penyedia dan mitra tertentu, yang juga harus memenuhi prasyarat sertifikat sebelum mengonfigurasi VPN per aplikasi.</span><span class="sxs-lookup"><span data-stu-id="51b01-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="51b01-118">Untuk informasi lebih lanjut, lihat [mengatur per aplikasi Virtual Private Network (VPN) untuk IOS/iPadOS perangkat di Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="51b01-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="51b01-119">Untuk informasi lebih lanjut tentang semua jenis sambungan VPN di Intune, lihat [membuat profil vpn untuk menyambung ke server VPN di Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="51b01-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="51b01-120">**VPN on-demand iOS tidak memicu ketika domain yang dikonfigurasi diakses**</span><span class="sxs-lookup"><span data-stu-id="51b01-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="51b01-121">Untuk menguji pengaturan VPN otomatis, tetapkan nilai berikut:</span><span class="sxs-lookup"><span data-stu-id="51b01-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="51b01-122">Saya ingin melakukan hal berikut: **mengevaluasi setiap upaya koneksi**</span><span class="sxs-lookup"><span data-stu-id="51b01-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="51b01-123">Memilih apakah akan menghubungkan: **Hubungkan jika diperlukan**</span><span class="sxs-lookup"><span data-stu-id="51b01-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="51b01-124">Ketika pengguna mengakses domain ini: **target** *nama domain*</span><span class="sxs-lookup"><span data-stu-id="51b01-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="51b01-125">Jika konfigurasi di atas tidak berhasil, tambahkan elemen berikut:</span><span class="sxs-lookup"><span data-stu-id="51b01-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="51b01-126">Ketika URL ini tidak terjangkau, memaksa menghubungkan VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="51b01-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>