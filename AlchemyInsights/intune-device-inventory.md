---
title: Intune inventaris perangkat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439656"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="834b9-102">Intune inventaris perangkat</span><span class="sxs-lookup"><span data-stu-id="834b9-102">Intune Device Inventory</span></span>

<span data-ttu-id="834b9-103">Bilah perangkat memberikan wawasan administrator ke perangkat di bawah manajemen di Intune pada setiap perangkat.</span><span class="sxs-lookup"><span data-stu-id="834b9-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="834b9-104">Informasi yang ditampilkan meliputi: perangkat keras, aplikasi yang ditemukan, status kepatuhan perangkat, dan status konfigurasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="834b9-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="834b9-105">Data inventaris untuk perangkat keras dan aplikasi yang ditemukan dikumpulkan pada siklus tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="834b9-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="834b9-106">Aplikasi dan elemen spesifik perangkat keras yang dilaporkan berbeda tergantung pada sistem operasi perangkat dan apakah perangkat tersebut dimiliki secara pribadi atau perusahaan.</span><span class="sxs-lookup"><span data-stu-id="834b9-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="834b9-107">Untuk informasi selengkapnya, lihat [Lihat rincian perangkat di Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="834b9-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="834b9-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="834b9-108">**FAQ**</span></span>

<span data-ttu-id="834b9-109">Q: saya tidak menerima daftar lengkap persediaan aplikasi yang hadir pada perangkat Windows Intune-terdaftar.</span><span class="sxs-lookup"><span data-stu-id="834b9-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="834b9-110">Mengapa tidak?</span><span class="sxs-lookup"><span data-stu-id="834b9-110">Why not?</span></span>

<span data-ttu-id="834b9-111">A: saat ini, hanya aplikasi modern yang terdaftar untuk PC Windows 10 yang diidentifikasi sebagai perangkat korporat.</span><span class="sxs-lookup"><span data-stu-id="834b9-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="834b9-112">Intune tidak mengumpulkan informasi tentang aplikasi Win32 diinstal pada perangkat ini.</span><span class="sxs-lookup"><span data-stu-id="834b9-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="834b9-113">T: Mengapa nomor telepon tidak dikumpulkan dari semua perangkat?</span><span class="sxs-lookup"><span data-stu-id="834b9-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="834b9-114">A: telepon dikategorikan sebagai perangkat korporat di Intune tidak diidentifikasi dengan nomor telepon penuh ketika, misalnya, Anda menjalankan laporan inventaris perangkat seluler.</span><span class="sxs-lookup"><span data-stu-id="834b9-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="834b9-115">Membawa-Anda-sendiri-nomor telepon perangkat selalu ditutupi sebagian dengan tanda bintang (\* \* \* \*), dan hanya menampilkan empat digit terakhir.</span><span class="sxs-lookup"><span data-stu-id="834b9-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>