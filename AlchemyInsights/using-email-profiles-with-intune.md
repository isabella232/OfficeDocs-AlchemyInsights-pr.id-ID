---
title: Menggunakan profil email dengan Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653291"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="8de64-102">Menggunakan profil email dengan Intune</span><span class="sxs-lookup"><span data-stu-id="8de64-102">Using email profiles with Intune</span></span>

<span data-ttu-id="8de64-103">Intune dapat digunakan untuk membuat dan menggunakan profil email untuk klien email bawaan (bawaan) di beberapa platform perangkat.</span><span class="sxs-lookup"><span data-stu-id="8de64-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="8de64-104">Untuk informasi tentang beberapa larangan yang terkait dengan profil email, termasuk bagaimana kehadiran profil yang sudah ditangani dan cara menghapus profil email, lihat [menambahkan pengaturan email ke perangkat yang menggunakan Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="8de64-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="8de64-105">Untuk informasi selengkapnya tentang cara membuat profil email untuk setiap platform perangkat, lihat:</span><span class="sxs-lookup"><span data-stu-id="8de64-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="8de64-106">Pengaturan perangkat Android untuk mengonfigurasi email, autentikasi, dan sinkronisasi di Intune</span><span class="sxs-lookup"><span data-stu-id="8de64-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="8de64-107">Menambahkan pengaturan email untuk perangkat iOS dan iPadOS di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8de64-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="8de64-108">Pengaturan profil email di Microsoft Intune untuk perangkat yang menjalankan Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="8de64-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="8de64-109">Pengaturan profil email untuk perangkat yang menjalankan Windows 10 di Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8de64-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="8de64-110">**Masalah sinkronisasi Umum**</span><span class="sxs-lookup"><span data-stu-id="8de64-110">**Common syncing issue**</span></span>

<span data-ttu-id="8de64-111">**KNOX pada profil email Android mencegah kontak, kalender, dan tugas pengguna, agar tidak disinkronkan dengan perangkat pengguna.**</span><span class="sxs-lookup"><span data-stu-id="8de64-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="8de64-112">Profil email KNOX di Android KNOX menawarkan admin opsi untuk memutuskan tipe konten mana yang disinkronkan ke perangkat dengan mengatur masing-masing untuk diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="8de64-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="8de64-113">Jika pengaturan untuk salah satu tipe konten diatur ke **tidak dikonfigurasi** (default), tipe konten tersebut tidak disinkronkan secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="8de64-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="8de64-114">Pengguna mungkin mengaktifkan tipe konten yang mereka inginkan secara langsung di perangkat secara manual, tapi konfigurasi tersebut ditimpa dengan pengaturan kebijakan Intune, dan sinkronisasi berhenti untuk tipe konten tersebut.</span><span class="sxs-lookup"><span data-stu-id="8de64-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

