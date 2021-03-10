---
title: Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694434"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="6cc8a-102">Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10</span><span class="sxs-lookup"><span data-stu-id="6cc8a-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="6cc8a-103">Dasar-dasar keamanan Intune membantu melindungi pengguna dan perangkat.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="6cc8a-104">Baseline keamanan adalah grup yang dikonfigurasi sebelumnya dari pengaturan Windows yang digunakan untuk menerapkan grup pengaturan dan nilai default yang diketahui yang direkomendasikan oleh tim keamanan yang relevan.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="6cc8a-105">Dengan membuat profil baseline keamanan di Intune, Anda membuat Templat yang terdiri dari beberapa profil konfigurasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="6cc8a-106">Saat Anda menggunakan baseline keamanan untuk grup pengguna atau perangkat, pengaturan diterapkan ke perangkat yang berjalan pada versi Windows 10 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="6cc8a-107">Misalnya, baseline keamanan manajemen perangkat seluler (MDM) Microsoft secara otomatis (1) memungkinkan BitLocker untuk drive yang dapat dilepas, (2) memerlukan kata sandi untuk membuka kunci perangkat, dan (3) menonaktifkan autentikasi dasar.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="6cc8a-108">Saat nilai default tidak berfungsi untuk lingkungan Anda, Anda bisa mengustomisasi baseline untuk menerapkan pengaturan yang Anda perlukan.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="6cc8a-109">Baseline keamanan juga membantu membuat alur kerja aman menyeluruh di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="6cc8a-110">Berikut ini adalah beberapa manfaat dari fungsionalitas ini:</span><span class="sxs-lookup"><span data-stu-id="6cc8a-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="6cc8a-111">Baseline keamanan menyertakan praktik terbaik dan saran untuk pengaturan yang mempengaruhi keamanan.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="6cc8a-112">Karena mitra Intune dengan tim keamanan Windows yang membuat baseline untuk kebijakan grup, rekomendasi ini didasarkan pada panduan yang solid dan pengalaman yang luas.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="6cc8a-113">Jika Anda baru menggunakan Intune dan tidak yakin tempat memulainya, baseline keamanan akan membantu Anda membuat dan menggunakan profil aman dengan cepat.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="6cc8a-114">Jika saat ini Anda menggunakan kebijakan grup, maka migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan, karena baseline keamanan ini dibangun ke dalam Intune dan menyertakan kapabilitas mutakhir untuk manajemen.</span><span class="sxs-lookup"><span data-stu-id="6cc8a-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="6cc8a-115">Untuk informasi selengkapnya, lihat baseline [keamanan Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) dan [manajemen perangkat seluler](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="6cc8a-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>