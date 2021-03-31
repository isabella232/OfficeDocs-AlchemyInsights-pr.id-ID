---
title: EndPoint Manager - Garis dasar keamanan
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440887"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="e31db-102">EndPoint Manager - Garis dasar keamanan</span><span class="sxs-lookup"><span data-stu-id="e31db-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="e31db-103">Garis dasar keamanan adalah grup pengaturan Windows yang telah dikonfigurasi sebelumnya yang membantu Anda menerapkan pengaturan keamanan yang disarankan oleh tim keamanan terkait.</span><span class="sxs-lookup"><span data-stu-id="e31db-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="e31db-104">Garis dasar ini dapat disesuaikan untuk menampilkan pengaturan dan nilai yang diinginkan saja.</span><span class="sxs-lookup"><span data-stu-id="e31db-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="e31db-105">Untuk informasi selengkapnya tentang garis dasar keamanan, lihat [Menggunakan garis dasar keamanan untuk mengonfigurasi perangkat Windows 10 di Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="e31db-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="e31db-106">Saat ini, garis dasar tersedia untuk produk berikut:</span><span class="sxs-lookup"><span data-stu-id="e31db-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="e31db-107">Pengaturan Keamanan Windows MDM</span><span class="sxs-lookup"><span data-stu-id="e31db-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="e31db-108">Pertahanan Microsoft untuk Keamanan Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="e31db-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="e31db-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e31db-109">Microsoft Edge</span></span>

<span data-ttu-id="e31db-110">Setiap garis dasar diperbarui secara berkala dan dirilis dalam versi bertahap.</span><span class="sxs-lookup"><span data-stu-id="e31db-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="e31db-111">Setiap versi menambahkan dan atau menghapus pengaturan dari versi sebelumnya untuk memastikan bahwa garis dasar tersebut sesuai dengan panduan saat ini.</span><span class="sxs-lookup"><span data-stu-id="e31db-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="e31db-112">Konsol Garis dasar keamanan di Keamanan Titik Akhir memungkinkan perbandingan berbagai versi dengan menjadikan perubahan dari versi ke versi terlihat.</span><span class="sxs-lookup"><span data-stu-id="e31db-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="e31db-113">Untuk panduan tentang cara paling efektif mengubah versi garis dasar mana yang disebarkan, lihat [Mengelola profil garis dasar keamanan di Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="e31db-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="e31db-114">Setelah menyebarkan garis dasar keamanan, Anda dapat memantau status penyebaran dan meninjau pengaturan di masing-masing perangkat.</span><span class="sxs-lookup"><span data-stu-id="e31db-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="e31db-115">**Catatan:** Data pelaporan garis dasar mungkin baru muncul 24 jam setelah penyebaran awal ke perangkat, dan hingga 6 jam untuk pembaruan selanjutnya.</span><span class="sxs-lookup"><span data-stu-id="e31db-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="e31db-116">Penyebab paling umum mengapa pengaturan garis dasar tidak diterapkan adalah karena pengaturan yang sama sedang digunakan di profil berbeda.</span><span class="sxs-lookup"><span data-stu-id="e31db-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="e31db-117">Skenario ini dapat diselidiki untuk perangkat tertentu dengan memilih perangkat tersebut dari dalam node Status Perangkat pada profil Garis Dasar Keamanan.</span><span class="sxs-lookup"><span data-stu-id="e31db-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="e31db-118">Untuk selengkapnya, baca [Mengatasi konflik untuk garis dasar keamanan](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="e31db-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>