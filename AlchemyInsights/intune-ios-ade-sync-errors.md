---
title: Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714832"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="d79ee-102">Kesalahan sinkronisasi pendaftaran perangkat otomatis Apple</span><span class="sxs-lookup"><span data-stu-id="d79ee-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="d79ee-103">"Kami telah mendeteksi bahwa Anda memiliki satu atau beberapa token ADE/DEP yang dalam kondisi kesalahan.</span><span class="sxs-lookup"><span data-stu-id="d79ee-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="d79ee-104">Hingga status kesalahan teratasi untuk setiap Token yang terpengaruh, fungsi ADE tidak akan berfungsi sama ".</span><span class="sxs-lookup"><span data-stu-id="d79ee-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="d79ee-105">Kesalahan ini mungkin terwujud dalam beberapa cara termasuk:</span><span class="sxs-lookup"><span data-stu-id="d79ee-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="d79ee-106">Perangkat mungkin tidak sinkron dari ABM/ASM ke Intune</span><span class="sxs-lookup"><span data-stu-id="d79ee-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="d79ee-107">Penetapan profil pendaftaran mungkin gagal</span><span class="sxs-lookup"><span data-stu-id="d79ee-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="d79ee-108">Perangkat mungkin tidak menyelesaikan pendaftaran ADE berhasil</span><span class="sxs-lookup"><span data-stu-id="d79ee-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="d79ee-109">Periksa kesalahan sinkronisasi yang dilaporkan dalam konsol Intune di bawah **perangkat > mendaftar perangkat > pendaftaran Apple > token program pendaftaran** dan Tinjau dokumentasi berikut ini untuk melihat potensi remediasi:</span><span class="sxs-lookup"><span data-stu-id="d79ee-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="d79ee-110">Kesalahan sinkronisasi ABM/ASM untuk iOS/iPadOS dan token pendaftaran perangkat otomatis macOS</span><span class="sxs-lookup"><span data-stu-id="d79ee-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
