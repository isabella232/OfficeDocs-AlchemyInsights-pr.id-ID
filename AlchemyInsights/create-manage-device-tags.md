---
title: Membuat dan mengelola tag atau grup perangkat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731667"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="72d26-102">Membuat dan mengelola tag atau grup perangkat</span><span class="sxs-lookup"><span data-stu-id="72d26-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="72d26-103">Menambahkan tag pada perangkat untuk membuat afiliasi grup logis.</span><span class="sxs-lookup"><span data-stu-id="72d26-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="72d26-104">Tag perangkat mendukung pemetaan jaringan yang sesuai, memungkinkan Anda untuk melampirkan tag yang berbeda untuk merekam konteks dan memungkinkan pembuatan daftar dinamis sebagai bagian dari insiden.</span><span class="sxs-lookup"><span data-stu-id="72d26-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="72d26-105">Tag dapat digunakan sebagai filter dalam tampilan daftar Perangkat, atau untuk mengelompokkan perangkat.</span><span class="sxs-lookup"><span data-stu-id="72d26-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="72d26-106">Untuk informasi selengkapnya tentang mengelompokkan perangkat, lihat [Membuat dan mengelola tag perangkat](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="72d26-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="72d26-107">Anda bisa menambahkan tag di perangkat dengan:</span><span class="sxs-lookup"><span data-stu-id="72d26-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="72d26-108">Menggunakan portal</span><span class="sxs-lookup"><span data-stu-id="72d26-108">Using the portal</span></span>

- <span data-ttu-id="72d26-109">Mengatur nilai kunci registri</span><span class="sxs-lookup"><span data-stu-id="72d26-109">Setting a registry key value</span></span>
 
<span data-ttu-id="72d26-110">**Catatan:** Mungkin ada latensi antara waktu ketika tag ditambahkan ke perangkat dan ketersediaannya di halaman daftar perangkat dan perangkat.</span><span class="sxs-lookup"><span data-stu-id="72d26-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="72d26-111">Untuk menambahkan tag perangkat menggunakan API, lihat [Menambahkan atau menghapus API tag perangkat](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="72d26-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="72d26-112">Menambahkan dan mengelola tag perangkat menggunakan portal</span><span class="sxs-lookup"><span data-stu-id="72d26-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="72d26-113">Pilih perangkat yang ingin Anda kelola tagnya.</span><span class="sxs-lookup"><span data-stu-id="72d26-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="72d26-114">Anda bisa memilih atau mencari perangkat dari salah satu tampilan berikut ini:</span><span class="sxs-lookup"><span data-stu-id="72d26-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="72d26-115">**Dasbor operasi keamanan** Pilih nama perangkat dari bagian Perangkat teratas dengan pemberitahuan aktif.</span><span class="sxs-lookup"><span data-stu-id="72d26-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="72d26-116">**Peringatan antrean** - Pilih nama perangkat di samping ikon perangkat dari antrean peringatan.</span><span class="sxs-lookup"><span data-stu-id="72d26-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="72d26-117">**Daftar perangkat** - Pilih nama perangkat dari daftar perangkat.</span><span class="sxs-lookup"><span data-stu-id="72d26-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="72d26-118">**Kotak pencarian** - Pilih Perangkat dari menu menurun, lalu masukkan nama perangkat.</span><span class="sxs-lookup"><span data-stu-id="72d26-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="72d26-119">Anda juga bisa masuk ke halaman pemberitahuan melalui file dan tampilan IP.</span><span class="sxs-lookup"><span data-stu-id="72d26-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="72d26-120">Pilih **Kelola Tag** dari baris tindakan Respons.</span><span class="sxs-lookup"><span data-stu-id="72d26-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="72d26-121">Ketik untuk menemukan atau membuat tag.</span><span class="sxs-lookup"><span data-stu-id="72d26-121">Type to find or create tags.</span></span>

<span data-ttu-id="72d26-122">Tag ditambahkan ke tampilan perangkat dan dicerminkan di tampilan daftar Perangkat.</span><span class="sxs-lookup"><span data-stu-id="72d26-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="72d26-123">Selanjutnya Anda bisa menggunakan filter Tag untuk melihat daftar perangkat yang relevan.</span><span class="sxs-lookup"><span data-stu-id="72d26-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="72d26-124">Untuk informasi selengkapnya, lihat [Membuat dan mengelola tag perangkat](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="72d26-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>