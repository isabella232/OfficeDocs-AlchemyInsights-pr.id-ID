---
title: Manajer EndPoint - Baseline keamanan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421094"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="25e20-102">Manajer EndPoint - Baseline keamanan</span><span class="sxs-lookup"><span data-stu-id="25e20-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="25e20-103">Baseline keamanan adalah grup Windows yang sudah dikonfigurasi sebelumnya yang membantu Anda menerapkan pengaturan keamanan yang direkomendasikan oleh tim keamanan yang relevan.</span><span class="sxs-lookup"><span data-stu-id="25e20-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="25e20-104">Baseline ini dapat dikustomisasi untuk memberikan pengaturan dan nilai yang diinginkan saja.</span><span class="sxs-lookup"><span data-stu-id="25e20-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="25e20-105">Untuk informasi selengkapnya tentang baseline keamanan, lihat [Menggunakan baseline keamanan untuk mengonfigurasi perangkat Windows 10 di Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="25e20-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="25e20-106">Saat ini ada baseline untuk produk ini:</span><span class="sxs-lookup"><span data-stu-id="25e20-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="25e20-107">Pengaturan Keamanan Windows MDM</span><span class="sxs-lookup"><span data-stu-id="25e20-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="25e20-108">Pertahanan Microsoft untuk Keamanan EndPoint</span><span class="sxs-lookup"><span data-stu-id="25e20-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="25e20-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="25e20-109">Microsoft Edge</span></span>

<span data-ttu-id="25e20-110">Setiap garis dasar diperbarui secara berkala dan dirilis dalam versi bertahap.</span><span class="sxs-lookup"><span data-stu-id="25e20-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="25e20-111">Setiap versi menambahkan dan atau menghapus pengaturan dari versi sebelumnya untuk memastikan bahwa garis dasar memenuhi panduan saat ini.</span><span class="sxs-lookup"><span data-stu-id="25e20-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="25e20-112">Konsol dasar keamanan di Keamanan Titik Akhir memungkinkan versi yang berbeda dibandingkan dengan membuat perubahan dari versi ke versi terlihat.</span><span class="sxs-lookup"><span data-stu-id="25e20-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="25e20-113">Untuk panduan tentang cara paling efektif mengubah versi baseline yang digunakan, lihat Mengelola profil [garis dasar keamanan di Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="25e20-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="25e20-114">Setelah menggunakan baseline keamanan, Anda bisa memantau status penggunaan dan meninjau pengaturan pada basis perangkat demi perangkat.</span><span class="sxs-lookup"><span data-stu-id="25e20-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="25e20-115">**Catatan:** Data pelaporan untuk baseline mungkin memakan waktu hingga 24 jam agar muncul dari penggunaan awal ke perangkat dan hingga 6 jam untuk pembaruan lebih lanjut.</span><span class="sxs-lookup"><span data-stu-id="25e20-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="25e20-116">Penyebab paling umum dari pengaturan garis dasar yang tidak diterapkan adalah karena pengaturan yang sama yang digunakan di profil berbeda.</span><span class="sxs-lookup"><span data-stu-id="25e20-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="25e20-117">Skenario ini dapat diselidiki untuk perangkat tertentu dengan memilih perangkat tersebut dari dalam node Status Perangkat di profil Garis Dasar Keamanan.</span><span class="sxs-lookup"><span data-stu-id="25e20-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="25e20-118">Untuk detailnya, [lihat Mengatasi konflik untuk baseline keamanan.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="25e20-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>