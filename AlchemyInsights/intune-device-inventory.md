---
title: Intune perangkat inventaris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667881"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="71a4f-102">Intune perangkat inventaris</span><span class="sxs-lookup"><span data-stu-id="71a4f-102">Intune Device Inventory</span></span>

<span data-ttu-id="71a4f-103">Bilah perangkat menyediakan wawasan administrator ke perangkat di bawah manajemen di Intune pada basis per perangkat.</span><span class="sxs-lookup"><span data-stu-id="71a4f-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="71a4f-104">Informasi yang diperlihatkan meliputi: perangkat keras, aplikasi yang ditemukan, status kepatuhan perangkat, dan status konfigurasi perangkat.</span><span class="sxs-lookup"><span data-stu-id="71a4f-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="71a4f-105">Inventaris data untuk perangkat keras dan ditemukan aplikasi dikumpulkan dalam siklus tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="71a4f-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="71a4f-106">Aplikasi dan elemen perangkat keras tertentu yang dilaporkan berbeda tergantung pada sistem operasi perangkat dan apakah perangkat tersebut bersifat pribadi atau milik perusahaan.</span><span class="sxs-lookup"><span data-stu-id="71a4f-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="71a4f-107">Untuk informasi selengkapnya, lihat [melihat detail perangkat di Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="71a4f-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="71a4f-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="71a4f-108">**FAQ**</span></span>

<span data-ttu-id="71a4f-109">T: saya tidak menerima daftar inventaris lengkap tentang aplikasi yang ada di perangkat Windows yang didaftarkan Intune.</span><span class="sxs-lookup"><span data-stu-id="71a4f-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="71a4f-110">Mengapa tidak?</span><span class="sxs-lookup"><span data-stu-id="71a4f-110">Why not?</span></span>

<span data-ttu-id="71a4f-111">J: saat ini, hanya aplikasi modern yang dicantumkan untuk PC Windows 10 yang diidentifikasi sebagai perangkat korporat.</span><span class="sxs-lookup"><span data-stu-id="71a4f-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="71a4f-112">Intune tidak mengumpulkan informasi tentang aplikasi Win32 yang terinstal di perangkat ini.</span><span class="sxs-lookup"><span data-stu-id="71a4f-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="71a4f-113">P: Mengapa nomor telepon tidak dikumpulkan dari semua perangkat?</span><span class="sxs-lookup"><span data-stu-id="71a4f-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="71a4f-114">A: telepon yang dikategorikan sebagai perangkat korporat di Intune tidak diidentifikasi dengan nomor telepon lengkap mereka saat, misalnya, Anda menjalankan laporan inventaris perangkat seluler.</span><span class="sxs-lookup"><span data-stu-id="71a4f-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="71a4f-115">Bawalah-Anda-sendiri-nomor telepon perangkat selalu ditutupi dengan tanda bintang (\* \* \* \*), dan hanya memperlihatkan empat digit terakhir.</span><span class="sxs-lookup"><span data-stu-id="71a4f-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>