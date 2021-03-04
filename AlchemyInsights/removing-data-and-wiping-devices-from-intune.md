---
title: Menghapus data dan menghapus perangkat secara menyeluruh dari Intune
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416316"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="d1108-102">Menghapus data dan menghapus perangkat secara menyeluruh dari Intune</span><span class="sxs-lookup"><span data-stu-id="d1108-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="d1108-103">Tindakan jarak jauh Penghentian Perangkat dan Penghapusan Perangkat dapat digunakan untuk menghapus data perusahaan yang dikelola oleh Intune atau untuk melakukan reset pabrik dan mengembalikan perangkat ke pengaturan default-nya.</span><span class="sxs-lookup"><span data-stu-id="d1108-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="d1108-104">Masuk ke Manajemen Perangkat Microsoft 365, lalu buka **Perangkat** > **Semua Perangkat**.</span><span class="sxs-lookup"><span data-stu-id="d1108-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="d1108-105">Pilih perangkat yang ingin Anda hapus.</span><span class="sxs-lookup"><span data-stu-id="d1108-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="d1108-106">Pilih jenis penghapusan jarak jauh yang ingin Anda lakukan.</span><span class="sxs-lookup"><span data-stu-id="d1108-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="d1108-107">Penghentian hanya menghapus informasi organisasi, sementara penghapusan menyeluruh mengembalikan perangkat ke pengaturan pabriknya.</span><span class="sxs-lookup"><span data-stu-id="d1108-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="d1108-108">Pilih **Ya** untuk mengonfirmasi.</span><span class="sxs-lookup"><span data-stu-id="d1108-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="d1108-109">Hingga penghapusan selesai, status tindakan perangkat ditampilkan sebagai *Penghentian Tertunda*.</span><span class="sxs-lookup"><span data-stu-id="d1108-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="d1108-110">Setelah tindakan selesai, Anda tidak akan melihat lagi perangkat seluler di daftar perangkat terkelola.</span><span class="sxs-lookup"><span data-stu-id="d1108-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="d1108-111">Data perusahaan tidak dapat dihapus dari perangkat yang BERGABUNG ke Microsoft Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1108-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="d1108-112">Untuk detail lengkap tentang dampak dari tindakan Penghentian dan Penghapusan, termasuk apa yang dipertahankan dan apa yang dihapus, lihat dokumentasi berikut:</span><span class="sxs-lookup"><span data-stu-id="d1108-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="d1108-113">[Hapus perangkat dengan menggunakan penghapusan menyeluruh, penghentian, atau pembatalan pendaftaran perangkat secara manual](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="d1108-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="d1108-114">Cara untuk hanya menghapus data perusahaan dari aplikasi yang dikelola Intune</span><span class="sxs-lookup"><span data-stu-id="d1108-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="d1108-115">[Hapus semua data dari perangkat macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="d1108-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>