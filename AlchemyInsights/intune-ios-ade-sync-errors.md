---
title: Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448925"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="80a9f-102">Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple</span><span class="sxs-lookup"><span data-stu-id="80a9f-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="80a9f-103">"Kami telah mendeteksi bahwa Anda memiliki satu atau beberapa token ADE/DEP yang dalam kondisi kesalahan.</span><span class="sxs-lookup"><span data-stu-id="80a9f-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="80a9f-104">Hingga status kesalahan teratasi untuk setiap Token yang terpengaruh, fungsi ADE tidak akan berfungsi seperti yang diharapkan. ".</span><span class="sxs-lookup"><span data-stu-id="80a9f-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="80a9f-105">Kesalahan ini mungkin terwujud dalam beberapa cara termasuk:</span><span class="sxs-lookup"><span data-stu-id="80a9f-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="80a9f-106">Perangkat mungkin tidak sinkron dari ABM/ASM ke Intune</span><span class="sxs-lookup"><span data-stu-id="80a9f-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="80a9f-107">Penetapan profil pendaftaran mungkin gagal</span><span class="sxs-lookup"><span data-stu-id="80a9f-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="80a9f-108">Perangkat mungkin tidak menyelesaikan pendaftaran ADE berhasil</span><span class="sxs-lookup"><span data-stu-id="80a9f-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="80a9f-109">Periksa kesalahan sinkronisasi yang dilaporkan dalam konsol Intune di bawah **perangkat > mendaftar perangkat > pendaftaran > token program pendaftaran**.</span><span class="sxs-lookup"><span data-stu-id="80a9f-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="80a9f-110">Salah satu penyebab kesalahan sinkronisasi paling umum adalah berakhirnya token saat ini.</span><span class="sxs-lookup"><span data-stu-id="80a9f-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="80a9f-111">Dalam banyak kasus, pembaruan Token yang terpengaruh akan mengatasi masalah tersebut.</span><span class="sxs-lookup"><span data-stu-id="80a9f-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="80a9f-112">Jika satu atau beberapa token Anda telah kedaluwarsa, lihat dokumentasi berikut ini untuk membantu Anda memperbaruinya sesuai keperluan:</span><span class="sxs-lookup"><span data-stu-id="80a9f-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="80a9f-113">Memperpanjang token pendaftaran perangkat otomatis</span><span class="sxs-lookup"><span data-stu-id="80a9f-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="80a9f-114">Selain itu, Anda bisa melihat dokumentasi berikut ini untuk melihat potensi remediasi untuk kesalahan lain yang menyebabkan kegagalan sinkronisasi token:</span><span class="sxs-lookup"><span data-stu-id="80a9f-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="80a9f-115">Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS</span><span class="sxs-lookup"><span data-stu-id="80a9f-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="80a9f-116">Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS</span><span class="sxs-lookup"><span data-stu-id="80a9f-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
