---
title: Menggunakan Microsoft Intune untuk mengelola akses web di Microsoft Edge untuk iOS dan Android
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
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678259"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="2d8e3-102">Menggunakan Microsoft Intune untuk mengelola akses web di Microsoft Edge untuk iOS dan Android</span><span class="sxs-lookup"><span data-stu-id="2d8e3-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="2d8e3-103">Microsoft Edge untuk iOS dan Android memungkinkan pengguna menelusuri web dari beberapa profil yang benar-benar terpisah.</span><span class="sxs-lookup"><span data-stu-id="2d8e3-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="2d8e3-104">Kemampuan perlindungan terluas untuk data Microsoft 365 akan tersedia saat Anda berlangganan ke rangkaian Enterprise Mobility + Security, yang menyertakan fitur Microsoft Intune dan Azure Active Directory Premium, seperti Access bersyarat.</span><span class="sxs-lookup"><span data-stu-id="2d8e3-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="2d8e3-105">Minimal, Anda akan ingin menyebarkan kebijakan akses bersyarat (1) memungkinkan pengguna menyambungkan dari perangkat seluler ke Microsoft Edge untuk iOS dan Android dan bahwa (2) menerapkan kebijakan perlindungan aplikasi Microsoft Intune yang menyediakan pengalaman penelusuran yang diproteksi.</span><span class="sxs-lookup"><span data-stu-id="2d8e3-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="2d8e3-106">Untuk memahami cara menggunakan akses dan kebijakan bersyarat, lihat:</span><span class="sxs-lookup"><span data-stu-id="2d8e3-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="2d8e3-107">Menerapkan kebijakan akses bersyarat direktori aktif Azure</span><span class="sxs-lookup"><span data-stu-id="2d8e3-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="2d8e3-108">Membuat kebijakan perlindungan aplikasi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d8e3-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="2d8e3-109">Menggunakan masuk tunggal untuk Azure Active Directory – aplikasi web yang tersambung dalam browser yang diproteksi kebijakan</span><span class="sxs-lookup"><span data-stu-id="2d8e3-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="2d8e3-110">Menggunakan konfigurasi aplikasi untuk mengelola pengalaman penelusuran</span><span class="sxs-lookup"><span data-stu-id="2d8e3-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="2d8e3-111">Memperbolehkan penggunaan akun kantor dan sekolah saja</span><span class="sxs-lookup"><span data-stu-id="2d8e3-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="2d8e3-112">Menyebarkan kebijakan konfigurasi aplikasi Umum</span><span class="sxs-lookup"><span data-stu-id="2d8e3-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="2d8e3-113">Menerapkan kebijakan konfigurasi aplikasi untuk proteksi data</span><span class="sxs-lookup"><span data-stu-id="2d8e3-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="2d8e3-114">Menggunakan Microsoft Endpoint Manager untuk menyebarkan kebijakan konfigurasi aplikasi</span><span class="sxs-lookup"><span data-stu-id="2d8e3-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="2d8e3-115">Untuk mempelajari cara mengakses log aplikasi terkelola, lihat [menggunakan Microsoft Edge untuk IOS dan Android untuk mengakses log aplikasi terkelola](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="2d8e3-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
