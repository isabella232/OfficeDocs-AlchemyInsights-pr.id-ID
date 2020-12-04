---
title: Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573539"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="de393-102">Menggunakan baseline keamanan Microsoft Intune untuk mengonfigurasi perangkat Windows 10</span><span class="sxs-lookup"><span data-stu-id="de393-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="de393-103">Dasar-dasar keamanan Intune membantu melindungi pengguna dan perangkat.</span><span class="sxs-lookup"><span data-stu-id="de393-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="de393-104">Baseline keamanan adalah grup yang dikonfigurasi sebelumnya dari pengaturan Windows yang digunakan untuk menerapkan grup pengaturan dan nilai default yang diketahui yang direkomendasikan oleh tim keamanan yang relevan.</span><span class="sxs-lookup"><span data-stu-id="de393-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="de393-105">Dengan membuat profil baseline keamanan di Intune, Anda membuat Templat yang terdiri dari beberapa profil konfigurasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="de393-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="de393-106">Saat Anda menggunakan baseline keamanan untuk grup pengguna atau perangkat, pengaturan diterapkan ke perangkat yang berjalan di Windows 10 atau yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="de393-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="de393-107">Misalnya, Baseline Security baseline secara otomatis (1) memungkinkan BitLocker untuk drive yang dapat dilepas, (2) memerlukan kata sandi untuk membuka kunci perangkat, dan (3) menonaktifkan autentikasi dasar.</span><span class="sxs-lookup"><span data-stu-id="de393-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="de393-108">Jika nilai default tidak berfungsi untuk lingkungan Anda, kustomisasi baseline untuk menerapkan pengaturan yang Anda perlukan.</span><span class="sxs-lookup"><span data-stu-id="de393-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="de393-109">Baseline keamanan juga membantu membuat alur kerja aman menyeluruh di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="de393-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="de393-110">Berikut ini adalah beberapa manfaat dari hal ini:</span><span class="sxs-lookup"><span data-stu-id="de393-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="de393-111">Baseline keamanan menyertakan praktik terbaik dan saran untuk pengaturan yang mempengaruhi keamanan.</span><span class="sxs-lookup"><span data-stu-id="de393-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="de393-112">Karena mitra Intune dengan tim keamanan Windows yang membuat baseline untuk kebijakan grup, rekomendasi ini didasarkan pada panduan yang solid dan pengalaman yang luas.</span><span class="sxs-lookup"><span data-stu-id="de393-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="de393-113">Jika Anda baru menggunakan Intune dan tidak yakin tempat memulainya, baseline keamanan akan membantu Anda membuat dan menggunakan profil aman dengan cepat.</span><span class="sxs-lookup"><span data-stu-id="de393-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="de393-114">Jika saat ini Anda menggunakan kebijakan grup, maka migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan, karena dibangun ke dalam Intune dan menyertakan kapabilitas terdepan untuk manajemen.</span><span class="sxs-lookup"><span data-stu-id="de393-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="de393-115">Untuk mempelajari selengkapnya, lihat [baseline keamanan Windows](https://go.microsoft.com/fwlink/?linkid=2141503) dan [manajemen perangkat seluler](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="de393-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>