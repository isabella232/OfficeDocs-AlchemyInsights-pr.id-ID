---
title: Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793898"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="a6d03-102">Menggunakan Microsoft Intune baseline keamanan untuk mengonfigurasi Windows 10 Anda</span><span class="sxs-lookup"><span data-stu-id="a6d03-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="a6d03-103">Baseline keamanan Intune membantu melindungi pengguna dan perangkat.</span><span class="sxs-lookup"><span data-stu-id="a6d03-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="a6d03-104">Baseline keamanan adalah Windows yang telah dikonfigurasi sebelumnya oleh grup yang digunakan untuk menerapkan grup pengaturan umum dan nilai default yang direkomendasikan oleh tim keamanan yang relevan.</span><span class="sxs-lookup"><span data-stu-id="a6d03-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="a6d03-105">Dengan membuat profil baseline keamanan di Intune, Anda membuat templat yang terdiri dari beberapa profil konfigurasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="a6d03-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="a6d03-106">Saat Anda menerapkan baseline keamanan ke sejumlah pengguna atau perangkat, pengaturan akan diterapkan ke perangkat yang dijalankan di Windows 10 baru.</span><span class="sxs-lookup"><span data-stu-id="a6d03-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="a6d03-107">Misalnya, baseline keamanan manajemen perangkat seluler (MDM) Microsoft secara otomatis mengaktifkan BitLocker untuk drive yang dapat dilepas, memerlukan kata sandi untuk membuka kunci perangkat, dan menonaktifkan autentikasi dasar.</span><span class="sxs-lookup"><span data-stu-id="a6d03-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="a6d03-108">Ketika nilai default tidak berfungsi untuk lingkungan Anda, Anda bisa mengkustomisasi garis dasar untuk menerapkan pengaturan yang Anda perlukan.</span><span class="sxs-lookup"><span data-stu-id="a6d03-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="a6d03-109">Baseline keamanan juga membantu menetapkan alur kerja aman secara end-to-end Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a6d03-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="a6d03-110">Baseline keamanan mencakup praktik terbaik dan rekomendasi untuk pengaturan yang mempengaruhi keamanan.</span><span class="sxs-lookup"><span data-stu-id="a6d03-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="a6d03-111">Intune bermitra dengan Windows keamanan grup yang membuat baseline untuk kebijakan grup, sehingga rekomendasi ini didasarkan pada panduan yang solid dan pengalaman ekstensif.</span><span class="sxs-lookup"><span data-stu-id="a6d03-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="a6d03-112">Jika Anda baru menggunakan Intune dan tidak yakin dari mana memulai, baseline keamanan membantu Anda membuat dan menggunakan profil yang aman dengan cepat.</span><span class="sxs-lookup"><span data-stu-id="a6d03-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="a6d03-113">Jika saat ini Anda menggunakan kebijakan grup, melakukan migrasi ke Intune untuk tujuan manajemen jauh lebih mudah dengan baseline keamanan karena baseline keamanan disertakan dalam Intune dan menyertakan kapabilitas manajemen yang canggih.</span><span class="sxs-lookup"><span data-stu-id="a6d03-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="a6d03-114">Untuk mempelajari selengkapnya, lihat [Windows dasar keamanan dan](/windows/security/threat-protection/windows-security-baselines) Manajemen perangkat [seluler](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="a6d03-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

