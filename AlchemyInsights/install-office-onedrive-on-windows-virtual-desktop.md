---
title: Menginstal Office dan OneDrive di Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595848"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="ec631-102">Menginstal Office dan OneDrive di Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="ec631-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="ec631-103">[Mempersiapkan dan mengustomisasi gambar VHD master](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="ec631-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="ec631-104">Buat mesin virtual (VM) jika belum dibuat.</span><span class="sxs-lookup"><span data-stu-id="ec631-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="ec631-105">[Menginstal Office dalam mode aktivasi komputer bersama.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="ec631-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="ec631-106">Aktivasi komputer bersama memungkinkan beberapa pengguna mengakses Office.</span><span class="sxs-lookup"><span data-stu-id="ec631-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="ec631-107">[Instal OneDrive dalam mode per komputer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="ec631-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="ec631-108">Biasanya OneDrive diinstal per pengguna, namun di sini, OneDrive harus diinstal per komputer.</span><span class="sxs-lookup"><span data-stu-id="ec631-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>