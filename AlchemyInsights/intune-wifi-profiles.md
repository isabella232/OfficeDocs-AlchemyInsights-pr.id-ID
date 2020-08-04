---
title: Profil Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555312"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="37dc2-102">Profil Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="37dc2-103">Keberhasilan implementasi konektivitas Wi-Fi untuk klien MDM tergantung pada profil yang disebarkan dengan benar yang mencerminkan persyaratan infrastruktur Wi-Fi perusahaan.</span><span class="sxs-lookup"><span data-stu-id="37dc2-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="37dc2-104">Untuk meninjau pengaturan yang sesuai untuk platform klien yang sedang Anda selidiki, lihat:</span><span class="sxs-lookup"><span data-stu-id="37dc2-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="37dc2-105">Menambahkan pengaturan Wi-Fi untuk perangkat yang menjalankan Android di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="37dc2-106">Menambahkan setelan Wi-Fi untuk perangkat Android Enterprise khusus dan terkelola sepenuhnya di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="37dc2-107">Menambahkan pengaturan Wi-Fi untuk perangkat iOS dan iPadOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="37dc2-108">Menambahkan pengaturan Wi-Fi untuk Windows 10 dan perangkat yang lebih baru di Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="37dc2-109">Mengimpor setelan Wi-Fi untuk perangkat Windows di Intune</span><span class="sxs-lookup"><span data-stu-id="37dc2-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="37dc2-110">**Masalah umum**</span><span class="sxs-lookup"><span data-stu-id="37dc2-110">**Common Issues**</span></span>

<span data-ttu-id="37dc2-111">**Saya menerapkan profil Wi-Fi yang bergantung pada sertifikat yang disebarkan yang ditentukan di profil Wi-Fi. Namun, profil konfigurasi menunjukkan status galat.**</span><span class="sxs-lookup"><span data-stu-id="37dc2-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="37dc2-112">Periksa apakah perangkat Anda menerima sertifikat.</span><span class="sxs-lookup"><span data-stu-id="37dc2-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="37dc2-113">Di Intune, buka **semua perangkat** dan pilih perangkat > **konfigurasi perangkat**.</span><span class="sxs-lookup"><span data-stu-id="37dc2-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="37dc2-114">Periksa bahwa semua profil yang diharapkan terdaftar dan dalam keadaan yang berhasil.</span><span class="sxs-lookup"><span data-stu-id="37dc2-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="37dc2-115">Untuk profil Android, jika Anda memiliki sertifikat perantara dalam rantai sertifikat, pastikan mereka disebarkan ke perangkat Android.</span><span class="sxs-lookup"><span data-stu-id="37dc2-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="37dc2-116">Untuk memeriksa status sertifikat, pergi ke profil **konfigurasi perangkat**  >  **Profiles**  >  **Android menengah CA**  >  **properti**  >  **sertifikat terpercaya**.</span><span class="sxs-lookup"><span data-stu-id="37dc2-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="37dc2-117">Jika Anda terus melihat kesalahan, Tinjau prosedur dan bagian pemecahan masalah.</span><span class="sxs-lookup"><span data-stu-id="37dc2-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="37dc2-118">Untuk informasi lebih lanjut, lihat [Ikhtisar untuk pemecahan masalah profil sertifikat SCEP dengan Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="37dc2-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="37dc2-119">**Saya menerapkan profil Wi-Fi ke perangkat. Intune menunjukkan bahwa itu berhasil, tetapi perangkat tidak terhubung ke Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="37dc2-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="37dc2-120">Status berhasil berarti bahwa Intune telah berhasil menyebarkan profil sebagai dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="37dc2-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="37dc2-121">Namun, konfigurasi ini mungkin tidak cocok dengan persyaratan jaringan dan/atau autentikasi Anda.</span><span class="sxs-lookup"><span data-stu-id="37dc2-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="37dc2-122">Untuk rincian lebih lanjut tentang percobaan sambungan, periksa log di infrastruktur dan otentikasi Layanan (pada titik akses Wi-Fi controller dan NPS/radius server).</span><span class="sxs-lookup"><span data-stu-id="37dc2-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="37dc2-123">Anda mungkin harus bekerja sama dengan tim infrastruktur jaringan, atau vendor Wi-Fi pihak ketiga, untuk mengumpulkan dan meninjau log.</span><span class="sxs-lookup"><span data-stu-id="37dc2-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>