---
title: Pemecahan masalah penyebaran sertifikat autentikasi klien
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658989"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="c1ef8-102">Pemecahan masalah penyebaran sertifikat autentikasi klien</span><span class="sxs-lookup"><span data-stu-id="c1ef8-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="c1ef8-103">Intune NDES/SCEP dan PKCS/PFX profil sertifikat klien biasanya digunakan bersama dengan tipe profil lain seperti WiFi, VPN, dan email untuk memperbolehkan pengguna mengautentikasi sumber daya perusahaan.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="c1ef8-104">Ketika tipe profil tersebut ditautkan ke profil sertifikat klien sangat tergantung pada keberhasilan penyebaran profil tersebut.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="c1ef8-105">Penyetelan infrastruktur awal dan konfigurasi profil sertifikat klien sering kali memerlukan pemecahan masalah.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="c1ef8-106">Untuk panduan langkah demi langkah untuk penyiapan yang berhasil dari konektor NDES dan panduan pemecahan masalah untuk mengisolasi masalah dengan penyebaran sertifikat, lihat:</span><span class="sxs-lookup"><span data-stu-id="c1ef8-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="c1ef8-107">Mengonfigurasi infrastruktur untuk mendukung SCEP dengan Intune</span><span class="sxs-lookup"><span data-stu-id="c1ef8-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="c1ef8-108">Gambaran umum untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c1ef8-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="c1ef8-109">Gunakan skrip PowerShell yang direferensikan untuk membantu memverifikasi konfigurasi Anda.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="c1ef8-110">Untuk informasi selengkapnya, lihat [skrip verifikasi konektor sertifikat Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="c1ef8-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="c1ef8-111">**Masalah umum lainnya**</span><span class="sxs-lookup"><span data-stu-id="c1ef8-111">**Other common issues**</span></span>

<span data-ttu-id="c1ef8-112">**Ketika saya mencoba untuk menginstal konektor sertifikat Intune di server konektor NDES, saya mendapatkan pesan, "kata sandi dalam permintaan Sertifikat tidak dapat diverifikasi. Mungkin telah digunakan sudah. Dapatkan kata sandi baru untuk dikirim dengan permintaan ini. "**</span><span class="sxs-lookup"><span data-stu-id="c1ef8-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="c1ef8-113">Pesan ini berarti Anda harus menjalankan instalasi konektor sertifikat sebagai administrator.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="c1ef8-114">Di beberapa lingkungan, server tempat sertifikat Intune berjalan harus menggunakan server proksi untuk menyambungkan ke Intune, dan konektor sertifikat harus menggunakan proksi.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="c1ef8-115">Dalam beberapa situasi, konektor NDES mengabaikan pengaturan proksi yang dikonfigurasi, dan mungkin perlu mengonfigurasi pengaturan proksi saat berjalan dalam konteks keamanan LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="c1ef8-116">Solusinya adalah dengan menjalankan Internet Explorer sebagai sistem dan mengonfigurasi proksi di IE.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="c1ef8-117">Setelah memulai ulang layanan konektor Intune, konektor NDES tersambung ke Intune.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="c1ef8-118">**Perangkat pengguna tidak lagi menerima sertifikat SCEP dari NDE.**</span><span class="sxs-lookup"><span data-stu-id="c1ef8-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="c1ef8-119">Dimungkinkan bahwa sertifikat autentikasi klien yang dikeluarkan untuk server NDE, dan ditentukan selama instalasi konektor NDES, telah kedaluwarsa atau hilang.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="c1ef8-120">Untuk mengatasi masalah:</span><span class="sxs-lookup"><span data-stu-id="c1ef8-120">To resolve:</span></span> 
 
1. <span data-ttu-id="c1ef8-121">Hapus instalasi konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="c1ef8-122">Gunakan detail ini untuk meminta autentikasi klien baru atau sertifikat autentikasi server:</span><span class="sxs-lookup"><span data-stu-id="c1ef8-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="c1ef8-123">Nama subjek: CN = eksternal FQDN</span><span class="sxs-lookup"><span data-stu-id="c1ef8-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="c1ef8-124">Nama Alternatif subjek (keduanya diperlukan): DNS = FQDN eksternal, DNS = FQDN internal</span><span class="sxs-lookup"><span data-stu-id="c1ef8-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="c1ef8-125">Instal ulang konektor NDES dengan sertifikat baru.</span><span class="sxs-lookup"><span data-stu-id="c1ef8-125">Reinstall the NDES connector with the new certificate.</span></span>