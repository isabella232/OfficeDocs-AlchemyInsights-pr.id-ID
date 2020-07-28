---
title: Menghapus data dan menyeka perangkat dari Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439647"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="5f834-102">Menghapus data dan menyeka perangkat dari Intune</span><span class="sxs-lookup"><span data-stu-id="5f834-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="5f834-103">Device pensiun dan penghapusan perangkat tindakan jarak jauh dapat digunakan untuk menghapus data perusahaan yang dikelola oleh Intune atau melakukan reset pabrik dan mengembalikan perangkat ke pengaturan default.</span><span class="sxs-lookup"><span data-stu-id="5f834-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="5f834-104">Masuk ke Microsoft 365 manajemen perangkat, dan pergi ke **perangkat**  >  **semua perangkat**.</span><span class="sxs-lookup"><span data-stu-id="5f834-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="5f834-105">Pilih perangkat yang akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="5f834-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="5f834-106">Pilih jenis penghapusan jarak jauh yang ingin Anda lakukan.</span><span class="sxs-lookup"><span data-stu-id="5f834-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="5f834-107">Pensiun hanya menghapus informasi organisasi, sementara tisu penuh mengembalikan perangkat ke pengaturan pabriknya.</span><span class="sxs-lookup"><span data-stu-id="5f834-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="5f834-108">Pilih **ya** untuk mengonfirmasi.</span><span class="sxs-lookup"><span data-stu-id="5f834-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="5f834-109">Hingga penghapusan selesai, status tindakan perangkat akan ditampilkan sebagai pensiun tertunda.</span><span class="sxs-lookup"><span data-stu-id="5f834-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="5f834-110">Setelah tindakan selesai, Anda tidak akan lagi melihat perangkat seluler di Daftar perangkat yang dikelola.</span><span class="sxs-lookup"><span data-stu-id="5f834-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="5f834-111">**Catatan** Data perusahaan tidak dapat dihapus dari perangkat bergabung ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5f834-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="5f834-112">Untuk rincian lengkap tentang efek dari tindakan pensiun dan wipe, termasuk apa yang dipertahankan dan apa yang dihapus, lihat [menghapus perangkat dengan menggunakan wipe, pensiun, atau secara manual unenrolling perangkat](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="5f834-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="5f834-113">Untuk menghapus semua data dari perangkat macOS, lihat [menghapus semua data dari perangkat MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="5f834-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>