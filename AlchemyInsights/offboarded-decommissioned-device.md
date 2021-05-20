---
title: Masalah dengan penghapusan perangkat offboarded atau yang dinonaktifkan dari Inventaris Perangkat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564340"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="308af-102">Masalah dengan penghapusan perangkat offboarded atau yang dinonaktifkan dari Inventaris Perangkat</span><span class="sxs-lookup"><span data-stu-id="308af-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="308af-103">Pertahanan Microsoft untuk Titik Akhir saat ini tidak mengizinkan penghapusan catatan perangkat dari perangkat offboarded atau yang dinonaktifkan secara manual dari Inventaris Perangkat.</span><span class="sxs-lookup"><span data-stu-id="308af-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="308af-104">Untuk tujuan keamanan, perangkat tetap ada di portal sebagai catatan riwayat hingga 180 hari.</span><span class="sxs-lookup"><span data-stu-id="308af-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="308af-105">Namun, data perangkat di purged sesuai dengan periode penyimpanan yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="308af-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="308af-106">**Catatan:** Perangkat yang dinonaktifkan atau offboarded akan beralih secara otomatis ke **keadaan Tidak** Aktif setelah tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="308af-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="308af-107">Selain itu, perangkat yang tidak aktif dalam 30 hari terakhir tidak difleksikan ke dalam data yang mencerminkan Pengelolaan Ancaman dan Kerentanan skor paparan atau Microsoft Secure Score untuk Perangkat.</span><span class="sxs-lookup"><span data-stu-id="308af-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="308af-108">Jika anda masih tidak ingin melihat perangkat tertentu dalam tampilan Inventaris Perangkat, coba tempatkan tag perangkat untuk memfilter perangkat yang dinonaktifkan dari tampilan Inventaris Perangkat.</span><span class="sxs-lookup"><span data-stu-id="308af-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="308af-109">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="308af-109">For more information, see:</span></span>

[<span data-ttu-id="308af-110">Perangkat offboard dari Pertahanan Microsoft untuk layanan Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="308af-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="308af-111">Skor paparan di Pengelolaan Ancaman dan Kerentanan</span><span class="sxs-lookup"><span data-stu-id="308af-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="308af-112">Memperbaiki sensor yang tidak sehat di Pertahanan Microsoft untuk Titik Akhir</span><span class="sxs-lookup"><span data-stu-id="308af-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="308af-113">Cara menggunakan penandaan secara efektif (Bagian 1)</span><span class="sxs-lookup"><span data-stu-id="308af-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="308af-114">Cara menggunakan penandaan secara efektif (Bagian 2)</span><span class="sxs-lookup"><span data-stu-id="308af-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="308af-115">Cara menggunakan penandaan secara efektif (Bagian 3)</span><span class="sxs-lookup"><span data-stu-id="308af-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




