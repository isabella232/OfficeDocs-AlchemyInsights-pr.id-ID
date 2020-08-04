---
title: Menggunakan profil email dengan Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555253"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="de441-102">Menggunakan profil email dengan Intune</span><span class="sxs-lookup"><span data-stu-id="de441-102">Using email profiles with Intune</span></span>

<span data-ttu-id="de441-103">Intune dapat digunakan untuk membuat dan menyebarkan profil email untuk klien email Native (built-in) pada beberapa platform perangkat.</span><span class="sxs-lookup"><span data-stu-id="de441-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="de441-104">Untuk informasi tentang beberapa pembatasan yang terkait dengan profil email, termasuk bagaimana keberadaan profil yang ada ditangani dan cara menghapus profil email, lihat [menambahkan pengaturan email ke perangkat menggunakan Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="de441-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="de441-105">Untuk informasi lebih lanjut tentang cara membuat profil email untuk setiap platform perangkat, lihat:</span><span class="sxs-lookup"><span data-stu-id="de441-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="de441-106">Pengaturan perangkat Android untuk mengkonfigurasi email, otentikasi, dan sinkronisasi di Intune</span><span class="sxs-lookup"><span data-stu-id="de441-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="de441-107">Menambahkan pengaturan e-mail untuk perangkat iOS dan iPadOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="de441-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="de441-108">Tataan profil email di Microsoft Intune untuk perangkat yang menjalankan Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="de441-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="de441-109">Pengaturan profil email untuk perangkat yang menjalankan Windows 10 di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="de441-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="de441-110">**Masalah sinkronisasi Umum**</span><span class="sxs-lookup"><span data-stu-id="de441-110">**Common syncing issue**</span></span>

<span data-ttu-id="de441-111">**Sebuah KNOX pada profil email Android mencegah pengguna kontak, kalender, dan tugas, dari yang akan disinkronkan ke perangkat pengguna.**</span><span class="sxs-lookup"><span data-stu-id="de441-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="de441-112">The KNOX di profil email Android KNOX menawarkan admin pilihan untuk memutuskan jenis konten yang akan disinkronkan ke perangkat dengan menetapkan masing-masing untuk diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="de441-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="de441-113">Jika setelan untuk jenis konten apa pun diatur ke **tidak dikonfigurasi** (default), jenis konten tersebut tidak disinkronkan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="de441-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="de441-114">Pengguna dapat mengaktifkan jenis konten yang mereka inginkan secara langsung pada perangkat secara manual, tetapi konfigurasi yang akan ditimpa oleh Intune pengaturan kebijakan, dan sinkronisasi berhenti untuk jenis konten tersebut.</span><span class="sxs-lookup"><span data-stu-id="de441-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

