---
title: Pemecahan masalah penyebaran sertifikat otentikasi klien
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555307"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="f1819-102">Pemecahan masalah penyebaran sertifikat otentikasi klien</span><span class="sxs-lookup"><span data-stu-id="f1819-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="f1819-103">Intune NDES/SCEP dan PKCS/PFX klien sertifikat profil yang umum digunakan bersama dengan jenis profil lain seperti WiFi, VPN, dan email untuk memungkinkan pengguna untuk mengotentikasi ke sumber daya perusahaan.</span><span class="sxs-lookup"><span data-stu-id="f1819-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="f1819-104">Ketika jenis profil tersebut tertaut ke profil sertifikat klien tergantung pada penyebaran berhasil profil tersebut.</span><span class="sxs-lookup"><span data-stu-id="f1819-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="f1819-105">Penataan infrastruktur awal dan konfigurasi terkait profil sertifikat klien sering memerlukan pemecahan masalah.</span><span class="sxs-lookup"><span data-stu-id="f1819-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="f1819-106">Untuk panduan selangkah demi selangkah untuk berhasil penataan konektor NDES dan panduan pemecahan masalah untuk mengisolasi masalah dengan penyebaran sertifikat, lihat:</span><span class="sxs-lookup"><span data-stu-id="f1819-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="f1819-107">Mengkonfigurasi infrastruktur untuk mendukung SCEP dengan Intune</span><span class="sxs-lookup"><span data-stu-id="f1819-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="f1819-108">Ikhtisar untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f1819-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="f1819-109">Gunakan skrip PowerShell yang direferensikan untuk membantu memverifikasi konfigurasi Anda.</span><span class="sxs-lookup"><span data-stu-id="f1819-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="f1819-110">Untuk informasi lebih lanjut, lihat [Intune sertifikat konektor verifikasi skrip](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="f1819-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="f1819-111">**Masalah umum lainnya**</span><span class="sxs-lookup"><span data-stu-id="f1819-111">**Other common issues**</span></span>

<span data-ttu-id="f1819-112">**Ketika saya mencoba untuk menginstal konektor sertifikat Intune di server konektor NDES, saya mendapatkan pesan, "sandi di sertifikat permintaan tidak dapat diverifikasi. Ini mungkin telah digunakan sudah. Dapatkan kata sandi baru untuk dikirimkan dengan permintaan ini. "**</span><span class="sxs-lookup"><span data-stu-id="f1819-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="f1819-113">Pesan ini berarti bahwa Anda harus menjalankan penginstalan konektor sertifikat sebagai administrator.</span><span class="sxs-lookup"><span data-stu-id="f1819-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="f1819-114">Di beberapa lingkungan, server di mana Intune sertifikat berjalan harus menggunakan server proksi untuk menyambung ke Intune, dan konektor sertifikat harus menggunakan proksi.</span><span class="sxs-lookup"><span data-stu-id="f1819-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="f1819-115">Dalam beberapa keadaan, konektor NDES mengabaikan pengaturan proksi dikonfigurasi, dan mungkin perlu untuk mengkonfigurasi pengaturan proxy saat berjalan dalam konteks keamanan LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="f1819-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="f1819-116">Solusinya adalah dengan menjalankan Internet Explorer sebagai sistem dan mengkonfigurasi proxy di IE.</span><span class="sxs-lookup"><span data-stu-id="f1819-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="f1819-117">Setelah restart layanan konektor Intune, konektor NDES menyambung ke Intune.</span><span class="sxs-lookup"><span data-stu-id="f1819-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="f1819-118">**Perangkat pengguna tidak lagi menerima SCEP sertifikat dari NDES.**</span><span class="sxs-lookup"><span data-stu-id="f1819-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="f1819-119">Dimungkinkan bahwa sertifikat otentikasi klien yang dikeluarkan untuk NDES server, dan ditentukan selama penginstalan konektor NDES, telah kedaluwarsa atau hilang.</span><span class="sxs-lookup"><span data-stu-id="f1819-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="f1819-120">Untuk menyelesaikan:</span><span class="sxs-lookup"><span data-stu-id="f1819-120">To resolve:</span></span> 
 
1. <span data-ttu-id="f1819-121">Membongkar konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="f1819-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="f1819-122">Gunakan rincian ini untuk meminta otentikasi klien baru atau sertifikat otentikasi server:</span><span class="sxs-lookup"><span data-stu-id="f1819-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="f1819-123">Nama subjek: CN = FQDN eksternal</span><span class="sxs-lookup"><span data-stu-id="f1819-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="f1819-124">Nama Alternatif subjek (keduanya diperlukan): DNS = eksternal FQDN, DNS = internal FQDN</span><span class="sxs-lookup"><span data-stu-id="f1819-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="f1819-125">Instal ulang konektor NDES dengan sertifikat baru.</span><span class="sxs-lookup"><span data-stu-id="f1819-125">Reinstall the NDES connector with the new certificate.</span></span>